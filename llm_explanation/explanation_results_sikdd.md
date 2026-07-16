

## Top 10 SHAP Features for Index Row 115

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| Mold_Temperature_4              |              1.57373  |               1.57373  | toward Fail |
| Mold_Temperature_3              |              1.08837  |               1.08837  | toward Fail |
| Plasticizing_Position           |              0.809664 |               0.809664 | toward Fail |
| Clamp_Close_Time                |              0.644952 |               0.644952 | toward Fail |
| Cushion_Position                |              0.328427 |               0.328427 | toward Fail |
| Max_Injection_Speed             |              0.312462 |               0.312462 | toward Fail |
| Injection_Time                  |              0.270415 |               0.270415 | toward Fail |
| Max_Injection_Pressure          |              0.185559 |               0.185559 | toward Fail |
| Average_Screw_RPM               |              0.174312 |               0.174312 | toward Fail |
| PART_NAME_CN7 W/S SIDE MLD'G LH |             -0.136279 |               0.136279 | toward Pass |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 115

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was driven mainly by elevated temperatures in two mold zones, which were the strongest factors pushing toward Fail. Plasticizing position, clamp close time, and cushion position also added to that failure-risk assessment, with additional support from higher injection speed, longer injection time, higher injection pressure, and higher screw speed during material preparation. These process signals collectively made the cycle look more failure-prone to the model, but they do not prove any physical root cause. The part type for this cycle pushed in the opposite direction and slightly reduced the failure-risk assessment.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 115

**Reason:** 미성형 => Unshaped

The process conditions for this production cycle showed multiple factors increasing the failure-risk assessment, primarily driven by temperature readings in two separate mold zones. Additionally, the screw position during plasticizing, the mold clamp closing time, and the volume of material remaining at the end of injection further contributed to this assessment. Conversely, the specific product part type was the only notable factor acting to reduce the failure-risk assessment. These observations reflect the influence of recorded settings on the current risk assessment but do not confirm the physical cause of any potential defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 115

**Reason:** 미성형 => Unshaped

Higher temperatures in two monitored mold zones (Mold_Temperature_4 and Mold_Temperature_3) most strongly increased the model's failure-risk assessment for this cycle. The plasticizing screw position, longer clamp-close time, and smaller cushion position also contributed to elevating risk. While most measured conditions pushed the assessment toward Fail, the specific part being produced (CN7 W/S SIDE MLD'G LH) slightly reduced the assessed risk. The combination of these factors shaped the model's overall risk evaluation, though they do not confirm the physical cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 116

| feature_name           |   feature_attribution |   absolute_attribution | direction   |
|:-----------------------|----------------------:|-----------------------:|:------------|
| Mold_Temperature_4     |              1.69009  |               1.69009  | toward Fail |
| Mold_Temperature_3     |              1.14841  |               1.14841  | toward Fail |
| Plasticizing_Position  |              0.83387  |               0.83387  | toward Fail |
| Clamp_Close_Time       |              0.70908  |               0.70908  | toward Fail |
| Cushion_Position       |              0.328658 |               0.328658 | toward Fail |
| Max_Injection_Speed    |              0.279951 |               0.279951 | toward Fail |
| Injection_Time         |              0.251903 |               0.251903 | toward Fail |
| Average_Screw_RPM      |              0.190411 |               0.190411 | toward Fail |
| Max_Injection_Pressure |              0.179815 |               0.179815 | toward Fail |
| Barrel_Temperature_4   |             -0.089785 |               0.089785 | toward Pass |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 116

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was driven mainly by higher readings in two mold temperature zones, which pushed strongly toward Fail. Plasticizing position, clamp close time, and cushion position also added to the failure-risk view, with the injection profile contributing further through higher peak speed, longer injection time, and higher peak pressure. Average screw RPM had a smaller but still Fail-leaning influence. The only notable counterweight was the temperature in the fourth barrel heating zone, which reduced the model’s failure-risk assessment slightly. These signals describe how the cycle looked to the model and do not prove the physical cause of the defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 116

