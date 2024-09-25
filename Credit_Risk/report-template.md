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

Description of Logistic Regression Model Accuracy

Precision Scores
- Healthy Loans (Label '0'): The precision score is a perfect 100%.
- High-Risk Loans (Label '1'): The precision score stands at 87%.

Recall Scores
- Healthy Loans (Label '0'): The recall score is also 100%, indicating flawless identification of healthy loans.
- High-Risk Loans (Label '1'): The recall for high-risk loans is 95%, demonstrating strong performance in recognizing high-risk loans.

Overall, the model effectively distinguishes between healthy and high-risk loans, showcasing its reliability and accuracy.

## Summary

Summary of Machine Learning Model Results

Model Performance Overview

The logistic regression model demonstrates strong performance in predicting healthy loans (class 0), achieving:
- Precision: 1.00
- Recall: 0.99

For risky loans (class 1), the model also performs well, with:
- Precision: 0.87
- Recall: 0.95

Analysis of Performance

The disparity in performance metrics, particularly for risky loans, can be attributed to the imbalanced nature of the dataset. The support for class 1 (risky loans) is significantly lower, with only 625 instances compared to 18,759 for class 0 (healthy loans). This imbalance limits the model's ability to learn effectively from high-risk loan data, indicating potential areas for improvement.

Importance of Class Prediction

In the context of loan classification, it is crucial to prioritize the prediction of high-risk loans over healthy ones. The financial implications of a default on a single high-risk loan can be substantial, often outweighing the benefits gained from issuing multiple low-risk loans. Therefore, enhancing the model's ability to accurately identify risky loans is essential for minimizing potential losses.

Recommendation

Given the model's overall accuracy of over 95% in predicting loan repayment outcomes, I recommend using the logistic regression model for assessing borrower creditworthiness. Its high precision and recall for healthy loans make it a reliable tool for lenders. However, to further improve its effectiveness in identifying risky loans, consider augmenting the training dataset with additional examples of high-risk loans. This could help balance the dataset and enhance the model's predictive capabilities.
In conclusion, while the current model is effective, focusing on improving its performance on class 1 predictions will provide a more robust solution for managing financial risk in lending practices.
