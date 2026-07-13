# Evaluating the Faithfulness of LLM-Generated Explanations for Injection-Molding Failure Prediction

This repository contains the experimental pipeline for evaluating whether large language models (LLMs) can translate local model-attribution evidence into clear, manufacturing-relevant explanations without introducing unsupported causal or process-value claims.

The study uses an injection-molding quality dataset, compares three gradient-boosting classifiers, extracts local feature-attribution evidence from the selected model, generates operator-facing explanations with three LLMs, and evaluates those explanations using an LLM-as-Judge protocol and a human-expert evaluation stage.

## Research question

> To what extent can different LLMs translate local model-attribution evidence into concise and manufacturing-relevant explanations without introducing unsupported causal or process-value claims?

## Main idea

A local feature attribution shows how a feature influenced a model prediction.

- A positive attribution indicates that the feature pushed the prediction toward **Fail**.
- A negative attribution indicates that the feature pushed the prediction toward **Pass**.
- The attribution sign does **not** show that the measured value was high, low, increasing, abnormal, or physically responsible for the defect.
- The attribution magnitude is used only to rank features by their influence on the model output.

The project evaluates whether LLM-generated explanations preserve these distinctions.

## Study pipeline

1. Prepare the injection-molding dataset.
2. Create a chronological train/test split.
3. Tune CatBoost, LightGBM, and XGBoost using time-aware validation.
4. Select the predictive model using temporal cross-validation PR-AUC.
5. Select observed non-startup failure cases from the held-out test set.
6. Extract local model-attribution evidence for each selected case.
7. Generate explanations using three LLMs.
8. Evaluate the explanations using a blinded LLM-as-Judge protocol.
9. Compare the automated evaluation with an independent human-expert assessment.

## Dataset

