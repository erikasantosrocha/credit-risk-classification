# Credit Risk Classification
Use various techniques to train and evaluate a model based on loan risk. A dataset of historical lending activity from a peer-to-peer lending services company is used to build a model that can identify the creditworthiness of borrowers.

Steps:
- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Write a Credit Risk Analysis Report

# Report

## Overview of the Analysis

The purpose of this analysis was to develop and assess a machine learning model utilizing a logistic regression classification algorithm to predict credit risk. Specifically, the objective was to classify loans as either "healthy" (low risk) or "high risk" based on historical lending activity. Logistic regression was chosen as the primary algorithm for this analysis because it is well-suited for binary classification tasks and provides probabilities for class membership. By leveraging this model, we aim to enhance our ability to identify and differentiate between low-risk and high-risk loans, thereby improving decision-making in credit risk management.


### Data Attributes (77,536 data entries)
* `loan size` : The amount of money borrowed.
* `interest_rate` : The percentage of the loan charged as interest to the borrower.
* `borrower_income` : The annual income of the borrower.
* `debt_to_income` : The ratio of a borrower's total debt payments to their gross income.
* `num_of_accounts` : The number of credit accounts the borrower has.
* `derogatory_marks` : Negative entries on the borrower's credit report, such as late payments or bankruptcies.
* `total_debt`: The total amount of debt the borrower owes.
* `loan_status`: The outcome of the loan, categorized as either "healthy" (low risk) or "high risk".

### ML Process
1. Data loading and exploration
2. Data split into training and testing sets
3. Train the model
4. Fit the model
5. Test the model
6. Evaluate the accurace of the model

## Results
    * Logistic Regression Machine Learning Model:
*                          precision    recall  f1-score   support
        Healthy Loan         1.00      0.99      1.00     18765
        High-risk Loan       0.85      0.91      0.88       619

        accuracy                               0.99     19384
        macro avg          0.92      0.95      0.94     19384
        weighted avg       0.99      0.99      0.99     19384

## Summary

The logistic regression model demonstrated exceptional performance in predicting healthy loans, with a precision of 1.00 and a recall of 0.99. It also performed well in predicting high-risk loans, achieving a precision of 0.85 and a recall of 0.91. Overall, the model attained an accuracy of 99%, indicating a high level of correctness in its predictions.

Given these results, it is recommended to use this machine learning model to predict credit risk. While it is important to accurately predict the behavior of both healthy and high-risk borrowers, predicting high-risk loans (i.e., the 1's) is particularly crucial. By identifying high-risk borrowers, the bank can pay special attention to them when providing new loans or increasing their loan amounts, thus better managing credit risk.
