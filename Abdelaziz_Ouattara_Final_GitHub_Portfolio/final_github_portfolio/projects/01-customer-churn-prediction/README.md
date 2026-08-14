# Customer Churn Prediction

**Status:** Complete

## Overview
End-to-end telecom churn analysis using the IBM Telco Customer Churn dataset. The project compares Logistic Regression, Decision Tree, and Random Forest using cross-validation and holdout testing. Logistic Regression achieved the strongest ROC-AUC at 0.8413 with 78.34% churn recall.

## Tools
Python, pandas, scikit-learn, Matplotlib, Machine Learning

## How to Run
1. Open `analysis.ipynb` in Jupyter Notebook or JupyterLab.
2. Restart the kernel.
3. Run all cells from top to bottom.

## Key Results
- 7,043 customer records analyzed.
- Overall churn rate: 26.54%.
- Selected model: Logistic Regression.
- Holdout ROC-AUC: 0.8413.
- Recall: 0.7834.
- Strong patterns included month-to-month contracts, short tenure, fiber-optic service, and electronic-check payment.

If the original dataset is not stored in this repository, place `WA_Fn-UseC_-Telco-Customer-Churn.csv` beside the notebook before running.

## Portfolio Notes
This project is included to demonstrate a specific part of the data science workflow and is documented so that a reviewer can quickly understand the objective, method, and output.
