# 💳 Loan Approval Prediction

## 📌 Project Overview

This project focuses on predicting whether a loan application will be approved or rejected based on applicant financial and profile attributes.

The objective is to build and compare classification models while properly handling class imbalance and evaluating performance using multiple metrics.


## 🎯 Problem Statement

Given applicant information such as income, employment status, credit history, and other financial indicators, the goal is to predict loan approval status.

This is a binary classification problem with moderately imbalanced classes.


## 📊 Dataset Information

- Total Samples: 4,000+
- Target Variable: `loan_status`
- Classes:
  - Approved
  - Rejected

No missing values were present after inspection.


## ⚙️ Methodology

### 1️⃣ Data Preparation
- Removed unnecessary identifier columns
- Cleaned string columns (removed extra spaces)
- Stratified train-test split
- Applied scaling to numeric features
- One-hot encoded categorical variables

### 2️⃣ Models Implemented
- Logistic Regression (Baseline)
- Decision Tree
- Logistic Regression with SMOTE

### 3️⃣ Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix


## 📈 Model Performance Summary

| Model | Accuracy |
|--------|----------|
| Logistic Regression | 93.56% |
| Decision Tree | **97.19%** |
| SMOTE + Logistic | 93.21% |

Decision Tree achieved the highest accuracy and balanced performance across both Approved and Rejected classes.

Applying SMOTE did not significantly improve performance, indicating the dataset was not severely imbalanced.

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib
- Seaborn
- Jupyter Notebook

## 🧠 Key Learning Outcomes

- Binary classification modeling
- Handling class imbalance
- Pipeline-based preprocessing
- Model comparison
- Confusion matrix interpretation
- Practical evaluation using multiple performance metrics