**Reason:** 미성형 => Unshaped

The model's assessment of failure risk for this cycle was primarily driven higher by conditions in the mold and injection process. Specifically, the temperatures in two monitored mold zones, the screw position reached during plasticizing, the mold clamp close time, and the cushion position all contributed to an increased failure-risk outlook. Conversely, the temperature recorded in the fourth heating zone of the injection barrel provided evidence that slightly counteracted this risk. Please note that these factors represent the model's internal assessment of this specific cycle and do not confirm the physical root cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 116

**Reason:** 미성형 => Unshaped

Higher temperatures in two monitored mold zones (Mold_Temperature_4 and Mold_Temperature_3) most strongly increased the model's failure-risk assessment for this cycle. The plasticizing screw position, longer clamp close time, and smaller cushion position further elevated the risk. Faster injection speeds, longer injection time, and higher screw RPM also contributed to the elevated assessment. However, the temperature in the fourth barrel heating zone slightly reduced the failure-risk assessment. These conditions combined to shape the model's overall risk evaluation, though they do not confirm the physical cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 1347

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| Barrel_Temperature_1            |              0.558777 |               0.558777 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.555446 |               0.555446 | toward Fail |
| Mold_Temperature_3              |             -0.343076 |               0.343076 | toward Pass |
| Hopper_Temperature              |             -0.298938 |               0.298938 | toward Pass |
| Barrel_Temperature_5            |              0.257078 |               0.257078 | toward Fail |
| Max_Screw_RPM                   |             -0.208215 |               0.208215 | toward Pass |
| Mold_Temperature_4              |             -0.205128 |               0.205128 | toward Pass |
| Barrel_Temperature_4            |              0.161324 |               0.161324 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.147986 |               0.147986 | toward Fail |
| Plasticizing_Time               |              0.136601 |               0.136601 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 1347

**Reason:** 가스 => Gas

The model’s failure-risk assessment was pushed mainly by the first barrel heating zone temperature and the product being made in the RG3 MOLD'G W/SHLD, RH configuration, with additional failure-risk influence from the fifth barrel zone temperature. Offsetting that, the mold temperature in one monitored zone and the hopper temperature both pulled the assessment toward Pass. Smaller counteracting support also came from the maximum screw speed and another mold temperature zone, while the fourth barrel zone, the LH part variant, and plasticizing time added some further push toward Fail. These factors describe how the model judged this cycle’s risk; they do not prove the actual physical cause of any defect or show that any setting was out of range.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 1347

**Reason:** 가스 => Gas

