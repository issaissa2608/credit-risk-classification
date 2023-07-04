# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


Through this analysis I used logical regression models to identify creditworthiness of borrowers from a peer-to-peer lending service. This dataset included fields loan size, interest rate borrower income, debt to income, number of accounts, derogatory marks and total debt. I used this to predict if a loan was either healthy or high risk. To analysis this data, I started by separating labels and features into x and y variables. Then I used sklearn to split the data into training and testing datasets using train_test_split module. Using this I created model 1 (results below). Due to the imbalance in the data, I resampled the data. This used to create model 2. Then I was able to compare the two models and analysis which would provide the better results.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
Accuracy: 99%
Healthy Loans
Precision: 1
Recall: 0.99
High-Risk loans
Precision: 0.85
Recall: 0.91


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  Accuracy: 99%
Healthy Loans
Precision: 1
Recall: 0.99
High-Risk loans
Precision: 0.84
Recall: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )


Overall, both models perform well when predicting healthy loans. The second model, using resample data, increased the recall of the high-risk loans. However, this precision has not changed. I would recommend the use of second model as it has high rate of return for high risk loans. As miscalculating high risk loan is more of a risk it would be better to go with better accuracy for high risk over healthy loan.

