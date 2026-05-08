# Credit Risk Detection

## Problem Statement
This project solves the problem of credit risk detection. Banks and financial companies can use this model to identify whether a person should be given a credit card or not, based on their financial profile. This helps companies reduce defaults and increase profitability.

## Dataset
Source: Kaggle — Credit Risk Dataset. Contains features like income, loan intent, loan grade, employment length, and home ownership.

## Approach
Supervised machine learning. Models tried: Logistic Regression, Random Forest (default), Random Forest (tuned), and XGBoost.

## Results
| Model | Accuracy | Recall | Precision | F1 Score | Verdict |
|-------|----------|--------|-----------|----------|---------|
| Logistic Regression | 93.14% | 77.8% | 55.4% | 0.647 | High recall, many false alarms |
| Random Forest (Default) | 93.14% | 71.1% | 97.1% | 0.822 | Overfitted |
| Random Forest (Tuned) | 89.95% | 77.0% | 77.5% | 0.772 | Balanced |
| XGBoost | 93.36% | 74.1% | 94.8% | 0.832 | Best ✅ |

## Key Learnings
- High income applicants → approve easily (low risk)
- Medium income applicants → depends on ML model threshold tuning
- Low income applicants → strict checks required