The assessment of failure risk for this cycle was primarily driven upward by the temperature in the first heating zone of the injection barrel and the specific product part type being manufactured. Additionally, the temperature in the fifth zone of the injection barrel contributed to a higher failure-risk assessment. Conversely, the model’s risk assessment was reduced by measurements from the mold temperature zone three and the hopper temperature, which acted to counteract the risk factors. These observations reflect how the model weighed specific process conditions for this production cycle.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 1347

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the high temperature in the first heating zone of the injection barrel and the specific part type being produced ('RG3 MOLD'G W/SHLD, RH'), both of which increased the perceived risk of failure. Additionally, the temperature in the fifth heating zone of the barrel contributed to this assessment. However, the mold temperature in one monitored zone and the hopper temperature counteracted this risk, reducing the model's failure-risk assessment. The maximum screw RPM during plasticizing also played a role in lowering the perceived risk.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 1415

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.565848 |               0.565848 | toward Fail |
| Barrel_Temperature_1            |              0.502482 |               0.502482 | toward Fail |
| Hopper_Temperature              |             -0.317344 |               0.317344 | toward Pass |
| Barrel_Temperature_4            |              0.287112 |               0.287112 | toward Fail |
| Plasticizing_Time               |             -0.186013 |               0.186013 | toward Pass |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.154775 |               0.154775 | toward Fail |
| Filling_Time                    |              0.128    |               0.128    | toward Fail |
| Mold_Temperature_4              |             -0.113954 |               0.113954 | toward Pass |
| Clamp_Open_Position             |              0.111136 |               0.111136 | toward Fail |
| Barrel_Temperature_3            |              0.10775  |               0.10775  | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 1415

**Reason:** 가스 => Gas

The model’s failure-risk assessment was driven most strongly by the specific part being run for this cycle and by higher readings in the first and fourth barrel heating zones, which both pushed the assessment toward Fail. The left-hand RG3 molded-with-shield part designation, along with filling time and clamp open position, also added smaller amounts of pressure toward Fail. Counteracting that, hopper temperature and plasticizing time pushed the assessment toward Pass, reducing some of the failure risk. Mold temperature in one monitored zone also supported Pass. Overall, the cycle mixed several signals, but the strongest ones leaned toward a higher chance of failure in the model’s view.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 1415

**Reason:** 가스 => Gas

The model's assessment of failure risk for this production cycle was primarily increased by the specific part being manufactured (RG3 Mold'g w/Shld, RH) and elevated temperatures in the first and fourth heating zones of the injection barrel. These factors collectively push the result toward a failure classification. Conversely, the temperature recorded at the hopper and the duration of the plasticizing time acted to counteract this assessment, reducing the predicted failure risk. While these variables shaped the model's output, they do not confirm the physical cause of any potential defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 1415

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH' and higher temperatures in the first and fourth barrel heating zones, which increased the perceived risk. The hopper temperature and plasticizing time counteracted this risk, reducing the model's failure assessment. Additional factors like the part type 'RG3 MOLD'G W/SHLD, LH', longer filling time, and mold opening position also contributed to the elevated risk, though to a lesser extent. While mold temperature in another zone further reduced the risk, the overall assessment was driven primarily by the part type and barrel temperatures. This evidence reflects how the model interpreted these conditions, not the actual cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 1515

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.598494 |               0.598494 | toward Fail |
| Barrel_Temperature_1            |              0.517301 |               0.517301 | toward Fail |
| Barrel_Temperature_4            |              0.199151 |               0.199151 | toward Fail |
| Hopper_Temperature              |              0.179079 |               0.179079 | toward Fail |
| Plasticizing_Time               |              0.173169 |               0.173169 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.161207 |               0.161207 | toward Fail |
| Cushion_Position                |              0.134428 |               0.134428 | toward Fail |
| Injection_Time                  |              0.127667 |               0.127667 | toward Fail |
| Filling_Time                    |              0.12257  |               0.12257  | toward Fail |
| Max_Injection_Speed             |              0.116265 |               0.116265 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 1515

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was driven mainly by the part being run, along with the first and fourth barrel heating zones, hopper temperature, and plasticizing time, all of which pushed the cycle toward a Fail outcome. Additional process timing and filling behavior, including cushion position, injection time, filling time, and maximum injection speed, also added to the same fail-leaning assessment. The second part category for the left-hand version of the same part also reinforced that direction. No strong countervailing evidence toward Pass appears in the provided factors, so the overall assessment was tilted toward failure risk by several process and product-related signals.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 1515

**Reason:** 미성형 => Unshaped

For this production cycle, the model’s assessment of failure risk was primarily driven by the specific part type, RG3 MOLD'G W/SHLD, RH, and elevated temperature readings in the first zone of the injection barrel. Additional factors contributing to an increased risk assessment included the temperatures in the fourth barrel zone and the hopper, as well as the duration of the plasticizing cycle. There were no variables identified in this cycle that acted to counteract or reduce the model's failure-risk assessment. These process conditions explain the model's output for this cycle but do not confirm a physical root cause for the outcome.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 1515

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which increased the perceived risk. Higher temperatures in the first and fourth barrel heating zones further elevated the risk, along with elevated hopper temperature and longer plasticizing time. These conditions collectively suggested a higher likelihood of failure. However, no strong counteracting factors were present to reduce the risk assessment. The evidence reflects how these process variables aligned with patterns the model associates with increased failure risk, without confirming a physical defect cause.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 1621

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.587329 |               0.587329 | toward Fail |
| Barrel_Temperature_1            |              0.55015  |               0.55015  | toward Fail |
| Hopper_Temperature              |              0.202673 |               0.202673 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.161081 |               0.161081 | toward Fail |
| Barrel_Temperature_4            |              0.144202 |               0.144202 | toward Fail |
| Injection_Time                  |              0.140595 |               0.140595 | toward Fail |
| Barrel_Temperature_2            |              0.139368 |               0.139368 | toward Fail |
| Barrel_Temperature_5            |             -0.137791 |               0.137791 | toward Pass |
| Clamp_Open_Position             |              0.119291 |               0.119291 | toward Fail |
| Filling_Time                    |              0.115998 |               0.115998 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 1621

