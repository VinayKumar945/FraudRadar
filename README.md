# FraudRadar: Credit Card Fraud Detection

FraudRadar is a machine learning project for detecting fraudulent credit card transactions using the popular `creditcard.csv` dataset. The project focuses on handling class imbalance, evaluating fraud detection performance with the right metrics, tuning decision thresholds, explaining predictions with SHAP, and exporting the final model for future deployment.

## Project Goal

The goal of this project is to build and compare fraud detection models that can identify rare fraudulent transactions accurately. Since fraud detection is a highly imbalanced classification problem, this project emphasizes metrics such as PR-AUC and recall instead of relying only on accuracy.

## Features

- Loads and explores the credit card fraud dataset
- Performs preprocessing on `Amount` and `Time`
- Handles class imbalance using SMOTE
- Trains multiple models:
  - Logistic Regression
  - Random Forest
  - XGBoost
- Evaluates models using:
  - ROC-AUC
  - PR-AUC
  - Classification report
  - Confusion matrix
- Tunes threshold for better fraud recall and F1 balance
- Uses SHAP for model explainability
- Saves the best model for later use

## Dataset

This project uses the well-known `creditcard.csv` fraud detection dataset.

Because the dataset may be large or licensing may vary, it is not included directly in this repository. Please place the dataset file here before running the notebook:

```bash
data/creditcard.csv
