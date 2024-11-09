# Module 12 Report

## Overview of the Analysis

The goal was to use machine learning to classify loans as either healthy (0) or high-risk (1) based on various financial metrics.

The dataset contained information on loans, including features like loan_amnt, int_rate, annual_inc, and other financial indicators.
The target variable was loan_status, where 0 indicates a healthy loan and 1 indicates a high-risk loan.

Steps for the analysis:

1. Loaded the dataset and split it into features (X) and labels (y).
2. Performed a train-test split with 70% of the data for training and 30% for testing.
3. Used a Logistic Regression model for binary classification due to its simplicity and effectiveness.
4. Evaluated the model using a confusion matrix and a classification report to measure accuracy, precision, recall, and F1 scores.



## Results

Accuracy: 99%
Precision (0 - healthy loans): 99%
Recall (0 - healthy loans): 100%
Precision (1 - high-risk loans): Low (due to class imbalance)
Recall (1 - high-risk loans): Low (due to many false negatives)
F1 Score:
Healthy loans (0): High F1 score, shows strong performance for predicting healthy loans.
High-risk loans (1): Lower F1 score, shows difficulty in identifying high-risk loans.


## Summary

The Logistic Regression model demonstrated high accuracy and performed well in predicting healthy loans (0) with strong precision and recall.
However, its performance in predicting high-risk loans (1) was limited, likely due to the dataset not having a balancing nature.

Based on the current model's performance, I would recommend using Logistic Regression for general loan classification if healthy loans are the focus.