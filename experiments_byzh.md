### 1. Sensitivity Analysis on the Number of Evolutionary Training Cases (TC)

The following table presents the sensitivity analysis results regarding the number of evolutionary training cases (denoted as the **TC** series). This experiment evaluates how different quantities of training cases affect the model's scheduling performance, measured by the Average Makespan across different problem scenarios (S1, S2, S3) and the overall average (All). 

As observed in the results, **TC_05** generally achieves the most competitive performance, yielding the lowest Average Makespan in the overall evaluation and across most individual scenarios.

| Run | TC | NC | S1_Makespan | S2_Makespan | S3_Makespan | Overall_Makespan |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 1 | 50 | 1649.69 | 3353.70 | 6678.29 | 3893.90 |
| 2 | 1 | 75 | 1645.51 | 3331.13 | 6558.22 | 3844.95 |
| 3 | 1 | 100 | 1632.57 | 3246.89 | 6368.74 | 3749.40 |
| 4 | 1 | 150 | 1639.80 | 3297.70 | 6491.98 | 3809.82 |
| 5 | 1 | 200 | 1640.58 | 3306.69 | 6579.62 | 3842.30 |
| 6 | 3 | 50 | 1649.61 | 3357.09 | 6734.09 | 3913.60 |
| 7 | 3 | 75 | 1646.27 | 3338.77 | 6622.32 | 3869.12 |
| 8 | 3 | 100 | 1633.92 | 3257.55 | 6438.74 | 3776.74 |
| 9 | 3 | 150 | 1640.90 | 3307.08 | 6559.48 | 3835.82 |
| 10 | 3 | 200 | 1641.51 | 3315.17 | 6645.36 | 3867.35 |
| 11 | 5 | 50 | 1641.11 | 3305.32 | 6632.90 | 3859.78 |
| 12 | 5 | 75 | 1638.17 | 3288.98 | 6525.00 | 3817.38 |
| 13 | 5 | 100 | 1626.09 | 3209.16 | 6344.16 | 3726.47 |
| 14 | 5 | 150 | 1632.96 | 3258.10 | 6463.74 | 3784.93 |
| 15 | 5 | 200 | 1633.48 | 3265.77 | 6548.80 | 3816.01 |
| 16 | 10 | 50 | 1646.22 | 3342.76 | 6727.56 | 3905.51 |
| 17 | 10 | 75 | 1643.11 | 3325.60 | 6618.08 | 3862.27 |
| 18 | 10 | 100 | 1630.93 | 3245.22 | 6436.12 | 3770.75 |
| 19 | 10 | 150 | 1638.32 | 3296.84 | 6560.95 | 3832.04 |
| 20 | 10 | 200 | 1639.22 | 3306.41 | 6649.72 | 3865.12 |
| 21 | 20 | 50 | 1639.92 | 3317.48 | 6652.66 | 3870.02 |
| 22 | 20 | 75 | 1636.66 | 3299.53 | 6541.61 | 3825.93 |
| 23 | 20 | 100 | 1624.36 | 3218.57 | 6358.53 | 3733.82 |
| 24 | 20 | 150 | 1632.28 | 3272.87 | 6488.60 | 3797.92 |
| 25 | 20 | 200 | 1633.56 | 3284.34 | 6581.10 | 3833.00 |

---

### 2. Sensitivity Analysis on the Number of Cells Partitioned in the CVT Space (NC)

This table illustrates the sensitivity analysis for the number of cells partitioned within the Centroidal Voronoi Tessellation (CVT) space (denoted as the **NC** series). Proper partitioning of the CVT space is crucial for maintaining rule diversity and quality during the evolutionary process. 