The study uses an injection-molding process dataset obtained from the Korea AI Manufacturing Platform (KAMP). The original dataset page is available through the [KAMP AI Dataset Detail page](https://www.kamp-ai.kr/aidataDetail?AI_SEARCH=&page=1&DATASET_SEQ=4&EQUIP_SEL=&GUBUN_SEL=&FILE_TYPE_SEL=&WDATE_SEL=).

The dataset preparation and initial injection-molding analysis are based on the public [Injection Molding Analysis GitHub repository](https://github.com/johnwslee/injection_molding_analysis/tree/main). This repository extends that work by adding predictive-model comparison, local model-attribution extraction, LLM-generated explanations, LLM-as-Judge evaluation, and human-expert assessment.

- **Production cycles:** 5,232
- **Features:** 35
- **Passing cycles:** 5,172
- **Failing cycles:** 60
- **Failure rate:** approximately 1.15%

Recorded failure reasons include:

- gas-related defects;
- incomplete-molding or short-shot defects;
- startup defects.

The chronological split contains:

| Split | Total cycles | Failures |
|---|---:|---:|
| Training set | 4,174 | 45 |
| Test set | 1,058 | 15 |

Startup defects are excluded from the explanation analysis. The final explanation set contains ten non-startup failure cases:

- five gas-related failures;
- five incomplete-molding failures.

All ten cases are false-negative predictions: the production cycles were recorded as failures, but the selected classifier predicted them as passing cases.

## Predictive models

Three gradient-boosting classifiers are evaluated:

- CatBoost
- LightGBM
- XGBoost

Hyperparameters are optimized using Optuna and time-aware cross-validation.

### Why PR-AUC?

PR-AUC is used as the main model-selection metric because failures are rare in the dataset. It measures how well a model identifies the rare failure class while accounting for false alarms and is more informative than overall accuracy for highly imbalanced classification problems.

### Decision threshold

Each model produces a probability that a production cycle will fail. A decision threshold converts this probability into a final **Pass** or **Fail** prediction.

Because the failure class is rare, the default threshold of 0.5 may miss many actual failures. A separate threshold is therefore selected for each model using validation predictions from the training data. The threshold maximizes the F2-score, which gives greater importance to detecting real failures while still considering false alarms.

### Model results

| Model | Temporal CV PR-AUC | Test PR-AUC | Failure recall | Failure F1 |
|---|---:|---:|---:|---:|
| **CatBoost** | **0.1604** | 0.3328 | 0.2000 | 0.2857 |
| LightGBM | 0.1051 | **0.3576** | **0.5333** | **0.3404** |
| XGBoost | 0.0651 | 0.2755 | 0.3333 | 0.1887 |

CatBoost is selected because it achieved the highest temporal cross-validation PR-AUC. The held-out test set is not used for model selection.

Although LightGBM performs better on the test set, selecting it based on test performance would weaken the independence of the final evaluation.

## Model-attribution evidence

For each selected failure case, the CatBoost model is used to calculate local feature attributions.

The evidence package supplied to the explanation-generating LLM contains:

| Field | Description |
|---|---|
| `feature_name` | Technical name of the process variable |
| `feature_description` | Manufacturing-readable description |
| `feature_attribution` | Signed local attribution value |
| `absolute_attribution` | Absolute value used only for ranking |
| `direction` | Whether the feature pushed the prediction toward **Fail** or **Pass** |

Example:

| Feature | Manufacturing-readable description | Attribution | Direction |
|---|---|---:|---|
| `Max_Injection_Pressure` | Maximum pressure recorded during injection | 0.8178 | Toward Fail |
| `Plasticizing_Time` | Time required to prepare and melt material | -0.7993 | Toward Pass |
| `Mold_Temperature_4` | Temperature in the fourth monitored mold zone | -0.6905 | Toward Pass |
| `Max_Screw_RPM` | Maximum screw rotation speed | 0.5960 | Toward Fail |

A positive or negative attribution describes model behavior only. It does not establish physical causality or indicate whether the raw process value was high, low, normal, or abnormal.

## LLM-based explanation generation

Three LLMs generate a short operator-facing explanation for each of the ten selected cases:

- GPT-5.4 mini
- Gemini 3.1 Flash-Lite
- Mistral Devstral 2512

Each model receives the same attribution evidence and feature descriptions.

The prompt instructs the models to:

- identify the most influential process variables;
- preserve the direction of each contribution;
- explain the evidence in manufacturing language;
- avoid unsupported claims about high, low, increasing, decreasing, or abnormal values;
- avoid presenting model attribution as proof of physical causation.

This produces **30 explanations** in total.

## LLM-as-Judge evaluation

The explanations are evaluated using a blinded and randomly ordered LLM-as-Judge protocol.

For each case, the judge receives:

- the local model-attribution evidence;
- three anonymized explanations;
- the evaluation rubric.

The identities of the explanation-generating models are hidden, and the candidate order is randomized.

Each explanation is scored from 1 to 5 using three criteria:

| Acronym | Criterion | Evaluation focus |
|---|---|---|
| EF | Evidence faithfulness | Whether the explanation accurately reflects the supplied model-attribution evidence |
| AC | Attribution caution | Whether the explanation avoids unsupported claims about process values, abnormality, or physical causation |
| MPR | Manufacturing-process relevance | Whether the explanation is meaningful in an injection-molding context |

The overall score is the arithmetic mean of EF, AC, and MPR.

### LLM-as-Judge results

| Explanation model | EF | AC | MPR | Overall |
|---|---:|---:|---:|---:|
| **GPT-5.4 mini** | **4.10** | 3.30 | **4.50** | **3.97** |
| Gemini 3.1 Flash-Lite | 3.20 | **4.10** | 3.90 | 3.73 |
| Mistral Devstral 2512 | 3.60 | 3.40 | 4.30 | 3.77 |

GPT-5.4 mini achieves the highest mean overall score. Gemini 3.1 Flash-Lite receives the highest attribution-caution score, while Mistral Devstral 2512 performs strongly in manufacturing-process relevance.

## Main finding

The explanations generally identify whether a feature pushed the prediction toward failure or toward passing. However, some explanations incorrectly describe process values as high, low, increasing, or abnormal, even though the attribution evidence does not contain that information.

This shows that readable explanations are not necessarily faithful explanations.

## Human-expert evaluation

The framework also includes an independent human-expert evaluation of the same explanations.

The human expert evaluates:

- evidence faithfulness;
- attribution caution;
- manufacturing-process relevance.

The expert assessment is intended to determine whether the LLM-as-Judge scores are consistent with domain-informed human judgment.

> **Current status:** the human-expert evaluation procedure is included in the study design, but the final expert scores and agreement analysis will be added after the assessment is completed.

Recommended agreement analyses include:

- Spearman rank correlation;
- Pearson correlation;
- mean absolute score difference;
- weighted Cohen's kappa for ordinal ratings;
- comparison of model rankings produced by the human expert and the LLM judge.

## Repository contents

The main analysis is organized into the following notebooks:

```text
02_ml_xai_new.ipynb
    Predictive-model training, temporal validation, threshold selection,
    test evaluation, failure-case selection, and local attribution extraction.

03_llm_as_judge_new.ipynb
    Parsing generated explanations, anonymization, randomization,
    LLM-as-Judge evaluation, scoring, and result aggregation.
```

Generated outputs include:

```text
explanation_results_sikdd.md
    LLM-generated explanations for the selected failure cases.

llm_as_judge_row_*.md
    Per-case judge reports containing criterion scores and justifications.
```

The exact filenames may contain numeric suffixes depending on the downloaded version.

## Installation

Create a Python environment and install the dependencies used by the notebooks.

```bash
python -m venv .venv
source .venv/bin/activate
```

On Windows:

```powershell
python -m venv .venv
.venv\Scripts\activate
```

Install the required packages:

```bash
pip install pandas numpy scikit-learn catboost lightgbm xgboost optuna shap matplotlib jupyter
```

The LLM notebooks may also require the client library used to access the selected model provider or routing service.

Store API credentials in environment variables rather than directly in the notebooks.

Example:

```bash
export OPENAI_API_KEY="your-key"
```

On Windows PowerShell:

```powershell
$env:OPENAI_API_KEY="your-key"
```

## Running the experiments

Run the notebooks in the following order:

1. `02_ml_xai_new.ipynb`
2. Generate the three explanations for each selected case.
3. Save the explanation output as `explanation_results_sikdd.md`.
4. Run `03_llm_as_judge_new.ipynb`.
5. Add the human-expert ratings.
6. Compare the automated and human evaluations.

Start Jupyter with:

```bash
jupyter notebook
```

## Reproducibility notes

To improve reproducibility:

- keep the chronological train/test split fixed;
- record all random seeds;
- save Optuna study configurations;
- record package versions;
- preserve the selected decision thresholds;
- save the exact prompts used for explanation generation and judging;
- save the randomized candidate order for each judge run;
- record the exact model identifiers and execution date.

## Scope and limitations

This repository evaluates explanation faithfulness, not physical root-cause discovery.

Important limitations include:

- only ten non-startup failure cases are evaluated;
- all ten selected cases are false negatives;
- the predictive dataset is highly imbalanced;
- only two temporal validation folds contain failures and are usable for PR-AUC evaluation;
- local feature attribution explains model behavior, not physical causality;
- LLM-as-Judge evaluation can contain its own biases;
- the human-expert evaluation is required to validate the automated assessment;
- conclusions should not be generalized beyond the evaluated dataset, models, prompts, and cases without further testing.

## Ethical and practical use

The generated explanations should be treated as decision-support material rather than definitive manufacturing diagnoses.

They should not replace:

- process-engineering review;
- equipment inspection;
- quality-control procedures;
- validated operating limits;
- expert root-cause analysis.

## Data sources

- [Injection Molding Analysis GitHub repository](https://github.com/johnwslee/injection_molding_analysis/tree/main)
- [KAMP AI Dataset Detail page](https://www.kamp-ai.kr/aidataDetail?AI_SEARCH=&page=1&DATASET_SEQ=4&EQUIP_SEL=&GUBUN_SEL=&FILE_TYPE_SEL=&WDATE_SEL=)

## Citation

A formal citation will be added after publication.

```bibtex
@article{hosseini_llm_injection_molding,
  title   = {Evaluating the Faithfulness of LLM-Generated Explanations for Injection-Molding Failure Prediction Using Model-Attribution Evidence},
  author  = {Hosseini, Seyed Iman and Mladenic, Dunja},
  year    = {2026},
  note    = {Manuscript in preparation}
}
```

## License

Add the repository license here, for example:

```text
MIT License
```

or replace this section with the license selected for the project.
