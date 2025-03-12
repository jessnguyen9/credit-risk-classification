# Loan Risk Classification Using Logistic Regression

## Overview
This project focuses on predicting the risk level of loans using machine learning techniques. A logistic regression model is trained to determine whether a loan is healthy or high-risk based on various financial factors such as loan size, interest rate, borrower income, and debt-to-income ratio.

By leveraging data analytics and machine learning, this project provides a predictive model that helps classify loans as either safe or high-risk, improving decision-making processes.

## Data Used
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
### **Initial Model Performance**

1. **Accuracy Score:** 0.992

2. **Confusion Matrix**

[[22399 116]

[ 70 676]]

- True Negatives (TN): 22,339
- False Positives (FP): 116
- False Negatives (FN): 70
- True Positives (TP): 676

This confusion matrix shows that the model correctly identified **22,399 healthy loans** and **676 high-risk loans**, with minimal misclassifications.

3. **Classification Report**

| Class        | Precision | Recall | F1-Score | Support |
|--------------|-----------|--------|----------|---------|
| 0            | 1.00      | 0.99   | 1.00     | 22,515  |
| 1            | 0.85      | 0.91   | 0.88     | 746     |
| Accuracy     |           |        | 0.99     | 23,261  |
| Macro avg    | 0.93      | 0.95   | 0.94     | 23,261  |
| Weighted avg | 0.99      | 0.99   | 0.99     | 23,261  |

- The first logistic regression model achieved a 99.2% accuracy rate but had some difficulty identifying high-risk loans due to an imbalance in the dataset.

- The model misclassified some high-risk loans as safe, which could be problematic for lenders.

### **Improvement with Resampling**

1. **Accuracy Score:** 0.994

2. **Confusion Matrix**

[[22382   133]

[    4   742]]

- True Negatives (TN): 22,382
- False Positives (FP): 133
- False Negatives (FN): 4
- True Positives (TP): 742

With oversampling, the model improved its ability to correctly classify high-risk loans, reducing false negatives significantly.

3. **Classification Report**



- To address the imbalance, the dataset was resampled using a technique called Random Oversampling, ensuring an equal number of healthy and high-risk loans.

- The updated model improved the detection of high-risk loans, increasing recall (ability to correctly identify high-risk loans) from 91% to 99%.

- The final accuracy improved slightly to 99.4% with a better balance between detecting safe and risky loans.

## Business Impact
More Accurate Risk Assessment: Lenders can better identify high-risk loans, reducing financial losses.

Improved Decision-Making: Loan officers can use the insights from this model to refine approval criteria.

Enhanced Fairness: By addressing data imbalance, the model ensures fairer evaluations of loan applicants.

## Conclusion
This project demonstrates how data analytics and machine learning can help financial institutions make more informed decisions regarding loan approvals. By improving risk prediction accuracy, lenders can reduce defaults and maintain a healthier loan portfolio.
