# Default_Prediction_Multiple_Technique_Comparison
This project aims to build and evaluate various machine learning classifiers to predict credit risk. The dataset used contains information about customers, including their income, loan amount, credit score, and other relevant features, as well as a binary target variable indicating whether a customer is likely to default on a loan.

# Credit Risk Classification Project

## Overview

This project aims to build and evaluate various machine learning classifiers to predict credit risk. The dataset used contains information about customers, including their income, loan amount, credit score, and other relevant features, as well as a binary target variable indicating whether a customer is likely to default on a loan (1 for default, 0 for non-default).

## Dataset

The dataset for this project can be found on Kaggle: [Loan Default Dataset](https://www.kaggle.com/datasets/nikhil1e9/loan-default).

## Data Preprocessing

- The dataset was loaded and preprocessed to handle missing values and categorical variables.
- Standardization (scaling) was applied to ensure consistent data ranges across features.

## Handling Class Imbalance

- The target variable showed a significant class imbalance, with a majority of non-default cases.
- Synthetic Minority Over-sampling Technique (SMOTE) was employed to balance the dataset, creating synthetic instances of the minority class.

## Model Selection and Evaluation

- Seven different classifiers were selected for the project:
  - Decision Tree
  - Random Forest
  - Support Vector Machine (SVM)
  - k-Nearest Neighbors (k-NN)
  - Naive Bayes
  - XGBoost
  - Nearest Centroid
- Model performance was evaluated using various metrics, including accuracy, F1 score, precision, recall, and ROC AUC.
- Cross-validation was employed to assess each classifier's performance robustly.

## Results

Here are the evaluation results for each classifier:

| Classifier      | Accuracy | F1 Score | Precision | Recall  | ROC AUC |
|-----------------|----------|----------|-----------|---------|---------|
| Decision Tree   | 0.8201   | 0.8225   | 0.8016    | 0.8486  | 0.8201  |
| Random Forest   | 0.8886   | 0.8847   | 0.8810    | 0.8954  | 0.9587  |
| SVM             | 0.7056   | 0.7158   | 0.6912    | 0.7425  | 0.7809  |
| k-NN            | 0.8163   | 0.8412   | 0.7407    | 0.9734  | 0.9129  |
| Naive Bayes     | 0.7511   | 0.7562   | 0.7354    | 0.7809  | 0.8328  |
| XGBoost         | 0.8973   | 0.8888   | 0.8985    | 0.8947  | 0.9664  |

## Conclusion

The Random Forest and XGBoost classifiers outperformed other models across multiple evaluation metrics. These models demonstrated higher accuracy, F1 score, precision, and ROC AUC, making them suitable candidates for credit risk prediction tasks. Additionally, the use of SMOTE to address class imbalance improved the model's performance in handling default cases.
