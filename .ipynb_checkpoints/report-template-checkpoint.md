# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
----The purpose of this analysis is to build a machine learning model to predict the loan status of financial transactions. In particular, the model aims to predict whether a loan is a "healthy" (0) or "high-risk" (1) loan based on the available financial information.
  
* Explain what financial information the data was on, and what you needed to predict.
  ----The dataset contains financial information related to loans, with the main focus on predicting the "loan_status." The "loan_status" is the target variable, which represents whether a loan is classified as "healthy" (0) or "high-risk" (1). This is a binary classification problem where the goal is to categorize loans into one of these two classes.
  
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
-----The lending_df DataFrame is used to hold the dataset, which includes features (independent variables) and the target variable.
The target variable loan_status is divided into "0" (healthy loans) and "1" (high-risk loans). We have used y.value_counts() to check the frequency of each loan status, which is crucial for understanding the class distribution.


* Describe the stages of the machine learning process you went through as part of this analysis.
---Data Loading and Preprocessing: The dataset is read from a CSV file, and the data is divided into features (X) and the target (y).
---Model Selection and Training: The Logistic Regression model is selected and trained on the training data.
---Model Evaluation: The trained model is used to make predictions on the testing data.
---Classification Report: A classification report is generated to provide more detailed metrics, including precision, recall, and F1-score for both "healthy" and "high-risk" loans.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
----Logistic Regression: A logistic regression model is used for binary classification.
---Metrics and Reporting: Evaluation of the model's performance includes the use of a confusion matrix.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.
a healthy loan (low-risk) is classified as a non-healthy loan (high-risk). **a non-healthy loan (high-risk) is classified as a healthy loan (low-risk).
## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
---To identify the best-performing model, assess accuracy, precision, recall, F1-score, and balanced accuracy. Consider the importance of correctly predicting both "0" and "1."

