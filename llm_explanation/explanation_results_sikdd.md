

## Top 10 SHAP Features for Index Row 2163

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              2.13913  |               2.13913  | toward Fail |
| Max_Injection_Pressure          |              0.8178   |               0.8178   | toward Fail |
| Plasticizing_Time               |             -0.799277 |               0.799277 | toward Pass |
| Mold_Temperature_4              |             -0.690494 |               0.690494 | toward Pass |
| Max_Screw_RPM                   |              0.596022 |               0.596022 | toward Fail |
| Barrel_Temperature_2            |              0.551511 |               0.551511 | toward Fail |
| Hopper_Temperature              |              0.452056 |               0.452056 | toward Fail |
| Barrel_Temperature_4            |             -0.425832 |               0.425832 | toward Pass |
| Barrel_Temperature_6            |              0.397235 |               0.397235 | toward Fail |
| Average_Back_Pressure           |             -0.378299 |               0.378299 | toward Pass |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was driven most strongly by the product type, which pushed the cycle toward Fail more than any other factor. Higher maximum injection pressure, maximum screw speed, barrel temperature in heating zones 2 and 6, and hopper temperature also increased the model’s expectation of failure. Offsetting that, longer plasticizing time and lower mold temperature in zone 4 reduced the failure-risk assessment, along with lower barrel temperature in zone 4 and lower average back pressure. Overall, the cycle had a mix of conditions leaning both ways, but the Fail-leaning evidence was stronger. These process signals explain the model’s decision for this cycle and do not prove the physical cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The production of the RG3 MOLD'G W/SHLD, RH part type significantly increased the failure-risk assessment for this cycle. Higher maximum injection pressure and an elevated maximum screw rotation speed also contributed to a higher projected failure risk. Conversely, the plasticizing time and the temperature in the fourth mold zone helped counteract the failure risk assessment. These observations reflect how the model weighed specific cycle data but do not confirm a physical root cause for any quality concerns.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which increased the risk, followed by high injection pressure and maximum screw RPM, both of which further raised the risk. However, the longer plasticizing time and mold temperature in zone 4 helped reduce the assessed risk. Barrel temperatures in zones 2 and 6, along with hopper temperature, also contributed to increasing the risk, while barrel temperature in zone 4 and average back pressure counteracted it. These conditions collectively shaped the model's assessment, though they do not confirm the physical cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 2177

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              2.24777  |               2.24777  | toward Fail |
| Barrel_Temperature_5            |              1.35305  |               1.35305  | toward Fail |
| Max_Screw_RPM                   |              0.511997 |               0.511997 | toward Fail |
| Average_Back_Pressure           |             -0.499829 |               0.499829 | toward Pass |
| Barrel_Temperature_1            |             -0.396617 |               0.396617 | toward Pass |
| Clamp_Close_Time                |             -0.366042 |               0.366042 | toward Pass |
| Max_Injection_Pressure          |              0.296481 |               0.296481 | toward Fail |
| Hopper_Temperature              |              0.282539 |               0.282539 | toward Fail |
| Mold_Temperature_4              |             -0.270166 |               0.270166 | toward Pass |
| Barrel_Temperature_3            |              0.25345  |               0.25345  | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2177

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was pushed most strongly toward Fail by the product type for this cycle, along with higher temperature in barrel zone 5 and a higher maximum screw speed during plasticizing. Additional Fail-leaning influence came from the maximum injection pressure, hopper temperature, and barrel zone 3 temperature. Offsetting that, the average back pressure, barrel zone 1 temperature, clamp close time, and a monitored mold temperature all pushed the assessment toward Pass and reduced the overall failure risk. These factors describe how the model weighed the cycle, but they do not prove any physical root cause or show that any setting was outside an acceptable process range.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2177

**Reason:** 미성형 => Unshaped

