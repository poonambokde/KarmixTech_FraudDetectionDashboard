# KarmixTech_FraudDetectionDashboard
"Fraud Detection &amp; Risk Analytics Dashboard - Karmix Tech Internship Project"
# Fraud Detection & Risk Analytics Dashboard


Fraud Detection & Risk Analytics Dashboard

Karmix Tech Data Analytics Internship — Project 1

Business Problem

Credit card fraud causes direct financial loss and erodes customer trust. With fraud cases making up a tiny fraction of total transactions, the challenge is to detect patterns in when and how fraud happens so risk teams can act proactively instead of reactively.

Dataset


Source: Kaggle — Credit Card Fraud Detection dataset
Size: 284,807 transactions, 31 columns (anonymized PCA features V1–V28, Time, Amount, Class)
Highly imbalanced: only 492 transactions (0.17%) are fraudulent


Tools Used


Python (Pandas, NumPy, Matplotlib, Seaborn) — EDA and feature engineering
Power BI — interactive dashboard and DAX measures


Approach


Loaded and explored the raw transaction data, checked class imbalance and amount distribution
Engineered two new features: Hour (extracted from Time) and Risk_Level (Low/Medium/High based on transaction amount), plus Txn_Size bucket
Exported a clean, dashboard-ready CSV
Built a Power BI dashboard with KPI cards, risk distribution, fraud vs legit split, transaction-size breakdown, and an hourly fraud trend


Key Insights


Fraud rate is only 0.17%, confirming a highly imbalanced dataset
73.6% of fraud cases occur in Low Risk (small amount) transactions — fraudsters favor small, less-scrutinized charges
Peak fraud hours are 2 AM (57 cases) and 11 AM (53 cases)
Average fraud amount: $122.21 | Total fraud amount: $60.13K


Recommendations


Implement real-time alerts during peak fraud hours (2 AM, 11 AM)
Monitor small-amount transactions more closely, since they are disproportionately used for fraud
Treat amount-based risk scoring as a weak signal — combine it with time-of-day patterns for better detection


Files in this Repository


creditcard.csv — raw dataset
Fraud_Detection_EDA.ipynb — Python EDA and feature engineering notebook
Fraud_Detection___Risk_Analysis_Dashboard.pbix — Power BI dashboard
dashboard_screenshot.png — dashboard preview
