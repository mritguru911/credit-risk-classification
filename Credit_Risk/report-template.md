# Credit-Risk-Classification

## Overview of the Analysis

This analysis aims to develop a supervised machine learning model designed to predict whether a loan is classified as healthy (class 0) or high-risk (class 1). For this purpose, we will employ logistic regression as our binary classification method. The analysis utilizes financial data, specifically examining factors such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. Our goal is to determine the loan status—either a healthy loan (0) or a high-risk loan (1)—using information extracted from a CSV file containing 77,537 entries.

Machine Learning Process Steps
- The machine learning process for this analysis involved several key stages:
- Data Preparation: The dataset was divided into labels and features, where the loan status (healthy or high-risk) served as the label and the remaining seven columns represented the features.
- Data Splitting: The dataset was further partitioned into training and testing subsets.
- Model Creation: A Logistic Regression model from the sklearn library was established.
- Model Selection: Logistic regression was selected as the binary classifier since our task involves categorizing loans into two distinct classes: healthy or high-risk.
- Model Training: The model was trained using the training dataset.
- Making Predictions: Predictions were generated using the test dataset.
- Performance Evaluation: The effectiveness of the model was assessed through metrics such as accuracy, precision, and recall scores.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
Description of Logistic Regression Model Accuracy,
Precision Scores
- Healthy Loans (Label '0'): The precision score is a perfect 100%.
- High-Risk Loans (Label '1'): The precision score stands at 87%.

Recall Scores
- Healthy Loans (Label '0'): The recall score is also 100%, indicating flawless identification of healthy loans.
- High-Risk Loans (Label '1'): The recall for high-risk loans is 95%, demonstrating strong performance in recognizing high-risk loans.

Overall, the model effectively distinguishes between healthy and high-risk loans, showcasing its reliability and accuracy.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