| Factor | Level | S1_Mean | S2_Mean | S3_Mean | Overall_Mean |
| :--- | :--- | :--- | :--- | :--- | :--- |
| TC | 1 | 1641.63 | 3307.22 | 6535.37 | 3828.07 |
| TC | 3 | 1642.45 | 3315.13 | 6600.00 | 3852.52 |
| TC | 5 | 1634.36 | 3265.46 | 6502.92 | 3800.92 |
| TC | 10 | 1639.56 | 3303.36 | 6598.49 | 3847.14 |
| TC | 20 | 1633.36 | 3278.56 | 6524.50 | 3812.14 |
| NC | 50 | 1645.31 | 3335.27 | 6685.10 | 3888.56 |
| NC | 75 | 1641.94 | 3316.80 | 6573.05 | 3843.93 |
| NC | 100 | 1629.57 | 3235.48 | 6389.26 | 3751.44 |
| NC | 150 | 1636.85 | 3286.52 | 6512.95 | 3812.11 |
| NC | 200 | 1637.67 | 3295.68 | 6600.92 | 3844.76 |

| Rank | Factor | Delta_Overall | Optimal_Level |
| :--- | :--- | :--- | :--- |
| 1 | NC | 137.12 | 100 |
| 2 | TC | 51.61 | 5 |

---

### 3. Taguchi Orthogonal Analysis for Stage-II Fingerprint Construction and Extraction

To further analyze the parameter sensitivity of the second stage in the proposed framework, we conducted a Taguchi `L25` orthogonal experiment over three factors: the number of matched cases (`K`), the number of case-binding rules (`M`), and the offline case library size (`off_size`). The table below reports the makespan on the three scenario groups (`S1`, `S2`, and `S3`) together with the overall makespan.

Among the 25 tested configurations, **Exp. 4** (`K=4`, `M=4`, `Off_Size=150`) achieves the best directly observed result, with the lowest `Overall_Makespan` of **3739.22**.

| Run | K | M | Off_Size | S1_Makespan | S2_Makespan | S3_Makespan | Overall_Makespan |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 1 | 1 | 50 | 1734.95 | 3423.43 | 6735.34 | 3964.57 |
| 2 | 2 | 2 | 75 | 1677.24 | 3312.85 | 6532.40 | 3840.83 |
| 3 | 3 | 3 | 100 | 1643.00 | 3246.68 | 6410.58 | 3766.75 |
| 4 | 4 | 4 | 150 | 1632.25 | 3224.94 | 6369.89 | 3742.36 |
| 5 | 5 | 5 | 200 | 1644.97 | 3247.62 | 6410.32 | 3767.64 |
| 6 | 1 | 2 | 200 | 1706.82 | 3368.93 | 6632.31 | 3902.69 |
| 7 | 2 | 3 | 50 | 1674.26 | 3307.75 | 6523.74 | 3835.25 |
| 8 | 3 | 4 | 75 | 1642.42 | 3245.28 | 6409.65 | 3765.78 |
| 9 | 4 | 5 | 100 | 1634.06 | 3227.22 | 6376.68 | 3745.99 |
| 10 | 5 | 1 | 150 | 1667.78 | 3292.23 | 6493.53 | 3817.85 |
| 11 | 1 | 3 | 150 | 1686.32 | 3330.37 | 6564.31 | 3860.34 |
| 12 | 2 | 4 | 200 | 1668.05 | 3294.19 | 6493.42 | 3818.55 |
| 13 | 3 | 5 | 50 | 1656.85 | 3271.51 | 6458.89 | 3795.75 |
| 14 | 4 | 1 | 75 | 1671.22 | 3300.44 | 6508.48 | 3826.71 |
| 15 | 5 | 2 | 100 | 1642.10 | 3245.03 | 6409.14 | 3765.42 |
| 16 | 1 | 4 | 100 | 1680.83 | 3319.47 | 6546.49 | 3848.93 |
| 17 | 2 | 5 | 150 | 1664.95 | 3286.98 | 6483.32 | 3811.75 |
| 18 | 3 | 1 | 200 | 1689.18 | 3332.44 | 6562.97 | 3861.53 |
| 19 | 4 | 2 | 50 | 1658.15 | 3277.20 | 6466.54 | 3800.63 |
| 20 | 5 | 3 | 75 | 1631.43 | 3225.47 | 6374.92 | 3743.94 |
| 21 | 1 | 5 | 75 | 1690.34 | 3336.21 | 6578.84 | 3868.47 |
| 22 | 2 | 1 | 100 | 1695.21 | 3345.59 | 6591.23 | 3877.34 |
| 23 | 3 | 2 | 150 | 1658.59 | 3275.74 | 6461.69 | 3798.67 |
| 24 | 4 | 3 | 200 | 1645.44 | 3250.30 | 6413.27 | 3769.67 |
| 25 | 5 | 4 | 50 | 1635.77 | 3233.56 | 6390.88 | 3753.40 |

