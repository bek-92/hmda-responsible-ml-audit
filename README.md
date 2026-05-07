# HMDA 2024 Responsible Machine Learning Audit

## Project Overview

This project audits mortgage approval prediction models using the 2024 HMDA Loan Application Register. The goal is to evaluate not only model performance, but also fairness, robustness, explainability, security risk, and deployment defensibility.

This project was completed for DNSC 6330: Responsible Machine Learning at George Washington University.

## Team

Group 6  
George Washington University School of Business  
May 2026

## Files Included

| File | Description |
|---|---|
| `LR Model for RML (1).ipynb` | Logistic Regression model, baseline performance, and fairness diagnostics |
| `Gradient Boosting Model (2).ipynb` | Selected Gradient Boosting model, subgroup error analysis, robustness checks, and deployment evidence |
| `Random_Forest_RML (2).ipynb` | Random Forest challenger model and comparison metrics |
| `HMDA_Capstone_Group6.pptx` | Final capstone presentation summarizing the audit findings |

## Models Evaluated

We compared three models:

1. Logistic Regression
2. Gradient Boosting
3. Random Forest

The Gradient Boosting model was selected because it provided strong overall performance, strong calibration, and the lowest Black applicant false positive rate among the compared models.

## Key Metrics

The audit uses the following metrics:

- AUC-ROC
- Brier Score
- Train-test generalization gap
- False Positive Rate
- False Negative Rate
- Adverse Impact Ratio
- Standardized Mean Difference
- Population Stability Index
- Security stress tests

## Fairness Audit

The model was evaluated across protected and sensitive attributes including race, sex, age, and intersectional groups.

The audit uses the four-fifths rule as a screening benchmark:

```text
AIR = protected group approval rate / reference group approval rate