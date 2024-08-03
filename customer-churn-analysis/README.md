# Introduction
This report provides an analysis of customer churn for a telecommunications company Telco, focusing on understanding the factors that influence customer retention and developing strategies to reduce churn. The analysis is based on data visualization and insights derived from Power BI.

In the context of a telecommunications company, "churn" refers to the rate at which customers discontinue or cancel their services with the company during a specific period. Customer churn is a critical metric for telecommunications companies, as it directly impacts their revenue and growth. High churn rates can be indicative of customer dissatisfaction, poor service quality, pricing issues, or increased competition. Understanding churn and the factors influencing it is essential for these companies to devise strategies to improve customer retention, enhance service offerings, and maintain a strong customer base.

# Dataset
The [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/ylchang/telco-customer-churn-1113) contains information about the customer data for Telco in a quarter, including customers' demographics, location, account information and services that each customer has signed up for.

# Data Preparation
I imported these 5 data files into Microsoft PowerBI and made sure the relationships among them are available and correct. 

At the first glance, the data is well organized and the data types are automatically revised to the correct form. A few adjustments needed and I did as follow:
- For Demographics table, create 'Age Category' column to categorize customers into 'Under 30', 'Other' and 'Senior'.
- For Account Information table, use DAX to create measures 'Number of Customers', 'Number of Churned Customers' and 'Churn Rate'. Create 'CLTV Category' column following the CLTV catogorize principles.
- For Services table, change the data types of 'Monthly Charges', 'Total Charges', 'Total Refunds',	'Total Extra Data Charges',	'Total Long Distance Charges', 'Total Revenue' to 'Currency'.

# Key Insights
## Overview
- Key Metrics:
  - Customers: 7,043
  - Churned Customers: 1,869
  - Churn Rate: 26.54%
- Churn Cateroy: The top 2 categories for churn reason are competitors and attitude. 45% of the churned customers churned because of competitors.
- Churn Reason: The top 3 churn reaseons are 'Competitor had better devices', 'Competitor mad better offer' and 'Attitude of support person'.
- Only customers with Satisfaction score from 1-3 will churn and those with satisfaction score from 4-5 will not churn.
- Customers with a Customer Lifetime Value (CLTV) higher than 4000 have lower churn rates, which means Telco did a good job in retaining high lifetime value customers.

## Churn by Customer Demographics
- Senior customers (Age above 65) have a higher churn rate compared to non-senior customers.
- Gender does not have a significant impact on churn rates.
- Customers who live with dependents have a lower churn rate compared to customers who live alone. But the number of dependents they're living with does not have a significant impact on churn rates.

## Churn by Services
- Customers using fiber optic internet services have a higher churn rate compared to those using cable, DSL or no internet service.
- Customers using unlimited data plan are more likely to churn than those without a unlimited data plan, especially when thir average monthly data consumption is less than 25 GB.

## Churn by Payment Method
- Customers paying by credit card have a lower churn rate compared to bank withdrawal and mailed check.
- Customers with offer A have a lower churn rate of 6.73%, with offer E have a higher churn rate of 52.92%.
- Customers with yearly contract are less likely to churn than with monthly contract.
- 
# Recommendations
- Competitive Pricing: Offering better deals and competitive pricing could address the 20.70% churn due to competitors.
- Improve Customer Support: Addressing issues related to support staff's attitude could reduce churn by 14.55%.
- Targeted Campaigns: Develop tailored retention strategies for younger customers, considering their unique preferences and needs.
- Offers and Services: Create targeted offers and services that address the needs of younger customers without partners or dependents, possibly through bundle packages or personalized plans.
- Enhance Service Reliability: Focusing on network reliability and reducing dissatisfaction could help retain 4.76% of customers.
- Payment Methods: Encourage the use of credit card payments and explore ways to improve the electronic check payment process to reduce churn.
Long-Term Contracts: Offer incentives to encourage customers to commit to longer-term contracts, such as discounts or additional services.
- Tailored Offers: Providing customized offers based on customer segments can help reduce churn related to competitors' offers.






