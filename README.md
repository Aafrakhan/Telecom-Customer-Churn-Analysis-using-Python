# 📊 Telecom Customer Churn Analysis 

## 📌 Project Overview

This project performs an Exploratory Data Analysis (EDA) on customer churn data to identify the factors that are most strongly associated with customer churn.
The analysis focuses on factors such as contract type, tenure, payment method, internet service, additional services, and demographic attributes to understand customer behaviour and identify opportunities for improving customer retention.

🎯 Objective

The main objectives of this project are to:

- Understand the overall customer churn rate.
- Identify customer segments with higher churn.
- Analyse the relationship between churn and contract type.
- Study the impact of customer tenure on churn.
- Analyse churn based on payment methods.
- Explore the relationship between internet services and churn.
- Evaluate the effect of additional services such as Online Security, Online Backup, Device Protection, and Tech Support.
- Analyse churn across demographic groups.
- Generate actionable insights and retention recommendations.

📂 Dataset

Telecom dataset contains 7,043 customer records and 21 columns.

Key Features

Feature| Description
"customerID"| Unique customer identifier
"gender"| Customer gender
"SeniorCitizen"| Indicates whether the customer is a senior citizen
"Partner"| Whether the customer has a partner
"Dependents"| Whether the customer has dependents
"tenure"| Number of months the customer has stayed
"PhoneService"| Phone service subscription
"MultipleLines"| Multiple phone lines subscription
"InternetService"| Type of internet service
"OnlineSecurity"| Online security subscription
"OnlineBackup"| Online backup subscription
"DeviceProtection"| Device protection subscription
"TechSupport"| Technical support subscription
"StreamingTV"| Streaming TV subscription
"StreamingMovies"| Streaming movie subscription
"Contract"| Contract duration
"PaperlessBilling"| Paperless billing status
"PaymentMethod"| Customer payment method
"MonthlyCharges"| Monthly customer charges
"TotalCharges"| Total customer charges
"Churn"| Whether the customer left the service

🛠️ Technologies & Libraries

- Python
- Pandas — Data manipulation and analysis
- NumPy — Numerical operations
- Matplotlib — Data visualisation
- Seaborn — Statistical visualisation
- Jupyter Notebook — Analysis environment

The notebook imports Pandas, NumPy, Matplotlib, and Seaborn for the analysis.

🔍 Project Workflow

1. Data Loading

The customer churn dataset was imported into a Pandas DataFrame.

2. Data Inspection

Initial inspection was performed using:

- "df.shape"
- "df.info()"
- "df.describe()"
- "df.isnull().sum()"
- Duplicate checks

The dataset initially contained "TotalCharges" as an object data type.

3. Data Cleaning

The following cleaning steps were performed:

- Replaced blank values in "TotalCharges" with "0".
- Converted "TotalCharges" from "object" to "float".
- Checked for missing values.
- Checked for duplicate records.
- Checked for duplicate customer IDs.
- Converted the "SeniorCitizen" indicator from "0/1" into a more readable Yes/No representation.

After conversion, "TotalCharges" was stored as a numerical "float64" column.

4. Exploratory Data Analysis

Different visualisation techniques were used to understand customer churn patterns, including:

- Count plots
- Bar charts
- Stacked percentage charts
- Pie charts
- Subplots
- Comparative churn visualisations


📈 Key Analysis & Insights

📄 Contract Type

Customers with month-to-month contracts are more likely to churn compared with customers having one-year or two-year contracts.

Insight: Longer contractual commitment is associated with better customer retention.


⏳ Customer Tenure

Customers with short tenure, particularly around the first 1–2 months, show substantially higher churn.

Insight: The early customer lifecycle is an important period for retention efforts.


💳 Payment Method

Customers using electronic checks show higher churn compared with other payment methods.

Insight: Payment method is strongly associated with customer churn and may also indicate differences in customer engagement.


🌐 Internet Service

Fiber optic customers show considerably higher churn than DSL and customers without internet service.

Insight: The company should investigate potential pricing, service-quality, or customer-experience issues among fiber optic users.


🛡️ Additional Services

Customers without services such as:

- Online Security
- Online Backup
- Device Protection
- Tech Support

show noticeably higher churn than customers who subscribe to these services.

Insight: Additional services may be associated with stronger customer engagement and retention.


👵 Senior Citizens

A comparatively higher percentage of senior citizens have churned compared with non-senior customers.

Insight: Senior customers could benefit from targeted support and retention initiatives.


👥 Demographics & Streaming Services

The analysis indicates that gender and streaming service usage have little to no predictive power for churn, compared with factors such as contract type, tenure, payment method, and service subscriptions.


📊 Overall Findings

The analysis found that 26.54% of customers have churned.

The strongest churn-associated factors identified in the analysis are:

- Month-to-month contracts
- Short customer tenure
- Electronic check payments
- Fiber optic internet service
- Lack of additional support/security services
- Senior citizen customer segment

In contrast, customers with longer tenure, longer-term contracts, and support/security add-ons are more likely to remain customers.

📊 Visualisations

The project uses multiple visualisation techniques to communicate insights, including:

- Customer churn distribution
- Churn by contract type
- Churn by payment method
- Churn by senior citizen status
- Churn by internet service
- Churn by additional services
- Stacked percentage charts
- Pie charts
- Subplots for categorical comparisons

🎓 Skills Demonstrated

This project demonstrates practical skills in:

- Data Cleaning
- Exploratory Data Analysis
- Data Preprocessing
- Missing Value Handling
- Data Type Conversion
- Duplicate Detection
- Categorical Data Analysis
- Statistical Analysis
- Data Visualisation
- Business Insight Generation
- Customer Retention Analysis


📌 Conclusion

This EDA demonstrates that customer churn is not evenly distributed across the customer base. Contract commitment, early tenure, payment method, internet service, additional services, and senior-citizen status are among the key factors associated with churn.

The analysis provides actionable insights that can help a business identify high-risk customer segments and design targeted retention strategies rather than applying the same approach to every customer.
