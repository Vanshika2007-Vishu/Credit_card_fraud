# Hospital Readmission Prediction

## About the Project

This project predicts whether a patient is likely to be readmitted to the hospital within 30 days.

A Logistic Regression model with L2 regularization is used for prediction. The model is evaluated using ROC-AUC, confusion matrix, precision, recall and F1-score.

## Dataset

The project uses the **Diabetes 130-US Hospitals for Years 1999-2008** dataset from the UCI Machine Learning Repository.

The dataset contains patient-related information such as hospital stay details, number of procedures, medications and previous hospital visits.

The dataset is loaded directly in the notebook, so no dataset file is required in this repository.

## Method Used

* Logistic Regression
* L2 Regularization
* StandardScaler for feature scaling
* 80-20 train-test split
* ROC-AUC evaluation
* Confusion Matrix
* Decision threshold analysis

## Features Used

The model uses the following numerical features:

* `time_in_hospital`
* `num_lab_procedures`
* `num_procedures`
* `num_medications`
* `number_outpatient`
* `number_emergency`
* `number_inpatient`

## Target

The target variable is:

* `1` → Patient was readmitted within 30 days
* `0` → Patient was not readmitted within 30 days

## Results

The model achieved a ROC-AUC score of approximately **0.63**.

A decision threshold of **0.30** was also tested to identify more patients who may be at risk of readmission.

At this threshold:

* Accuracy: approximately **89%**
* Readmission Precision: **0.40**
* Readmission Recall: **0.05**
* ROC-AUC: **0.6323**

## Clinical Cost of Errors

In this problem, false negatives can be more concerning because a patient who is actually at risk of readmission may be missed by the model.

False positives can result in additional follow-up, monitoring or healthcare resources being used for patients who may not actually be readmitted.

Therefore, the decision thres