The main-effect analysis provides a more stable factor-level view by averaging the response at each level. According to `Overall_Mean`, the preferred levels are `K=5`, `M=4`, and `off_size=100`. This inferred optimum is slightly different from the single best run in the `L25` table, suggesting that the best-performing region is characterized by a larger matching set, a moderately large rule-binding set, and a moderate offline library size.

| Factor | Level | S1_Mean | S2_Mean | S3_Mean | Overall_Mean |
| :--- | :--- | :--- | :--- | :--- | :--- |
| K | 1 | 1699.85 | 3355.68 | 6611.46 | 3889.00 |
| K | 2 | 1675.94 | 3309.47 | 6524.82 | 3836.74 |
| K | 3 | 1658.01 | 3274.33 | 6460.75 | 3797.70 |
| K | 4 | 1648.22 | 3256.02 | 6426.97 | 3777.07 |
| K | 5 | 1644.41 | 3248.78 | 6415.76 | 3769.65 |
| M | 1 | 1691.67 | 3338.83 | 6578.31 | 3869.60 |
| M | 2 | 1668.58 | 3295.95 | 6500.41 | 3821.65 |
| M | 3 | 1656.09 | 3272.12 | 6457.36 | 3795.19 |
| M | 4 | 1651.86 | 3263.49 | 6442.06 | 3785.81 |
| M | 5 | 1658.24 | 3273.91 | 6461.61 | 3797.92 |
| Off_Size | 50 | 1672.00 | 3302.69 | 6515.08 | 3829.92 |
| Off_Size | 75 | 1662.53 | 3284.05 | 6480.86 | 3809.15 |
| Off_Size | 100 | 1659.04 | 3276.80 | 6466.82 | 3800.89 |
| Off_Size | 150 | 1661.98 | 3282.05 | 6474.55 | 3806.19 |
| Off_Size | 200 | 1670.89 | 3298.70 | 6502.46 | 3824.01 |

The factor ranking in the Taguchi analysis is highly consistent across both `Delta_Overall` and `Delta_SN`. Specifically, `K` is the most influential factor, followed by `M`, while `off_size` has a noticeably smaller impact. This indicates that performance is more sensitive to how many relevant cases are matched and how many rules are bound to each case than to simply enlarging the offline fingerprint library. In addition, the results show that increasing `off_size` beyond a moderate level does not continuously improve performance, and `off_size=100` already offers the best average trade-off.

| Rank | Factor | Delta_Overall | Optimal_Level |
| :--- | :--- | :--- | :--- |
| 1 | K | 119.35 | 5 |
| 2 | M | 83.80 | 4 |
| 3 | Off_Size | 29.03 | 100 |

### 4. Computational Cost and Resource Consumption

The table outlines the computational costs and resource consumption required to run and generate 400 valid rules across five different evolutionary frameworks: openevolve, alphaevolve, DSevolve, shinkaevolve, and Seevo. 

Key metrics evaluated include the total execution time (`duration_seconds`), the number of interactions with the Large Language Model (`llm_calls_total`), and detailed token usage breakdowns (`prompt_tokens_total`, `completion_tokens_total`, and `tokens_total`). 

| framework | duration_seconds | llm_calls_total | prompt_tokens_total | completion_tokens_total | tokens_total |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **openevolve** | 1199.7468910217285 | 442 | 4679965 | 480712 | 5160677 |
| **alphaevolve** | 1970.172393321991 | 480 | 4669582 | 278414 | 4947996 |
| **DSevolve** | 4146.187037706375 | 560 | 2654766 | 1079363 | 3734129 |
| **shinkaevolve** | 10325.659145355225 | 399 | 4155058 | 386658 | 4541716 |
| **Seevo** | 3579.176538927627 | 477 | 4547682 | 798754 | 5346436 |

---
