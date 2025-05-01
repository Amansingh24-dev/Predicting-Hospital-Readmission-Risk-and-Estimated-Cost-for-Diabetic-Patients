#  Predicting Hospital Readmission Risk and Estimating Cost for Diabetic Patients

A machine learning project that predicts 30-day hospital readmission risk and estimates hospitalization cost for diabetic patients using clinical data from the UCI dataset.



# Problem Statement

Hospitals face financial and clinical challenges due to unplanned readmissions of diabetic patients. Identifying high-risk patients early can help reduce costs and improve patient care. This project aims to:

- Predict whether a diabetic patient will be readmitted within 30 days.
- Estimate the hospital cost based on their clinical profile.



# Project Objectives

- Build a classification model to detect 30-day readmission risk.
- Build a regression model to estimate cost using length of stay.
- Handle class imbalance using SMOTE.
- Evaluate models using standard metrics (Recall, AUC, R², MSE).
- Visualize predictions using confusion matrix and cost scatter plots.



# Dataset

- Source: [UCI ML Repository – Diabetes 130-US hospitals for years 1999–2008](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- ~100,000 patient records with 50+ attributes (diagnosis, medications, lab tests, etc.)



# ML Models Used

1. Classification: Readmission Risk
- Model: Random Forest Classifier
- Class Imbalance Handling**: SMOTE + `class_weight="balanced"`
- Performance:
  - Recall (YES class): 0.56
  - AUC Score:0.62

2. Regression: Hospital Cost Estimation
- Model: Random Forest Regressor
- Target: `time_in_hospital × $1200`
- Performance:
  - R² Score: ~0.99
  - Very low MSE


# Technologies Used

- Python, NumPy, Pandas
- Scikit-learn, imbalanced-learn
- Matplotlib, Seaborn
- Google Colab (Notebook environment)



# Visualizations

- Confusion Matrix for classifier
- ROC Curve
- Predicted vs Actual Hospital Cost Scatter Plot



