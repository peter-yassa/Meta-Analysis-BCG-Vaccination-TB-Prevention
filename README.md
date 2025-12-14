# Meta-Analysis-BCG-Vaccination-TB-Prevention
## Overview
I utilized RStudio to evaulate the efficacy of bacillus Calmette-Guerin (BCG) vaccination on tuberculosis across multiple clinical trials. I conducted this meta-analysis using summary data obtained from the metafor R package (dat.bcg), which compiled randomized controlled trials (RCTs) evaluating the efficacy of BCG vaccination against tuberculosis. 

The `dat.bcg` dataset included 13 RCTs conducted between 1948 and 1980.

## Methods
Given the variability in study design and sample size of included trials, I conducted a random-effects meta-analysis. I used restricted maximum likelihood (REML) estimation to generate a pooled odds ratio (OR) and corresponding 95% confidence interval (CI) for the association between BCG vaccination and TB 

After conducting the analysis, I assessed for heterogeneity using Q-statistics and I².

To explore the impact of heterogeneity, meta-regression was performed to evaluate the impact of allocation method and absolute latitude on treatment effects.

## Results
The pooled analysis demonstrated a significant protective effect of BCG vaccination (OR = 0.47, 95% CI: 0.33–0.68),  suggesting that BCG vaccination was associated with a 53% reduction in the odds of developing TB compared to controls

However, substantial heterogeneity was observed. The I² statistic indicated that approximately 92% of the total variability in observed effect sizes was attributable to heterogeneity rather than sampling error, which was supported by a statistically significant Cochran’s Q test (p < 0.001).

Meta-regression indicated that absolute latitude explained a substantial proportion of between-study heterogeneity, while allocation method was not significantly associated with treatment effects.