The model's assessment of failure risk for this production cycle was primarily increased by the specific part type being manufactured, the temperature in the fifth zone of the injection barrel, and the maximum screw rotation speed. Higher injection pressure and elevated hopper temperatures also contributed to this increased risk assessment. Conversely, the average back pressure during material preparation, the temperature in the first heating zone of the barrel, and the clamp closing time acted to reduce the model's failure-risk assessment. These factors reflect the model’s internal evaluation and do not confirm the physical root cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2177

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which increased the risk, followed by the high temperature in the fifth barrel heating zone. The maximum screw RPM also contributed to higher risk, while the average back pressure and first barrel temperature helped reduce it. Other factors like injection pressure and hopper temperature slightly raised the risk, but clamp close time and mold temperature in zone 4 counteracted some of that risk. The combination of these conditions shaped the model's overall assessment without confirming a physical defect cause.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 4726

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| Average_Screw_RPM               |             -0.736716 |               0.736716 | toward Pass |
| PART_NAME_RG3 MOLD'G W/SHLD, RH |             -0.622412 |               0.622412 | toward Pass |
| Clamp_Close_Time                |             -0.612787 |               0.612787 | toward Pass |
| Hopper_Temperature              |              0.538462 |               0.538462 | toward Fail |
| Max_Injection_Pressure          |             -0.463647 |               0.463647 | toward Pass |
| Mold_Temperature_3              |             -0.39628  |               0.39628  | toward Pass |
| Mold_Temperature_4              |             -0.363806 |               0.363806 | toward Pass |
| Max_Screw_RPM                   |             -0.339795 |               0.339795 | toward Pass |
| Injection_Time                  |              0.272046 |               0.272046 | toward Fail |
| Barrel_Temperature_1            |              0.240349 |               0.240349 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 4726

**Reason:** 미성형 => Unshaped

The model saw several conditions as lowering the failure-risk assessment, especially the average screw rotation speed, the part type for this cycle, and the mold clamp closing time, with additional support from the maximum injection pressure and mold temperatures. The main conditions pushing the other way were the hopper temperature, which increased the failure-risk assessment, along with longer injection time and the first barrel heating zone temperature. Overall, the pass-leaning evidence was stronger than the fail-leaning evidence, so the cycle was assessed as more consistent with Pass than Fail. This describes how the process signals affected the model’s judgment, not the physical root cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 4726

**Reason:** 미성형 => Unshaped

