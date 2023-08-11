# Credit RISK Models

## Overview of the Analysis

* Purpose of the Analysis
The analysis was conducted to develop machine learning models that predict loan status (either "0" or "1") based on various financial features. By predicting loan status, the analysis aims to assess credit risk, which can help in making informed lending decisions.

* Financial Information and Prediction Target
The data consists of various financial features related to lending, and the target variable is "loan_status." The models were trained to predict this binary outcome, representing the creditworthiness of a borrower.

* Variables
The target variable, "loan_status," was predicted based on multiple financial features. The distribution of the target variable was analyzed, and class imbalance was addressed using the RandomOverSampler method.

* Stages of Machine Learning Process
The analysis included the following stages:
Data Loading and Exploration
Feature Selection
Data Splitting (Training and Testing Sets)
Model Training (including handling class imbalance)
Model Prediction and Evaluation

* Methods Used
Two machine learning models were used:
Logistic Regression
Logistic Regression with RandomOverSampler (to handle class imbalance)

## Results

Machine Learning Model 1: Logistic Regression
Accuracy Score: 0.9918
Confusion Matrix:
Predicted 0, Actual 0: 18663
Predicted 1, Actual 0: 102
Predicted 0, Actual 1: 56
Predicted 1, Actual 1: 563
Classification Report:
Precision: 0.99 (for 0), 0.91 (for 1)
Recall: 1.00 (for 0), 0.85 (for 1)
F1-Score: 1.00 (for 0), 0.88 (for 1)

Machine Learning Model 2: Logistic Regression with RandomOverSampler
Accuracy Score: 0.9938
Confusion Matrix:
Predicted 0, Actual 0: 18649
Predicted 1, Actual 0: 116
Predicted 0, Actual 1: 4
Predicted 1, Actual 1: 615
Classification Report:
Precision: 0.99 (for 0), 0.99 (for 1)
Recall: 1.00 (for 0), 0.84 (for 1)
F1-Score: 1.00 (for 0), 0.91 (for 1)

## Summary

The analysis involved the development of two machine learning models to predict loan status and assess credit risk. The first model used Logistic Regression, while the second model applied the RandomOverSampler technique to address class imbalance. Both models achieved high accuracy, with the second model showing a slight improvement. The results indicate that machine learning can be an effective tool in credit risk assessment, with the ability to accurately predict loan status based on financial features.

* Which one seems to perform best? How do you know it performs best?
Based on the accuracy scores, Model 2 (Logistic Regression with RandomOverSampler) performs slightly better overall. The precision for predicting class 1 is also higher in Model 2, while the recall for predicting class 1 is almost the same for both models.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
In this analysis, Model 2 shows higher precision in predicting class 1, which could be more favorable if the focus is on identifying high-risk loans.

If you do not recommend any of the models, please justify your reasoning.
Model 2(oversampled data fited) is recommended, it will help avoid money lost costed by false negatives which means lower risk level.
