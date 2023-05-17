# credit-risk-classification


## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of the analysis is to train a model that can classify and identify the creditworthiness of borrowers
* The dataset is of historical lending activity from a peer-to-peer lending services company, and what you are trying to predict are the people who are likely to default on a loan.
* The variables that is being predicted is the lr_prediction. I start with the y which holds the values of the loan_status column and use the value_counts method to see the count of good and bad loans in the dataset. I use this information to build the test data for training and prediction.
* I build two models and used `LogisticRegression` method on one, and `RandomOverSampler` on the other.

## Results

* Machine Learning Model 1: `LogisticRegression`
  * `balanced_accuracy_score` : 0.9520479254722232
  * `precision` : 0 = 1.00, 1 = 0.85
  * `recall` : 0 = 0.99, 1 = 0.91
  

* Machine Learning Model 2: `RandomOverSampler`
  * `balanced_accuracy_score` : 0.9936781215845847
  * `precision` : 0 = 1.00, 1 = 0.84
  * `recall` : 0 = 0.99, 1 = 0.99

## Summary

Based on the analysis, it appears that Model 2 outperforms Model 1 in predicting high-risk loans and has an overall higher accuracy in predicting both labels. Specifically, Model 2 achieved a relatively high precision in predicting high-risk loans while correctly identifying all high-risk loans in the dataset, which is considered a relatively good performance in this context. Therefore, I would recommend using Model 2 in identifying high-risk loans and overall better accuracy in predicting labels.
