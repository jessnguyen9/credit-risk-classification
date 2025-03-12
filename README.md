# Loan Risk Classification Using Logistic Regression

## Overview
Lenders need to determine whether a loan applicant is likely to default on a loan. This project builds a machine learning model using logistic regression to predict the risk level of loans. The goal is to classify loans as either "healthy" (low risk) or "high risk," helping financial institutions make informed lending decisions.

## Problem Statement
The dataset contains information about borrowers, such as loan size, interest rate, income, debt-to-income ratio, and credit history. However, there is a significant imbalance in the dataset:

- 75,036 loans are classified as low risk (0)

- 2,500 loans are classified as high risk (1)

This imbalance can lead to a model that favors predicting low-risk loans while failing to correctly identify high-risk ones. The project aims to:

1. Train an initial logistic regression model on the imbalanced data.

2. Improve performance by balancing the data using oversampling.

3. Compare the results to assess the impact of oversampling.