**Reason:** 가스 => Gas

The failure-risk assessment was driven mainly by the part being run for this cycle, especially the RG3 MOLD'G W/SHLD, RH and RG3 MOLD'G W/SHLD, LH categories, which both pushed the result toward Fail. Heating-related conditions also increased the failure-risk assessment, led by the first barrel temperature, with additional support from hopper temperature and the barrel temperatures in zones 2 and 4. Injection and mold-cycle timing, including injection time, filling time, and clamp open position, also pushed the model toward Fail. The main evidence working in the opposite direction was the fifth barrel temperature, which reduced the failure-risk assessment and partially offset the Fail-leaning signals. Overall, the model saw this cycle as more failure-prone, but this does not prove these conditions physically caused the defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 1621

**Reason:** 가스 => Gas

The model’s assessment of failure risk for this production cycle was primarily driven upward by the specific part type being manufactured, identified as the right-hand molded shield, and elevated temperatures in the first heating zone of the injection barrel. Additional factors increasing the risk assessment included the hopper temperature, the production of the left-hand molded shield, and temperatures in the fourth heating zone of the injection barrel. These process conditions collectively pushed the model toward a higher failure-risk designation. Conversely, the temperature recorded in the fifth heating zone of the injection barrel served to counteract this trend and reduced the model's failure-risk assessment. Please note that this analysis reflects how the model interpreted these process variables and does not confirm the definitive physical cause of the production outcome.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 1621

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH' and high barrel temperature in the first heating zone, both increasing the risk of failure. Elevated hopper temperature and the part type 'RG3 MOLD'G W/SHLD, LH' also contributed to higher failure risk, along with barrel temperature in the fourth heating zone. However, the temperature in the fifth heating zone of the barrel helped reduce the assessed failure risk. Other factors like injection time, barrel temperature in the second heating zone, clamp open position, and filling time had smaller effects increasing failure risk. The evidence reflects how these conditions collectively shaped the model's risk evaluation, without confirming physical causes.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 1937

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| Barrel_Temperature_1            |              0.582936 |               0.582936 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.54541  |               0.54541  | toward Fail |
| Mold_Temperature_3              |             -0.330759 |               0.330759 | toward Pass |
| Mold_Temperature_4              |             -0.310983 |               0.310983 | toward Pass |
| Hopper_Temperature              |              0.231754 |               0.231754 | toward Fail |
| Barrel_Temperature_5            |             -0.206709 |               0.206709 | toward Pass |
| Barrel_Temperature_2            |              0.187179 |               0.187179 | toward Fail |
| Barrel_Temperature_4            |              0.168281 |               0.168281 | toward Fail |
| Cycle_Time                      |              0.162492 |               0.162492 | toward Fail |
| Injection_Time                  |              0.147448 |               0.147448 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 1937

**Reason:** 가스 => Gas

The model’s failure-risk assessment was pushed up most strongly by the first barrel heating zone, the selected part type for this cycle, and the hopper temperature, with additional fail-leaning influence from the second and fourth barrel heating zones as well as cycle time and injection time. These factors made the cycle look more like a Fail to the model. Counteracting that, the temperatures in two mold zones and the fifth barrel heating zone pulled the assessment back toward Pass. Overall, the evidence shows a mix of opposing process signals, but it does not establish the physical cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 1937

