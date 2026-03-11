# Logistic and Bayesian Regression Analysis of Campaign Outcomes

## Project Overview
This project analyzes the success and failure of violent and nonviolent political campaigns using regression modeling in R. The analysis uses the NAVCO-style campaign dataset and examines how campaign type, democracy, duration, international support, repression, and defections relate to campaign outcomes.

## Research Questions
1. Are nonviolent campaigns more successful than violent campaigns?
2. What other factors influence campaign success or failure?
3. Do the conclusions remain consistent under both likelihood-based and Bayesian inference?

## Methods
The project uses a two-stage modeling strategy:

- **Model 1:** Logistic regression for failure vs. not-failure
- **Model 2:** Logistic regression for full success vs. partial success, conditional on not failing
- **Likelihood Ratio Tests (LRTs):** To evaluate interaction effects
- **Bayesian Logistic Regression:** To assess robustness of conclusions using weakly informative priors

## Key Variables
- Campaign type: violent vs. nonviolent
- Democracy score
- Campaign duration (log-transformed)
- International sanctions
- Foreign aid
- International support
- Violent repression
- Security-force defections
- Year of campaign

## Main Findings
- Nonviolent campaigns had substantially lower odds of outright failure than violent campaigns.
- Democracy reduced failure risk, especially for nonviolent campaigns.
- Security-force defections were strongly associated with higher chances of full success.
- Longer campaigns were less likely to move from partial to full success.
- Bayesian analysis confirmed the main likelihood-based conclusions.

## Tools Used
- R
- RMarkdown
- ggplot2
- dplyr
- broom
- car
- pROC
- rstanarm

## Files
- `code/Regs-Final_Take_home.Rmd`: Full reproducible analysis
- `report/regression_analysis_report.pdf`: Final written report
- `data/navc.csv`: Dataset used for analysis

## Authors
- Matthew Nartey
- Isaac Gbene
