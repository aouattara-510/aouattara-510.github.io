# DSC 680 Project 3 - Customer Churn Prediction

**Student:** Abdelaziz Frederic Ouattara  
**Milestone:** 3 - Final Project

## Project Summary
This project analyzes the IBM Telco Customer Churn dataset and compares Logistic Regression, Decision Tree, and Random Forest models. The executed analysis contains 7,043 customer records with an overall churn rate of 26.54%.

## Final Model Results
| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.7381 | 0.5043 | 0.7834 | 0.6136 | **0.8413** |
| Random Forest | **0.7764** | **0.5646** | 0.6898 | **0.6209** | 0.8375 |
| Decision Tree | 0.7402 | 0.5068 | **0.7941** | 0.6188 | 0.8343 |

**Selected model:** Logistic Regression because it produced the highest holdout ROC-AUC (0.8413) and the highest mean five-fold cross-validation ROC-AUC (0.8459).

## Key Findings
- Month-to-month churn: 42.7%; one-year: 11.3%; two-year: 2.8%.
- Fiber-optic churn: 41.9%; DSL: 19.0%; no internet: 7.4%.
- Electronic-check churn: 45.3%; automatic credit-card churn: 15.2%.
- Tenure was the strongest Random Forest feature (importance 0.1254) and the largest-magnitude Logistic Regression coefficient (-1.1236).
- Logistic Regression confusion matrix: TN=747, FP=288, FN=81, TP=293.

## Research Questions
1. Which customer characteristics are most strongly associated with customer churn?
2. Can machine learning accurately predict whether a customer will leave?
3. Which classification algorithm performs best for predicting customer churn?
4. What business recommendations can be made to reduce customer attrition?

## Files
- `Final_Project_3_Customer_Churn.ipynb` - reproducible analysis notebook.
- `Project_3_White_Paper_FINAL.docx` - final white paper with actual results.
- `Project_3_QA_FINAL.docx` - final answers to the research questions.
- `Project_3_Presentation_FINAL.pptx` - final 10-slide presentation with speaker notes.
- `Presentation_Narration_Script_FINAL.docx` - narration script for the required 5-10 minute presentation.
- `requirements.txt` - Python dependencies.

## Dataset
IBM Telco Customer Churn, commonly distributed through Kaggle. The executed notebook shown in the submitted PDF loaded a public raw mirror of the same 7,043-row dataset because the local-file check did not resolve in that run.

## Reproducing the Analysis
1. Place `WA_Fn-UseC_-Telco-Customer-Churn.csv` in the same folder as the notebook.
2. Install dependencies with `pip install -r requirements.txt`.
3. Open the notebook in Jupyter.
4. Restart the kernel and run all cells.

## Responsible Use
The model should support retention outreach rather than adverse automated decisions. Operational deployment would require local validation, privacy controls, fairness/error monitoring, human oversight, and ongoing model-drift monitoring.
