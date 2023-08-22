# credit_risk_classification
Module 20

# Credit Risk Analysis Report

## Overview of the Analysis

Analysis conducted to evaluate a trained model's suitablity to identify high-risk loans. High-risk being those loans where borrowers are identified as less suitable for credit due to their likelihood of defaulting on their obligations.

Historical lending data (77,536 records) was used which included the below list of features:

    * loan_size
    * interest_rate
    * borrower_income
    * debt_to_income
    * num_of_accounts
    * derogatory_marks
    * total_debt
    * loan_status

Using the Python machine learning library Scikit-Learn the original data was split into training and testing datasets using model_selection then a Logistic Regression Model applied to predict the 'loan_status' of the testing dataset. In the data and predictions '0' is a healthy loan and a '1' is a high-risk loan.

## Results

Logistic Regression Model:
  * Overall accuracy of the model was very good at an accuracy of 0.99
  * Overall prediction of a "Healthy Loan" was excellent
    * Precision 1.00
    * Recall 1.00
    * f1-score 1.00
  * Overall accuracy of predicting a "High-Risk Loan" was moderate
    * Precision 0.87
    * Recall 0.89
    * f1-score 0.88  

## Summary    

Overall accruacy is very high at 99%. 
Healthly loans are predicted at 100% accruacy, but high-risk loans are less than 90%. 
As high-risk loans (result value '1') are the ones most important to predict for creditworthiness of borrowers I would not recommend this model unless there was more data and/or features to increase the prediction accuracy of high-risk loans.