

## Top 10 SHAP Features for Index Row 2163

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| Clamp_Close_Time                |             1.56197  |
| Mold_Temperature_4              |             0.633204 |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             0.623496 |
| Average_Screw_RPM               |             0.491415 |
| Average_Back_Pressure           |             0.429887 |
| Hopper_Temperature              |             0.408182 |
| Max_Back_Pressure               |             0.325091 |
| Max_Injection_Pressure          |             0.306197 |
| Barrel_Temperature_5            |             0.2555   |
| Plasticizing_Time               |             0.233488 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The strongest association was with the time taken for the mold clamp to close, suggesting the clamp closing step may have been an important condition in this failed cycle. The monitored mold temperature, the part type being run, and the average screw rotation speed during material preparation also stood out, pointing to part/setup differences and material-prep or heat-related conditions. Back pressure during material preparation and screw recovery, hopper temperature, and injection pressure were also linked to the failure risk. Plasticizing time and one barrel heating zone temperature added further signs that the material preparation and heating conditions may have played a role.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

The time taken for the mold clamp to close had the most significant influence on this production failure. Fluctuations in mold temperature and the specific part being manufactured also appear to be contributing factors. Additionally, settings related to material preparation, including average screw rotation speed, back pressure, and hopper temperature, may have affected process stability. Variations in injection pressure, barrel temperature, and plasticizing time might be further associated with this outcome. Please review these parameters to ensure they align with current process standards.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2163

**Reason:** 미성형 => Unshaped

This failure may be linked to how long the mold clamp took to close before injection, as this was the most strongly associated factor. The temperature in one of the mold zones and the specific part being produced also showed notable associations with the failure risk. Additionally, the average screw speed and back pressure during material preparation, along with the hopper temperature, may have played supporting roles. Other contributing factors could include the highest back pressure, injection pressure, and the temperature in one of the barrel heating zones. The time taken to prepare the plastic material might have further influenced the outcome.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 2177

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| Barrel_Temperature_5            |             1.09033  |
| Barrel_Temperature_3            |             0.954515 |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             0.757566 |
| Average_Screw_RPM               |             0.724447 |
| Plasticizing_Time               |             0.720355 |
| Mold_Temperature_3              |             0.49428  |
| Clamp_Close_Time                |             0.328497 |
| Hopper_Temperature              |             0.259448 |
| Average_Back_Pressure           |             0.25866  |
| Barrel_Temperature_1            |             0.242705 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 2177

**Reason:** 미성형 => Unshaped

This cycle may have failed because the barrel heating in the third and fifth zones was a major factor, which can affect how the plastic melted and flowed. The part type being made also appears to have been linked to higher risk for this run, along with the screw’s average rotation speed and the time needed to plasticize the material. Mold temperature, clamp closing time, hopper temperature, back pressure, and the first barrel heating zone also look like possible contributors.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 2177

**Reason:** 미성형 => Unshaped

The recent production failure may be linked to thermal variations in the fifth and third heating zones of the injection barrel. The specific product part being manufactured and settings related to material preparation, including the average screw rotation speed and total plasticizing time, were also significant contributors. Changes in the temperature of the third mold zone may have further influenced this result. Additionally, variations in clamp closing time, hopper temperature, average back pressure, and the first barrel heating zone should be reviewed as potential factors in this incident.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 2177

**Reason:** 미성형 => Unshaped

This failure may be linked to temperature inconsistencies in the barrel's heating zones, particularly the fifth and third zones, which could affect material melting and flow. The specific part being produced (PART_NAME_RG3 MOLD'G W/SHLD, LH) and the average screw speed during plasticizing also appear closely associated with the issue. Longer plasticizing times might indicate material preparation challenges, while mold temperature in one zone could contribute to cooling or forming problems. Variations in clamp closing time or hopper temperature may further influence process stability. These conditions together suggest potential instability in material processing or mold interaction.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 4726

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| Average_Screw_RPM               |             0.8981   |
| Barrel_Temperature_3            |             0.42395  |
| Plasticizing_Time               |             0.417788 |
| Hopper_Temperature              |             0.236374 |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             0.2245   |
| PART_NAME_CN7 W/S SIDE MLD'G LH |             0.209418 |
| Max_Injection_Pressure          |             0.194514 |
| Max_Injection_Speed             |             0.183316 |
| Barrel_Temperature_4            |             0.178109 |
| Barrel_Temperature_5            |             0.159217 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 4726

