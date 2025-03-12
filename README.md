# Loan Risk Classification Using Logistic Regression

## Overview
This project focuses on predicting the risk level of loans using machine learning techniques. A logistic regression model is trained to determine whether a loan is healthy or high-risk based on various financial factors such as loan size, interest rate, borrower income, and debt-to-income ratio.

By leveraging data analytics and machine learning, this project provides a predictive model that helps classify loans as either safe or high-risk, improving decision-making processes.

## Problem Statement
The dataset contains loan records with key financial metrics, including:

Loan Size – The amount borrowed by an individual.

Interest Rate – The percentage charged for borrowing.

Borrower Income – The borrower's annual income.

Debt-to-Income Ratio – A measure of financial health.

Number of Accounts – The number of financial accounts a borrower has.

Derogatory Marks – Indicators of past financial delinquencies.

Total Debt – The borrower’s outstanding debt.

Loan Status – The classification of a loan as healthy (0) or high-risk (1).

## Key Findings
1. **Initial Model Performance**
- The first logistic regression model achieved a 99.2% accuracy rate but had some difficulty identifying high-risk loans due to an imbalance in the dataset.

- The model misclassified some high-risk loans as safe, which could be problematic for lenders.

2. **Improvement with Resampling**
- To address the imbalance, the dataset was resampled using a technique called Random Oversampling, ensuring an equal number of healthy and high-risk loans.

- The updated model improved the detection of high-risk loans, increasing recall (ability to correctly identify high-risk loans) from 91% to 99%.

- The final accuracy improved slightly to 99.4% with a better balance between detecting safe and risky loans.
