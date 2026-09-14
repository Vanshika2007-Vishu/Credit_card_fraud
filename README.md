# Credit Card Fraud Detection

## About the Project

This project detects fraudulent credit card transactions using **XGBoost**.

Since fraud transactions are much fewer than normal transactions, the dataset is highly imbalanced. **SMOTE (Synthetic Minority Oversampling Technique)** is used to balance the training data.

Different decision thresholds are also tested to see how they affect precision, recall and F1-score.

## Dataset

The project uses the **Credit Card Fraud Detection** dataset from Kaggle.

The dataset contains **284,807 transactions**, including **492 fraudulent transactions**.

The dataset is loaded directly in the notebook, so the dataset file does not need to be uploaded to this repository.

## Method Used

* XGBoost Classifier
* SMOTE for handling class imbalance
* 80-20 train-test split
* Decision threshold analysis
* Confusion Matrix
* Precision, Recall and F1-score
* Feature Importance

## Target

The target variable is:

* `0` → Normal transaction
* `1` → Fraudulent transaction

## Class Distribution

The original dataset is highly imbalanced:

* Normal transactions: **284,315**
* Fraudulent transactions: **492**

SMOTE is applied only to the training data to increase the numb