**Reason:** 미성형 => Unshaped

This failure looks most associated with the screw rotation speed during material preparation, the temperature in the third barrel heating zone, and the time used to melt and prepare the plastic before injection. Hopper area temperature and the part type being run may also have played a role in the cycle conditions. Injection pressure and injection speed, along with temperatures in the fourth and fifth barrel zones, were additional possible contributors. Overall, the cycle may have been sensitive to material preparation and barrel heating conditions.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 4726

**Reason:** 미성형 => Unshaped

The recent production failure is primarily associated with variations in the average screw rotation speed during material preparation. The temperature in the third heating zone of the barrel and the time required to melt and prepare the plastic also appear to be contributing factors. Additionally, fluctuations in hopper temperature, injection pressure, and injection speed may have influenced the outcome of this cycle. Reviewing these process conditions may help confirm their impact on current production consistency.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 4726

**Reason:** 미성형 => Unshaped

This failure may be linked to variations in material preparation, particularly the average screw speed and plasticizing time, which can affect material consistency. The temperature in the third heating zone of the barrel was also a notable factor, suggesting uneven melting or material flow. The hopper temperature and specific part types being produced may have contributed to the issue, possibly due to material handling or part-specific sensitivities. Injection pressure and speed were additional factors, indicating potential instability during mold filling. Barrel temperatures in zones four and five were also involved, reinforcing the role of thermal conditions in this cycle.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5183

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| Average_Screw_RPM               |             3.33814  |
| Max_Back_Pressure               |             1.91072  |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             0.702418 |
| Clamp_Close_Time                |             0.614865 |
| Barrel_Temperature_3            |             0.491025 |
| Plasticizing_Time               |             0.453288 |
| PART_NAME_CN7 W/S SIDE MLD'G LH |             0.387758 |
| Average_Back_Pressure           |             0.387138 |
| Hopper_Temperature              |             0.336166 |
| Barrel_Temperature_4            |             0.304961 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5183

**Reason:** 가스 => Gas

The cycle looks most associated with material preparation conditions, especially the average screw rotation speed during material preparation and the highest resistance pressure during screw recovery and plasticizing. The mold closing time and the temperatures in the barrel heating zones may also have contributed, since these can affect how the material is prepared and injected. Plasticizing time and average back pressure are additional signs that the material-handling stage may have been a factor. The part type itself also appears linked to this failure risk, which may mean this product is more sensitive to process variation. Hopper temperature and another barrel zone temperature may have added to the risk as well.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5183

**Reason:** 가스 => Gas

This production cycle shows variations in material preparation, specifically regarding average screw rotation speed and back pressure, that may have contributed to the failure. The specific part configuration and the timing of the mold clamp closing also appear to be associated with this result. Additionally, inconsistencies in the third and fourth barrel heating zones, along with the time taken to prepare the plastic, are possible factors. Finally, fluctuations in the hopper temperature may have also influenced the outcome of this cycle.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5183

**Reason:** 가스 => Gas

