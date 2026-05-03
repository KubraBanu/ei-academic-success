# Emotional Intelligence & Academic Success

**Author:** Kubra Banu
**Presented at:** NEDSI 2025 Academic Conference

---

## Overview

This project investigates whether **Emotional Intelligence (EI)** is a statistically significant predictor of academic success in graduate school. Using the MacCann et al. (2020) meta-analytic dataset, we applied regression analysis and decision tree modeling in R to test EI as an alternative or complement to traditional academic predictors (GPA, GRE, SAT, IQ).

---

## Research Question

**Can measures of Emotional Intelligence be predictive markers for academic performance in graduate students?**

---

## Tools & Methods

| Tool / Method | Purpose |
|---------------|---------|
| **R / R Markdown** | Statistical analysis and reproducible reporting |
| **Regression Analysis** | 7 models testing EI measures vs. academic outcomes |
| **Decision Tree (rpart)** | Non-linear classification of academic performance |
| **Cross-Validation** | Model generalizability testing |
| **Pruned Decision Tree** | Complexity reduction for interpretability |
| **ANOVA / F-statistic** | Variance comparison across groups |
| **Q-Q Plots / Residual Analysis** | Model assumption validation |

---

## Dataset

- **MacCann et al. (2020)** — Meta-analytic dataset on EI and academic performance
- Source: Published in *Psychological Bulletin* (Oct 2019)
- Variables include EI measures (MSCEIT, EQI), publication type, sample demographics, effect sizes, and academic outcome metrics

---

## Methodology

1. **Data Cleaning** — Trimmed outliers, handled missing values (NaN), standardized variables
2. **Descriptive Statistics** — Pre/post-trim summary statistics, variable distributions
3. **Regression Analysis** — 7 progressive models (Models 1–7) testing EI predictors on academic outcomes
4. **Decision Tree** — Branched classification tree using `rpart`, visualized with `rpart.plot`
5. **Cross-Validation** — xerror minimization to identify optimal tree complexity parameter (CP)
6. **Pruned Tree** — Final interpretable model based on optimal CP

---

## Key Findings

- EI measures show statistically significant associations with academic performance
- Regression models indicate EI explains variance in outcomes beyond traditional cognitive measures
- Decision tree analysis identifies key EI thresholds that distinguish high vs. low academic performers
- Results suggest EI could complement GPA/GRE as an admissions evaluation tool

---

## Files

| File | Description |
|------|-------------|
| `20241212_STAT4600_Final_project_Code_EI_Measures_KB_JK_KS_AZ.Rmd` | Main R Markdown analysis file |
| `20241212_STAT4600_Final_project_Code_EI_Measures_KB_JK_KS_AZ.html` | Rendered HTML output of full analysis |
| `20241212_KBanu_JKawal_KhabiShan_AZuger_Maccan_2020_EI_STAT4600_Final_Project.R` | EI_Analysis_Final.R |
| `maccann2020.csv` | Dataset used for analysis |
| `grouped_r2_summary.csv` | R-squared summary by model group |
| `model_summary.txt` – `model7_summary.txt` | Individual regression model outputs |
| `202411208_KB_JK_KS_AZ_STAT4600_FInal_Project_v4.pdf` | Final project report |
| `20241128_Update_STAT_4600_Project_EI_PPT.pptx` | Final presentation slides |
| `2025_Emotional_Intelligence_Clark_Unovserity_Presentation.pptx` | NEDSI 2025 conference presentation |
| `2025_NEDSI_Poster_Emotional_Intellgience.pptx` | NEDSI 2025 research poster |
| `20241201_Finalized_Project_Proposal_v6.pdf` | Final project proposal |

---

## References

- MacCann, C. et al. (2020). *Emotional intelligence predicts academic performance: A meta-analysis.* Psychological Bulletin.
- Haynes, 2023 — SAT score limitations in predicting GPA
- Kobrin et al., 2008 — SAT correlation study (n=50,000)
