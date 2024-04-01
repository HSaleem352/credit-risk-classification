# Module 20 Report Template

## Overview of the Analysis

* When lending companies provide money or properties to borrowers, they expect the borrower to either return the asset or repay the loan. Credit Risk arises when a borrower fails to fulfill this obligation, leading to financial losses for the lender. Lenders assess credit risk through various methods. However, in this analysis, the focus is on using Machine Learning to examine a dataset of past lending activities from a peer-to-peer lending services company. The goal is to develop a model that can effectively determine the creditworthiness of borrowers.

* With the dataset provided by the lending company, a Logistic Regression Model was created, achieving an accuracy score of 95%. Despite its high accuracy, the model's recall value for non-healthy loans is lower (0.91) compared to healthy loans (0.99). This suggests that the model is better at predicting loan statuses as healthy than identifying non-healthy ones. The imbalance in the dataset, where healthy loans significantly outnumber non-healthy ones, is the reason behind this observation.

* The Logistic Regression Algorithm is considered the most suitable tool for their machine learning model as it is widely utilized to predict the probability of a target variable in classification problems, therefore, this model was used.

## Results

* The Logistic Regression model fitted with the Original dataset predicted healthy loans 100% of the time and predicted non-healthy loans 85% of the time.

## Summary

* A lending company might want a model that requires classifying healthy loans and non-healthy loans correctly most of the time:

  * healthy loans being identified as a non-healthy loan might be more costly for a lending company since it might cause the loss of customers.

  * non-healthy loans being identified as a healthy loan might also be more costly for a lending company due to the loss of funds being provided by the lender.

  * The lending company would most likely want fewer False Positives due to the high possibility of a lender loosing provided funds when classifying non-healthy loans as healthy. The data below is shown in the confusion matrices which indicates how many healthy/non-healthy loans the model predicted correctly/incorrectly.

    * 56 (FALSE POSITIVES) --> The actual value is healthy and the predicted value is non-healthy

    * 102 (FALSE NEGATIVES) --> The actual value is non-healthy and the predicted value is healthy
