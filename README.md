# Credit Card Customer Segmentation

## Business Context
This project aims to develop a customer segmentation to define marketing strategy. The dataset has information about 9000 credit card holders for the last 6 months.

## Project Overview
- Derived new KPI by using data manipulation methods.
- Checked the multi-collinearity using a heatmap.
- Standardized the data and applied PCA to get the optimal number of Principal Components.
- Used KMeans Clustering — Silhouette Score and Cluster Inertia Score were used to determine the optimal number of clusters.
- Profiling was done to draw insights for each cluster.

## Dataset Description
- **CUST_ID**: Credit card holder ID
- **BALANCE**: Monthly average balance (based on daily balance averages)
- **BALANCE_FREQUENCY**: Ratio of last 12 months with balance
- **PURCHASES**: Total purchase amount spent during the last 12 months
- **ONEOFF_PURCHASES**: Total amount of one-off purchases
- **INSTALLMENTS_PURCHASES**: Total amount of installment purchases
- **CASH_ADVANCE**: Total cash-advance amount
- **PURCHASES_FREQUENCY**: Frequency of purchases (Percent of months with at least one purchase)
- **ONEOFF_PURCHASES_FREQUENCY**: Frequency of one-off purchases
- **PURCHASES_INSTALLMENTS_FREQUENCY**: Frequency of installment purchases
- **CASH_ADVANCE_FREQUENCY**: Cash-Advance frequency
- **AVERAGE_PURCHASE_TRX**: Average amount per purchase transaction
- **CASH_ADVANCE_TRX**: Average amount per cash-advance transaction
- **PURCHASES_TRX**: Average amount per purchase transaction
- **CREDIT_LIMIT**: Credit limit
- **PAYMENTS**: Total payments (due amount paid by the customer to decrease their statement balance) in the period
- **MINIMUM_PAYMENTS**: Total minimum payments due in the period
- **PRC_FULL_PAYMENT**: Percentage of months with full payment of the due statement balance
- **TENURE**: Number of months as a customer

## Final Clusters and Recommendations
Based on the **silhouette score**, I have chosen the number of clusters to be 4.

### Suggested Marketing Strategy for Each Cluster:
![Picture5_clusters_plot](https://github.com/user-attachments/assets/ea7cec3e-e331-4db5-8044-77ba74de7d2d)



#### **Group 0**
- Potential target customers who pay their bills, make purchases, and maintain a good credit score.
- Recommendations:
  - Increase credit limit or lower the interest rate.
  - Promote premium cards/loyalty cards to increase transactions.

#### **Group 1**
- Customers who take the maximum cash advances.
- Recommendations:
  - Send reminders for payments.
  - Provide offers for early payments to improve the payment rate.

#### **Group 2**
- Best performing group, maintaining the highest monthly average purchases.
- Recommendations:
  - Offer reward points to increase their purchases.

#### **Group 3**
- Customers making the maximum one-off payments (likely for bills).
- Recommendations:
  - Offer discounts or promotions for the next transaction upon full payment.