This failure may be linked to variations in material preparation, particularly the average screw speed and peak back pressure during plasticizing. The specific part being produced (RG3 MOLD'G W/SHLD, LH) and clamp closing time also showed stronger associations with the issue. Additionally, barrel temperatures in zones 3 and 4, plasticizing time, and hopper temperature may have played supporting roles in the process conditions leading to the failure. The part type CN7 W/S SIDE MLD'G LH and average back pressure were less influential but still notable. Check these areas for inconsistencies that could affect material flow or stability.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5185

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| Average_Screw_RPM               |             3.22632  |
| Max_Back_Pressure               |             1.99207  |
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             0.677658 |
| Barrel_Temperature_3            |             0.593727 |
| Average_Back_Pressure           |             0.571508 |
| Clamp_Close_Time                |             0.543364 |
| Plasticizing_Time               |             0.498845 |
| Max_Injection_Pressure          |             0.446098 |
| Barrel_Temperature_5            |             0.397349 |
| PART_NAME_CN7 W/S SIDE MLD'G LH |             0.318748 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5185

**Reason:** 가스 => Gas

This cycle may have been more likely to fail because the screw rotation speed during material preparation was a major factor, along with the highest resistance pressure during screw recovery and plasticizing. The product type being run also appears to matter, which suggests this part may be more sensitive to process conditions. Temperature in the barrel heating zones, clamp closing time, plasticizing time, and injection pressure also seem to have contributed to the risk. Another part type in the history of this cycle was also associated with the failure, so the issue may be tied to a mix of part-specific and process-condition effects.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5185

**Reason:** 가스 => Gas

The production process for this cycle shows that the average screw rotation speed and back pressure during material preparation were significant factors and may have contributed to the failure. Additionally, the specific part being produced, along with temperature settings in the injection barrel, likely played a role in the outcome. Other process timings and pressures during the clamp and injection phases could also have been contributing factors. We recommend reviewing these preparation and molding settings to ensure they are consistent with their established quality standards.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5185

**Reason:** 가스 => Gas

This failure may be linked to variations in material preparation, particularly the average screw speed and high back pressure during plasticizing, which can affect material consistency. The part type "RG3 MOLD'G W/SHLD, LH" and specific barrel temperatures in zones 3 and 5 might also play a role, as they influence how the material melts and flows. Additionally, the time taken to close the mold clamp and the plasticizing time could contribute to instability in the process. High injection pressure may further indicate potential issues with material flow or mold filling. These factors together suggest conditions that could increase the risk of defects in this cycle.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5188

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             2.35756  |
| Max_Back_Pressure               |             1.28945  |
| Average_Screw_RPM               |             1.16402  |
| Plasticizing_Time               |             0.384992 |
| Clamp_Close_Time                |             0.308258 |
| Barrel_Temperature_5            |             0.231653 |
| Barrel_Temperature_3            |             0.217354 |
| Max_Injection_Pressure          |             0.206666 |
| Barrel_Temperature_4            |             0.194226 |
| Injection_Time                  |             0.16301  |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5188

**Reason:** 미성형 => Unshaped

This failure may be associated with the RG3 MOLD'G W/SHLD, LH part run, which suggests this product type had a higher risk in this cycle.  
The strongest process signals were in screw recovery and material prep, especially the highest resistance pressure during plasticizing and the average screw rotation speed, which may point to less stable melt preparation.  
Plasticizing time and clamp close time also stood out, along with barrel temperatures in zones 3 to 5, suggesting the melt and mold conditions may not have been fully consistent.  
Injection pressure and injection time also contributed, so the fill and packing sequence may have been part of the issue.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5188

**Reason:** 미성형 => Unshaped

The production of the RG3 molding with shield, LH, was identified as a cycle with potential concerns. Variations in the back pressure and average screw rotation speed during material preparation were significant factors associated with this result. Additionally, inconsistencies in the time taken for plasticizing and clamping, as well as shifts in specific barrel zone temperatures and injection pressure, may have contributed to the process instability. Reviewing these mechanical and thermal settings may help clarify the conditions surrounding this production cycle.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5188

**Reason:** 미성형 => Unshaped

This failure may be linked to the specific part being produced (PART_NAME_RG3 MOLD'G W/SHLD, LH), as it was the most strongly associated factor. The highest resistance pressure during material preparation (Max_Back_Pressure) and the average screw speed (Average_Screw_RPM) also played a notable role, suggesting potential issues with material processing. The time taken to melt and prepare the plastic (Plasticizing_Time) and the mold clamp closing time (Clamp_Close_Time) were additional contributing factors. Temperatures in the barrel's heating zones (especially zones 3, 4, and 5) and the maximum injection pressure may have further influenced the outcome. These conditions together could indicate variability in material handling or process stability during this cycle.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5190

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             2.32965  |
| Max_Back_Pressure               |             1.2724   |
| Average_Screw_RPM               |             1.20342  |
| Barrel_Temperature_4            |             0.489393 |
| Plasticizing_Time               |             0.341227 |
| Clamp_Close_Time                |             0.296555 |
| Barrel_Temperature_3            |             0.202296 |
| Injection_Time                  |             0.161457 |
| Max_Injection_Pressure          |             0.156108 |
| Barrel_Temperature_5            |             0.148473 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5190

**Reason:** 미성형 => Unshaped

This failure may be linked first to the specific part being made, which can have tighter process sensitivity than other parts.  
The strongest process factors were the highest resistance pressure during screw recovery and plasticizing, along with the average screw rotation speed during material preparation, which suggests the material prep stage may have been a key contributor.  
Heating conditions in the barrel, especially in the third, fourth, and fifth zones, also appear to have played a role, along with plasticizing time and clamp close time.  
Injection time and the highest injection pressure were also associated with this cycle’s failure risk, so the issue may be tied to how the material was prepared and injected on this part.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5190

**Reason:** 미성형 => Unshaped

The specific production run of the RG3 MOLD'G W/SHLD, LH part is the primary factor associated with this failure. Variations in the material preparation process, particularly the maximum resistance pressure during screw recovery and the average screw rotation speed, may have contributed to this result. Additionally, the temperature settings across the middle barrel zones, along with the duration of the plasticizing process, are potential factors in this cycle's performance. Minor variations in clamp closing time, injection timing, and injection pressure are also linked to this failure. Please review these settings to ensure they remain within established process standards.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5190

**Reason:** 미성형 => Unshaped

This failure may be linked to the specific part being produced (PART_NAME_RG3 MOLD'G W/SHLD, LH), as it was the most strongly associated factor. The highest resistance pressure during screw recovery (Max_Back_Pressure) and the average screw rotation speed (Average_Screw_RPM) during material preparation were also key contributors, suggesting potential issues with material processing. The temperature in the fourth heating zone of the injection barrel (Barrel_Temperature_4) and the time taken to melt and prepare the plastic (Plasticizing_Time) may have played a role as well. Additionally, the time taken for the mold clamp to close (Clamp_Close_Time) and the temperature in the third heating zone (Barrel_Temperature_3) could have been influencing factors.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5192

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             2.48769  |
| Max_Back_Pressure               |             1.21786  |
| Average_Screw_RPM               |             1.17579  |
| Clamp_Close_Time                |             0.349701 |
| Barrel_Temperature_5            |             0.328133 |
| Barrel_Temperature_3            |             0.304889 |
| Plasticizing_Time               |             0.270693 |
| Max_Injection_Pressure          |             0.242305 |
| Barrel_Temperature_4            |             0.220438 |
| Injection_Time                  |             0.161786 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5192

**Reason:** 가스 => Gas

This failure is most associated with the part type being run, which may have different process needs or sensitivity than other parts. The strongest process factors linked to the failure were the highest back pressure during plasticizing and the average screw speed, suggesting the material preparation step may have been less stable for this cycle. Clamp closing time, barrel temperatures in several zones, and plasticizing time also stand out as possible contributors, along with injection pressure and injection time. Together, these points suggest the cycle may have had an issue in material preparation and mold filling conditions.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5192

**Reason:** 가스 => Gas

The production of the RG3 MOLD'G W/SHLD, LH part is the primary factor associated with this cycle's result. Variations in the back pressure applied during screw recovery and the average screw rotation speed were also significant contributors to the process outcome. Fluctuations in the mold clamp closing time, barrel heating zone temperatures, and material preparation timing may have further impacted the process stability. Finally, consider reviewing the injection pressure and injection timing for any potential irregularities.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5192

**Reason:** 가스 => Gas

This failure may be linked to the specific part being produced (PART_NAME_RG3 MOLD'G W/SHLD, LH), as it was the most strongly associated factor. The highest resistance pressure during screw recovery and plasticizing, along with the average screw rotation speed, also played a notable role. Additionally, variations in mold clamp closing time, barrel temperatures in zones 3, 4, and 5, and plasticizing time may have contributed. The highest injection pressure and injection time were less influential but could still be related to the issue. These conditions together suggest a combination of material preparation, pressure control, and part-specific factors that may have increased failure risk.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5205

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| PART_NAME_RG3 MOLD'G W/SHLD, LH |             2.37951  |
| Max_Back_Pressure               |             1.20328  |
| Average_Screw_RPM               |             1.18679  |
| Clamp_Close_Time                |             0.360926 |
| Plasticizing_Time               |             0.26996  |
| Hopper_Temperature              |             0.20775  |
| Barrel_Temperature_3            |             0.200379 |
| Barrel_Temperature_5            |             0.192911 |
| Max_Injection_Pressure          |             0.187038 |
| Injection_Time                  |             0.163035 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5205

**Reason:** 가스 => Gas

This failure may be linked to the specific part being run, since this part type has shown an association with higher risk in similar cycles. Material preparation conditions also stood out, especially the highest back pressure and average screw speed, which can affect how the plastic is melted and fed. Clamp closing time and plasticizing time may also have contributed, along with hopper and barrel heating conditions that influence melt quality. Injection pressure and injection time were also part of the pattern, suggesting the fill process for this cycle may have been less stable than usual.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5205

**Reason:** 가스 => Gas

This failure may be related to the specific production run of the RG3 MOLD'G W/SHLD, LH part. Key process conditions, such as the highest resistance pressure applied during screw recovery and the average screw rotation speed, appear to be significant contributors to this outcome. Variations in the mold clamp closing time and the time taken to prepare the plastic material also seem to be associated with the failure. Additionally, fluctuations in hopper and barrel temperatures, as well as the injection pressure and time during this cycle, may have played a role.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5205

**Reason:** 가스 => Gas

This failure may be linked to the specific part being produced (PART_NAME_RG3 MOLD'G W/SHLD, LH), as it was the most strongly associated factor. The highest resistance pressure during screw recovery and plasticizing, along with the average screw rotation speed, also played a notable role. Additionally, the time taken for the mold clamp to close and the plasticizing time could have contributed to the issue. Hopper temperature and temperatures in certain barrel heating zones were slightly involved, as well as the maximum injection pressure and injection time. These conditions together may have increased the risk of failure for this cycle.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------


## Top 10 SHAP Features for Index Row 5207

| feature_name                    |   feature_importance |
|:--------------------------------|---------------------:|
| PART_NAME_RG3 MOLD'G W/SHLD, LH |            2.16658   |
| Max_Back_Pressure               |            1.23719   |
| Average_Screw_RPM               |            1.1087    |
| Clamp_Close_Time                |            0.341588  |
| Barrel_Temperature_5            |            0.338849  |
| Plasticizing_Time               |            0.262676  |
| Max_Injection_Pressure          |            0.220152  |
| Barrel_Temperature_3            |            0.184678  |
| Injection_Time                  |            0.163124  |
| Barrel_Temperature_6            |            0.0971648 |

----------------------------------------------------------------------------------------------------
**Model:** `openai/gpt-5.4-mini`

**Index Row:** 5207

**Reason:** 가스 => Gas

This failure may be linked first to the specific part being run, which can have different process sensitivity than other parts. The strongest process-related factors were the screw recovery and plasticizing conditions, especially the highest back pressure and the average screw speed, which may have affected how the material was prepared. Clamp close time, barrel temperatures in several zones, plasticizing time, injection pressure, and injection time also stood out as possible contributors, suggesting the cycle may have had unstable molding conditions.

----------------------------------------------------------------------------------------------------
**Model:** `google/gemini-3.1-flash-lite`

**Index Row:** 5207

**Reason:** 가스 => Gas

The production of this specific part type was the most notable factor associated with this cycle's performance. The variation in back pressure and the average screw rotation speed during material preparation also appear to have contributed to the risk of failure. Additionally, fluctuations in clamp closing time and local temperature settings within the injection barrel may have influenced this outcome. Together, these factors suggest that settings related to material preparation and the initial injection stage were significant contributors to this production issue. Please review these process parameters to ensure they remain consistent with established operating standards.

----------------------------------------------------------------------------------------------------
**Model:** `mistralai/devstral-2512`

**Index Row:** 5207

**Reason:** 가스 => Gas

This failure may be linked to the specific part being produced (PART_NAME_RG3 MOLD'G W/SHLD, LH), as it was the most strongly associated factor. The highest resistance pressure during screw recovery and plasticizing, along with the average screw rotation speed during material preparation, also played a notable role. Additionally, variations in mold clamp closing time, barrel temperatures in zones 5 and 3, and plasticizing time may have contributed to the issue. Injection pressure and injection time were less influential but could still be related. These conditions together suggest a combination of part-specific and process factors that may have increased failure risk.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