The temperature around the material hopper increased the model's assessment of failure risk for this production cycle. Conversely, the specific screw rotation speed, the product part identity, and the mold clamp closing time acted as the strongest factors pushing the assessment toward a successful outcome. Additionally, the maximum injection pressure helped counteract the failure-risk assessment. These influences describe the model's interpretation of the data and do not confirm the physical cause of any production outcome.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 4726

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment was most strongly reduced by the average screw rotation speed during material preparation, the specific part being manufactured ('RG3 MOLD'G W/SHLD, RH'), and the clamp close time, all of which pushed the assessment toward Pass. However, the hopper temperature increased the failure-risk assessment more than any other single factor. The injection time and the temperature in the first heating zone of the barrel also contributed to increasing the failure-risk assessment, though to a lesser extent. Overall, the conditions pushing toward Pass outweighed those increasing failure risk, shaping the model's final assessment for this cycle.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5183

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              2.18961  |               2.18961  | toward Fail |
| Max_Back_Pressure               |              1.35706  |               1.35706  | toward Fail |
| Average_Back_Pressure           |              1.01159  |               1.01159  | toward Fail |
| Max_Injection_Pressure          |              0.685946 |               0.685946 | toward Fail |
| Hopper_Temperature              |              0.494269 |               0.494269 | toward Fail |
| Barrel_Temperature_6            |              0.487087 |               0.487087 | toward Fail |
| Max_Screw_RPM                   |              0.477147 |               0.477147 | toward Fail |
| Plasticizing_Time               |              0.46788  |               0.46788  | toward Fail |
| Cycle_Time                      |              0.392393 |               0.392393 | toward Fail |
| Clamp_Close_Time                |             -0.279484 |               0.279484 | toward Pass |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5183

**Reason:** 가스 => Gas

The model leaned toward Fail mainly because the part being run, RG3 MOLD'G W/SHLD, RH, was associated with a higher failure-risk assessment for this cycle. Higher back pressure, both the maximum and the average during plasticizing, also pushed the assessment toward Fail, with additional support from higher maximum injection pressure. Hopper temperature, barrel temperature in zone 6, screw speed, plasticizing time, and overall cycle time each added smaller amounts of failure-risk. The main offsetting evidence was clamp close time, which pushed the assessment toward Pass and partially reduced the overall failure-risk view.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5183

**Reason:** 가스 => Gas

The model’s assessment of increased failure risk for this production cycle was primarily driven by the specific part type, RG3 MOLD'G W/SHLD, RH. Additionally, high readings for maximum and average back pressure, maximum injection pressure, and hopper temperature further increased the risk profile during this run. While these factors contributed to the failure-risk assessment, the clamp close time served to counteract this trend and reduced the overall assessment. These observations reflect how the model processed these variables and do not confirm that these conditions physically caused a defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5183

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which increased the risk of failure. High back pressure, both maximum and average, further elevated the failure-risk assessment, along with elevated maximum injection pressure and hopper temperature. The sixth barrel temperature zone, maximum screw RPM, plasticizing time, and cycle time also contributed to increasing the model's failure-risk assessment. However, a faster clamp close time helped reduce the model's failure-risk assessment for this cycle. These conditions collectively shaped the model's evaluation, though they do not confirm the physical cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5185

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |              2.14701  |               2.14701  | toward Fail |
| Max_Back_Pressure               |              1.30035  |               1.30035  | toward Fail |
| Max_Injection_Pressure          |              1.08043  |               1.08043  | toward Fail |
| Average_Back_Pressure           |              0.918646 |               0.918646 | toward Fail |
| Clamp_Close_Time                |             -0.617266 |               0.617266 | toward Pass |
| Barrel_Temperature_2            |              0.497433 |               0.497433 | toward Fail |
| Mold_Temperature_4              |             -0.438651 |               0.438651 | toward Pass |
| Hopper_Temperature              |              0.417874 |               0.417874 | toward Fail |
| Barrel_Temperature_4            |             -0.409705 |               0.409705 | toward Pass |
| Cycle_Time                      |              0.382443 |               0.382443 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5185

**Reason:** 가스 => Gas

The model’s failure-risk assessment was driven mainly by the part type for this cycle, which strongly pushed the decision toward Fail. Higher maximum back pressure, higher maximum injection pressure, and higher average back pressure also increased the model’s concern about failure, indicating the pressure profile was an important contributor to the risk assessment. In addition, barrel zone 2 temperature, hopper temperature, and cycle time each added smaller amounts of Fail-leaning evidence. Counteracting this, the clamp close time reduced the failure-risk assessment, and mold temperature zone 4 and barrel temperature zone 4 also pushed the model toward Pass.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5185

**Reason:** 가스 => Gas

The model’s assessment of higher failure risk for this production cycle was primarily influenced by the specific part type, RG3 MOLD'G W/SHLD, RH. Additionally, elevated readings for maximum back pressure, maximum injection pressure, and average back pressure further increased the failure-risk assessment. Conversely, the time taken for the mold clamp to close acted to counteract these factors and reduced the model's failure-risk assessment. Please note that this analysis reflects internal model logic and does not identify the definitive physical cause of the defect or indicate that any individual measurement fell outside of operational specifications.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5185

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which increased the risk. High back pressure, high injection pressure, and above-average back pressure during material preparation further elevated the risk. However, a faster clamp close time and lower temperatures in mold zone 4 and barrel zone 4 reduced the assessed risk. While these conditions shaped the model's output, they do not confirm the physical cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5188

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| Average_Back_Pressure           |              1.50851  |               1.50851  | toward Fail |
| PART_NAME_RG3 MOLD'G W/SHLD, RH |             -1.23971  |               1.23971  | toward Pass |
| Max_Injection_Pressure          |              1.19555  |               1.19555  | toward Fail |
| Max_Back_Pressure               |              1.16629  |               1.16629  | toward Fail |
| Hopper_Temperature              |              0.590555 |               0.590555 | toward Fail |
| Mold_Temperature_4              |             -0.533641 |               0.533641 | toward Pass |
| Plasticizing_Time               |              0.454321 |               0.454321 | toward Fail |
| Average_Screw_RPM               |             -0.441036 |               0.441036 | toward Pass |
| Clamp_Close_Time                |             -0.397    |               0.397    | toward Pass |
| Max_Screw_RPM                   |              0.389777 |               0.389777 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5188

**Reason:** 미성형 => Unshaped

The model’s failure-risk assessment was driven mainly by higher average back pressure, higher maximum injection pressure, and higher maximum back pressure, all of which pushed the cycle toward Fail. Higher hopper temperature, longer plasticizing time, and a higher maximum screw speed also added to the failure-risk view. Offsetting that, the part type for this cycle and the mold temperature in one monitored zone pushed the assessment toward Pass. Lower average screw speed and a shorter clamp-close time also reduced the model’s concern about failure. Overall, the cycle had several strong pressure-related signals increasing failure risk, balanced by a smaller set of factors pointing toward Pass.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5188

**Reason:** 미성형 => Unshaped

The average resistance pressure during material preparation, the maximum injection pressure, and the maximum resistance pressure during screw recovery were the primary factors increasing the failure-risk assessment for this cycle. Additionally, the hopper temperature contributed to this increased risk. Conversely, the specific part type being manufactured counteracted these factors by pushing the assessment toward a pass. Other mitigating influences included the temperature in the monitored mold zone and the average screw rotation speed.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5188

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly influenced by higher-than-typical average back pressure, maximum injection pressure, and maximum back pressure, all of which increased the perceived risk. The specific part being produced ('RG3 MOLD'G W/SHLD, RH') notably reduced the risk assessment, as did stable mold temperature in one zone and consistent clamp closure timing. While hopper temperature, plasticizing time, and maximum screw RPM also contributed to the risk assessment, their impact was less significant. The combination of these factors shaped the model's output, though they do not confirm the physical cause of any defect. Process conditions appeared generally controlled, with no single measurement standing out as extreme.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5190

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |             -1.71132  |               1.71132  | toward Pass |
| Average_Back_Pressure           |              1.4507   |               1.4507   | toward Fail |
| Max_Back_Pressure               |              1.15538  |               1.15538  | toward Fail |
| Max_Injection_Pressure          |              0.748531 |               0.748531 | toward Fail |
| Hopper_Temperature              |              0.529087 |               0.529087 | toward Fail |
| Plasticizing_Time               |              0.474033 |               0.474033 | toward Fail |
| Clamp_Close_Time                |             -0.453913 |               0.453913 | toward Pass |
| Mold_Temperature_4              |             -0.451478 |               0.451478 | toward Pass |
| Barrel_Temperature_2            |              0.439037 |               0.439037 | toward Fail |
| Max_Screw_RPM                   |              0.381787 |               0.381787 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5190

**Reason:** 미성형 => Unshaped

The model’s assessment was pulled most toward Pass by the product part type for this cycle, which strongly reduced the failure-risk estimate. Against that, higher average back pressure and higher peak back pressure were the strongest process signals pushing the assessment toward Fail, indicating a higher perceived risk during material preparation. Higher peak injection pressure and hopper temperature also increased the failure-risk assessment, with plasticizing time, barrel temperature in zone 2, and maximum screw speed adding smaller Fail-leaning influence. Some conditions counteracted that risk: clamp close time and one monitored mold temperature pushed the assessment toward Pass.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5190

**Reason:** 미성형 => Unshaped

The model's assessment for this production cycle was influenced most strongly by the specific part type being manufactured, which acted to reduce the failure-risk assessment. Conversely, higher readings for average and maximum back pressure, maximum injection pressure, hopper temperature, and plasticizing time all worked to increase the failure-risk assessment. Other conditions, such as the clamp closing time and mold temperature readings, provided additional counteracting influence that reduced the risk assessment. These observations reflect the influence of monitoring data on the current model output and do not represent a definitive finding of a physical defect or root cause for the cycle.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5190

**Reason:** 미성형 => Unshaped

The model's failure-risk assessment for this cycle was most strongly reduced by the part type being 'RG3 MOLD'G W/SHLD, RH', which pushed the outcome toward Pass. However, this was countered by higher-than-typical average and maximum back pressure, as well as elevated maximum injection pressure, all of which increased the assessed risk of failure. Additional factors like hopper temperature and plasticizing time further contributed to the failure-risk assessment, though to a lesser extent. On the other hand, a faster clamp close time and mold temperature in one zone helped reduce the perceived risk. The combination of these conditions shaped the model's overall risk evaluation for this cycle.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5192

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |             -1.67014  |               1.67014  | toward Pass |
| Average_Back_Pressure           |              1.49367  |               1.49367  | toward Fail |
| Max_Back_Pressure               |              1.10799  |               1.10799  | toward Fail |
| Max_Injection_Pressure          |              0.863074 |               0.863074 | toward Fail |
| Hopper_Temperature              |              0.51082  |               0.51082  | toward Fail |
| Mold_Temperature_4              |             -0.499888 |               0.499888 | toward Pass |
| Plasticizing_Time               |              0.47387  |               0.47387  | toward Fail |
| Barrel_Temperature_6            |              0.445111 |               0.445111 | toward Fail |
| Average_Screw_RPM               |             -0.36964  |               0.36964  | toward Pass |
| Max_Screw_RPM                   |              0.339193 |               0.339193 | toward Fail |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5192

**Reason:** 가스 => Gas

The model’s failure-risk assessment was pushed up most by higher average back pressure, higher maximum back pressure, and higher maximum injection pressure, with additional upward pressure from hopper temperature, plasticizing time, barrel temperature zone 6, and maximum screw speed. These conditions made the cycle look more likely to fail than pass in the model’s view. Offsetting that, the part type for “RG3 MOLD'G W/SHLD, RH” and the mold temperature at zone 4 both pulled the assessment toward Pass. The average screw speed also reduced the failure-risk assessment. This indicates which process conditions most influenced the model’s decision for this cycle, not the physical root cause of the defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5192

**Reason:** 가스 => Gas

The production cycle for the RG3 MOLD'G W/SHLD, RH part type had the strongest influence in reducing the failure-risk assessment. Conversely, several pressure-related variables increased the failure-risk assessment, specifically the average and maximum back pressure levels during material preparation, as well as the maximum injection pressure. Elevated hopper temperatures further contributed to the risk assessment. The temperature recorded in the fourth mold zone helped counteract these factors, working to reduce the overall failure-risk assessment for this cycle.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5192

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly reduced by the part type being 'RG3 MOLD'G W/SHLD, RH', which pushed the outcome toward Pass. However, this was countered by elevated average and maximum back pressure, along with high injection pressure, all of which increased the assessed risk of failure. Additional factors like hopper temperature and plasticizing time further contributed to the failure-risk assessment, while mold temperature in zone 4 and average screw RPM helped reduce it. The combination of these conditions shaped the model's overall risk evaluation, though they do not confirm the physical cause of any defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5205

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |             -1.86773  |               1.86773  | toward Pass |
| Max_Back_Pressure               |              1.1584   |               1.1584   | toward Fail |
| Average_Back_Pressure           |              1.06604  |               1.06604  | toward Fail |
| Max_Injection_Pressure          |              0.839625 |               0.839625 | toward Fail |
| Barrel_Temperature_5            |              0.786269 |               0.786269 | toward Fail |
| Barrel_Temperature_6            |              0.606709 |               0.606709 | toward Fail |
| Plasticizing_Time               |              0.56926  |               0.56926  | toward Fail |
| Mold_Temperature_4              |             -0.467079 |               0.467079 | toward Pass |
| Hopper_Temperature              |              0.356431 |               0.356431 | toward Fail |
| Barrel_Temperature_4            |             -0.341338 |               0.341338 | toward Pass |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5205

**Reason:** 가스 => Gas

The model’s assessment was pushed toward Pass most strongly by the product part being run, which weighed against a failure call for this cycle. The strongest process signals pushing toward Fail were higher maximum and average back pressure, along with higher maximum injection pressure, all of which increased the model’s failure-risk assessment. Higher barrel temperature in zones 5 and 6 also contributed toward Fail, and plasticizing time plus hopper temperature added smaller additional pressure in that direction. Offsetting some of that, mold temperature in one monitored zone and barrel temperature in zone 4 pushed the assessment back toward Pass.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5205

**Reason:** 가스 => Gas

The model's assessment for this cycle was strongly influenced toward a Pass classification by the specific part type being manufactured. Conversely, higher values in maximum and average back pressure, maximum injection pressure, and the temperature of the fifth heating zone all acted to increase the assessed failure risk. While the fourth mold temperature zone provided evidence that countered this risk assessment, the collective pressure and heat variables were the primary drivers pushing the model toward a potential Fail outcome. Please note that these observations reflect the model’s internal assessment patterns and do not confirm these variables as the physical root cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5205

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly reduced by the part type being 'RG3 MOLD'G W/SHLD, RH', which pushed the outcome toward Pass. However, high back pressure—both maximum and average—along with elevated maximum injection pressure increased the assessed risk of failure. Additional contributing factors included higher temperatures in the fifth and sixth barrel heating zones. These pressure and temperature conditions collectively raised the model's failure-risk assessment, though the specific part type helped counteract this effect. The evidence does not confirm whether these measurements were outside normal operating ranges or directly caused a defect.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5207

| feature_name                    |   feature_attribution |   absolute_attribution | direction   |
|:--------------------------------|----------------------:|-----------------------:|:------------|
| PART_NAME_RG3 MOLD'G W/SHLD, RH |             -1.21719  |               1.21719  | toward Pass |
| Average_Back_Pressure           |              1.19614  |               1.19614  | toward Fail |
| Max_Back_Pressure               |              1.17841  |               1.17841  | toward Fail |
| Max_Injection_Pressure          |              0.987248 |               0.987248 | toward Fail |
| Mold_Temperature_4              |             -0.591077 |               0.591077 | toward Pass |
| Hopper_Temperature              |              0.539487 |               0.539487 | toward Fail |
| Average_Screw_RPM               |             -0.494038 |               0.494038 | toward Pass |
| Barrel_Temperature_6            |              0.470355 |               0.470355 | toward Fail |
| Barrel_Temperature_4            |             -0.461513 |               0.461513 | toward Pass |
| Barrel_Temperature_1            |             -0.414562 |               0.414562 | toward Pass |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5207

**Reason:** 가스 => Gas

The model’s failure-risk assessment was pushed upward mainly by higher average back pressure, higher maximum back pressure, and higher maximum injection pressure, which were the strongest process signals favoring Fail. Hopper temperature and the sixth barrel heating zone also added some additional pressure toward a Fail assessment. Offsetting that, the part type for this cycle, along with mold temperature in zone 4, average screw speed, and the first and fourth barrel heating zones, all pulled the assessment back toward Pass. Overall, the evidence shows a mixed pattern with several pressure-related conditions increasing the model’s concern while other settings reduced it, but it does not establish the physical root cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5207

**Reason:** 가스 => Gas

The manufacturing of the RG3 mold with shield significantly reduced the model's assessment of failure risk for this cycle. Conversely, higher readings for average and maximum back pressure, as well as the maximum injection pressure, contributed to an increased assessment of failure risk in the production cycle. The measured mold temperature in zone four also helped counteract the risk profile, pushing the assessment toward a pass. These combined technical factors shaped how the model evaluated the cycle, though this interpretation does not determine the physical cause of any defect.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5207

**Reason:** 가스 => Gas

The model's failure-risk assessment for this cycle was most strongly influenced by the part type 'RG3 MOLD'G W/SHLD, RH', which reduced the risk of failure. However, high average and maximum back pressure during material preparation, along with elevated maximum injection pressure, increased the failure-risk assessment. Additionally, higher hopper temperature and barrel temperature in zone 6 contributed to the increased risk. On the other hand, mold temperature in zone 4, along with lower barrel temperatures in zones 1 and 4, and average screw RPM helped counteract the failure risk.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
