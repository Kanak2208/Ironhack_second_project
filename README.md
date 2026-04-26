# Ironhack_second_Project






----------------------------------------------------------------------------------------------------
## Hypothesis 1: Completion Rate

- **H0:** Completion rate between Control and Test groups is similar
- **H1:** Completion rate between Control and Test groups is different

**Test Used:** Two-proportion Z-test

**Results:**
| Group   | Completions | Total  | Rate   |
|---------|-------------|--------|--------|
| Control | 15,434      | 23,532 | 65.59% |
| Test    | 18,687      | 26,968 | 69.29% |

- Z-statistic: -8.8745
- P-value: ~0.0000

**Conclusion:**
We reject H0. The Test group shows a statistically significant higher completion 
rate (69.3%) compared to Control (65.6%), a difference of ~3.7 percentage points. 
This is unlikely due to random chance and suggests the new interface positively 
improved user completion behavior.

----------------------------------------------------------------------------------------------------
## Hypothesis 2: Demographic Fairness (Average Age)

- **H0:** Average age of Control and Test groups is similar
- **H1:** Average age of Control and Test groups is different

**Test Used:** Independent samples T-test

**Results:**
| Group   | Mean Age |
|---------|----------|
| Control | 47.50    |
| Test    | 47.16    |

- T-statistic: 2.4161
- P-value: 0.0157

**Conclusion:**
Although the t-test rejects H0 (p = 0.016 < 0.05), the actual difference in mean 
age is only 0.34 years — practically negligible. This is a known effect of large 
sample sizes, where even trivial differences become statistically significant. 
The experiment groups are considered demographically balanced and the A/B split 
was fair.
----------------------------------------------------------------------------------------------------
## Hypothesis 3: Time Spent on Steps

- **H0:** Median time per step is similar between Control and Test groups
- **H1:** Median time per step is different between Control and Test groups

**Test Used:** Mann-Whitney U test (chosen due to right-skewed time distribution)

**Results:**
| Group   | Median Time |
|---------|-------------|
| Control | 35.0 sec    |
| Test    | 34.0 sec    |

- U-statistic: 7,829,845,182.5
- P-value: 0.3765

**Conclusion:**
We fail to reject H0 (p = 0.3765 > 0.05). The median time spent on steps is 
nearly identical between groups — just 1 second apart. The new interface did 
not significantly change the time users spent navigating through the process steps.