**Reason:** 가스 => Gas

The temperature in the first heating zone of the injection barrel and the specific product part type (RG3 MOLD'G W/SHLD, RH) had the strongest influence in increasing the model's failure-risk assessment for this cycle. The temperature at the hopper also contributed factors that pushed the assessment toward a fail. Conversely, temperatures in the third and fourth mold zones, as well as the fifth barrel heating zone, provided evidence that counteracted these risks and pushed the assessment toward a pass. Note that these observations reflect the model’s interpretation of this cycle’s process data and do not confirm these variables as the physical cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 1937

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the high temperature in the first heating zone of the injection barrel and the specific part being produced ('RG3 MOLD'G W/SHLD, RH'), both of which increased the perceived risk. Counteracting this were the temperatures in two monitored zones of the mold, which reduced the failure-risk assessment. Additional factors like the hopper temperature, cycle time, and injection time also contributed to the elevated risk, though to a lesser extent. The evidence suggests these conditions collectively shaped the model's output but does not confirm they caused the defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 2021

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| Barrel_Temperature_1            |              0.560474 |               0.560474 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.537925 |               0.537925 | toward Fail |
| Barrel_Temperature_3            |             -0.293756 |               0.293756 | toward Pass |
| Barrel_Temperature_5            |              0.194597 |               0.194597 | toward Fail |
| Hopper_Temperature              |              0.17511  |               0.17511  | toward Fail |
| Barrel_Temperature_2            |              0.158506 |               0.158506 | toward Fail |
| Barrel_Temperature_4            |              0.145788 |               0.145788 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.132484 |               0.132484 | toward Fail |
| Mold_Temperature_4              |             -0.129914 |               0.129914 | toward Pass |
| Injection_Time                  |              0.128408 |               0.128408 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2021

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was pushed up mainly by the first barrel heating zone, the specific part being run, the fifth barrel zone, the hopper temperature, and the second and fourth barrel zones, all of which leaned toward Fail. The product type for this cycle also added to the failure-risk view, indicating the model associated this part family with a less favorable outcome in this instance. Against that, the third barrel zone and one monitored mold temperature pulled the assessment toward Pass, partly offsetting the fail-leaning evidence. Injection time also added some failure-risk pressure, though it was weaker than the temperature-related signals. These factors explain the model’s judgment for this cycle, but they do not establish the physical root cause of the recorded defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2021

**Reason:** 미성형 => Unshaped

The model’s assessment of failure risk for this production cycle was primarily increased by the temperature in the first heating zone of the injection barrel and the specific product type being manufactured. Additional factors contributing to a higher failure-risk assessment included the temperatures in the fifth heating zone and the hopper, as well as the injection time. Conversely, the temperature in the third heating zone helped counteract these pressures by pushing the assessment toward a pass. Please note that these factors reflect how the model processed the cycle data and do not confirm the physical root cause of a defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2021

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly influenced by the first heating zone temperature and the part type 'RG3 MOLD'G W/SHLD, RH', both increasing the risk of failure. The third heating zone temperature counteracted this risk by reducing the failure assessment. Additional factors like the fifth heating zone temperature, hopper temperature, and second heating zone temperature further contributed to the elevated risk, while the fourth mold temperature zone helped lower it. The combination of these conditions, particularly the high influence of the first heating zone and part type, shaped the overall risk profile without confirming a physical defect cause.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 2105

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.569506 |               0.569506 | toward Fail |
| Barrel_Temperature_1            |              0.491898 |               0.491898 | toward Fail |
| Barrel_Temperature_5            |              0.380728 |               0.380728 | toward Fail |
| Hopper_Temperature              |              0.266253 |               0.266253 | toward Fail |
| Max_Screw_RPM                   |              0.169619 |               0.169619 | toward Fail |
| Plasticizing_Time               |              0.167731 |               0.167731 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.163151 |               0.163151 | toward Fail |
| Barrel_Temperature_2            |              0.158704 |               0.158704 | toward Fail |
| Injection_Time                  |              0.135133 |               0.135133 | toward Fail |
| Barrel_Temperature_6            |              0.133569 |               0.133569 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2105

**Reason:** 가스 => Gas

The model’s failure-risk assessment was driven mainly by the part being made, along with the temperature profile in the injection barrel and hopper, which together pushed the cycle toward Fail. The strongest contributors were the RG3 MOLD'G W/SHLD, RH part category, followed by the first and fifth barrel temperature zones, then the hopper temperature and the maximum screw speed, all increasing the model’s concern about failure. Plasticizing time and injection time also added additional, smaller pressure toward Fail, and the RG3 MOLD'G W/SHLD, LH part category reinforced that pattern. No strong evidence in this cycle pushed the assessment toward Pass, so the overall balance favored a Fail outcome.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2105

**Reason:** 가스 => Gas

The model’s assessment of failure risk for this cycle was influenced primarily by the production of the RH shield mold product. Additionally, elevated temperature readings in the first and fifth barrel zones, as well as the hopper temperature, increased the overall failure-risk assessment. The maximum screw rotation speed during plasticizing also contributed to this higher risk outlook. No process variables were identified that reduced the model’s assessment of failure risk for this specific cycle. Note that these indicators identify patterns in the data and do not confirm the physical root cause of a defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2105

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which increased the perceived risk. Higher temperatures in the first and fifth barrel heating zones further elevated the risk, along with elevated hopper temperature and maximum screw RPM. The plasticizing time also contributed to the model's higher risk assessment. While no strong evidence counteracted these factors, the combined effect of these conditions led the model to flag this cycle as higher risk.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 2163

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              0.553779 |               0.553779 | toward Fail |
| Barrel_Temperature_1            |              0.539913 |               0.539913 | toward Fail |
| Hopper_Temperature              |              0.271211 |               0.271211 | toward Fail |
| Clamp_Close_Time                |             -0.164106 |               0.164106 | toward Pass |
| Max_Screw_RPM                   |              0.164078 |               0.164078 | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |              0.148409 |               0.148409 | toward Fail |
| Injection_Time                  |              0.136161 |               0.136161 | toward Fail |
| Barrel_Temperature_2            |              0.11859  |               0.11859  | toward Fail |
| Max_Injection_Speed             |              0.10172  |               0.10172  | toward Fail |
| Filling_Time                    |              0.100814 |               0.100814 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was driven mainly by the product type for this cycle and by process conditions around the barrel and hopper, with the RG3 MOLD'G W/SHLD, RH part category, the first barrel heating zone, and hopper temperature all pushing the assessment toward Fail. Additional process evidence also nudged the result toward Fail from the maximum screw speed, the left-hand part category, injection time, the second barrel heating zone, maximum injection speed, and filling time. One factor, clamp close time, pushed in the opposite direction and reduced the model’s failure-risk assessment. These signals describe how the model weighed the cycle, but they do not prove that any one condition physically caused the recorded defect or that any value was outside an acceptable range.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The production of the RG3 mold with shield (RH) most significantly increased the model’s assessment of failure risk for this cycle. Elevated temperature settings in the first heating zone of the injection barrel and the hopper, along with higher maximum screw rotation speeds, further contributed to this assessment. Conversely, the time taken for the mold clamp to close acted to reduce the model's failure-risk assessment. Please note that these factors reflect the model's behavior and do not confirm the physical cause of any production issues.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH' and high barrel temperature in the first heating zone, both increasing the risk of failure. Elevated hopper temperature and maximum screw RPM further contributed to the higher risk assessment, while the clamp close time acted to reduce the perceived risk. Other factors like injection time and barrel temperature in the second heating zone also played a smaller role in raising the failure risk. The evidence suggests these conditions collectively shaped the model's output, though it does not confirm they physically caused the defect. The part type 'RG3 MOLD'G W/SHLD, LH' had a lesser but still notable impact on increasing failure risk.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
