# CREDIT-CARD-CUSTOMER-SEGMENTATION

Business Context: This project aims to develop a customer segmentation to define marketing strategy. The dataset has about 9000 credit card holders information for last 6 months.

Project Overview
Derived new KPI by using data manipulation methods.
Checked the multi-collinearity using heatmap.
Standardized the data and applyied PCA to get optimal number of Pricipal Components.
KMeans Clustering is used - Silhotte Score and Cluster Inertia Score used to fix the number of clusters.
Done profiling to draw insights for the clusters.
Dataset Description
CUST_ID: Credit card holder ID
BALANCE: Monthly average balance (based on daily balance averages)
BALANCE_FREQUENCY: Ratio of last 12 months with balance
PURCHASES: Total purchase amount spent during last 12 months
ONEOFF_PURCHASES: Total amount of one-off purchases
INSTALLMENTS_PURCHASES: Total amount of installment purchases
CASH_ADVANCE: Total cash-advance amount
PURCHASES_FREQUENCY: Frequency of purchases (Percent of months with at least one purchase)
ONEOFF_PURCHASES_FREQUENCY: Frequency of one-off-purchases
PURCHASES_INSTALLMENTS_FREQUENCY: Frequency of installment purchases
CASH_ADVANCE_FREQUENCY: Cash-Advance frequency
AVERAGE_PURCHASE_TRX: Average amount per purchase transaction
CASH_ADVANCE_TRX: Average amount per cash-advance transaction
PURCHASES_TRX: Average amount per purchase transaction
CREDIT_LIMIT: Credit limit
PAYMENTS: Total payments (due amount paid by the customer to decrease their statement balance) in the period
MINIMUM_PAYMENTS: Total minimum payments due in the period.
PRC_FULL_PAYMEN: Percentage of months with full payment of the due statement balance
TENURE: Number of months as a customer
Final Clusters and Recommendations
Based on silhouette_score, i have taken number of clusters to be 4.


Suggested Marketing Strategy for these clusters:
Group 0

They are potential target customers who are paying bills and doing purchases and maintaining comparatively good credit score. So we can increase credit limit or can lower down interest rate. Promote premium cards/loyality cards to increase transcations.
Group 1

These customers are taking maximum cash advance, these customers should be given remainders for payments. Offers can be provided on early payments to improve their payment rate.
Group 2

This is performing best among all the clusters are maintaining highest monthly average purchases. Giving any reward points might increase their purchases.
Group 3

This group is doing maximum oneoff payments(may be for bills only). Customers of this group can be offered discount/offer on next transactions upon full payment.
