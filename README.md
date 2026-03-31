## Project README

### 1. Project Goal:
This project aims to demonstrate the process of downloading a Kaggle dataset, implementing a custom linear regression model for binary classification, training it on stock market data, and evaluating its performance.

### 2. Data and Model:
The dataset used is the 'Stock Market Dataset' from Kaggle (`jacksoncrow/stock-market-dataset`). Specifically, `MSFT.csv` was utilized, with 'Open' and 'High' prices as features and a binary target ('Y' for Close price above median, 'N' otherwise). The `TangentLinearRegression` model, which internally uses `sklearn.linear_model.LinearRegression`, was employed for classification.

### 3. Key Findings:
- The model achieved an accuracy of approximately **0.8684** on the test set.
- It performed strongly in identifying class 'N' (stocks closing below median) with a precision of 0.79 and a recall of 1.00.
- For class 'Y' (stocks closing above median), the model showed high precision (1.00) but a relatively lower recall (0.74).

### 4. Next Steps & Recommendations:
- Consider using classification-specific algorithms like Logistic Regression for this binary classification task, as Linear Regression might not be optimally calibrated for probability predictions.
- Investigate the reasons for the lower recall in class 'Y' to understand specific challenges in identifying these instances. This could involve exploring additional features or techniques to address potential class imbalance.
