# Walmart-Sales-Data-Analysis-Using-SQL
📍Project Overview

This project analyzes Walmart sales transaction data to uncover performance patterns across branches, product lines, customer types, and time periods. The goal is to translate raw transactional data into insights that support strategic sales decisions, revenue optimization, customer segmentation, and inventory planning.

The dataset is sourced from the Kaggle Walmart Sales Forecasting Competition, containing a structured record of purchases across three branches located in Mandalay, Yangon, and Naypyitaw. The analysis focuses on identifying sales trends, customer behavior, and profitability indicators using SQL.

🎯 Project Purpose

The primary objective of this project is to understand what factors influence sales performance across branches and product lines, enabling data-driven improvement opportunities. Key focus areas include:

Determining product lines that consistently perform well vs. those needing improvement

Identifying high-revenue periods, peak sales hours, and seasonal trends

Understanding customer segmentation and spending patterns

Calculating revenue, COGS, VAT, total billed amount, and gross margin performance

This project provides the foundation for sales forecasting, pricing strategy evaluation, and operational decision-making.

📂 Dataset Summary

Source: Kaggle Walmart Sales Forecasting Competition

Branches Covered: Mandalay, Yangon, Naypyitaw

Total Columns: 17

Total Rows: 1,000
| Column                  | Description                             |
| ----------------------- | --------------------------------------- |
| invoice_id              | Invoice reference for each transaction  |
| branch                  | Store branch where transaction occurred |
| city                    | Geographic location of the branch       |
| customer_type           | Customer classification (Member/Normal) |
| gender                  | Gender of purchasing customer           |
| product_line            | Product category purchased              |
| unit_price              | Price per unit of item                  |
| quantity                | Number of units sold                    |
| VAT                     | 5% taxation value applied               |
| total                   | Amount billed to customer (COGS + VAT)  |
| date / time             | When the purchase was made              |
| payment_method          | Mode of payment used                    |
| cogs                    | Cost of goods before tax                |
| gross_margin_percentage | Percentage profitability ratio          |
| gross_income            | Profit earned per transaction           |
| rating                  | Customer purchase satisfaction score    |

🔍 Analysis Scope

This project covers three major analysis tracks:

1️⃣ Product Analysis

Identify highest and lowest performing product lines

Analyze VAT contribution by product line

Evaluate gender-based purchase patterns

Flag performance status as "Good" or "Bad" based on average sales

2️⃣ Sales Performance Analysis

Sales trend by day of week, month, and time of day

Identify busiest operational periods

Compare revenue and COGS seasonality

Determine highest revenue-generating locations

3️⃣ Customer & Behavior Analysis

Customer segmentation by type, payment preference, and gender

Purchase frequency and high-value customer mapping

Determine rating distribution and customer experience by time & branch

⚙️ Methodology / Approach Used
🔧 Data Wrangling

Created database and structured tables for storage

Inserted data and enforced data quality (NOT NULL constraints)

Confirmed dataset contained no null values at insertion

📌 Feature Engineering

Additional fields were created to support analytical questioning:

time_of_day → Morning | Afternoon | Evening

day_name → Weekday name extracted from the date

month_name → Month associated with the transaction

These engineered columns allow deeper behavioral analysis such as peak operating time and branch rush patterns.

📈 Exploratory Data Analysis (EDA)

Conducted using SQL queries to answer defined business questions and measure:

Sales performance distribution

Product profitability ranking

Customer profile segmentation

Operational performance insights

❓ Key Business Questions Answered
General

How many unique cities exist in the data?

Which branches operate in each city?

Product

How many unique product lines are available?

Most common payment method?

Best-selling product line?

Total revenue by month & which month had the highest COGS?

City and product line with highest revenue / VAT contribution?

Product lines classified as “Good” or “Bad” performance?

Average rating per product line?

Sales

Sales count by time of day and weekday?

Customer type contributing the most revenue?

City with highest VAT rate?

Customer segment paying the highest VAT?

Customer

Unique customer types and payment structures?

Most common customer type and gender?

Gender distribution across branches?

Highest rating time-of-day and weekday?

📌 Conclusion

This project reveals critical insight into Walmart’s branch-level operations, including performance gaps, peak demand cycles, and customer behavior indicators. These findings contribute to potential improvements in:

Inventory planning

Customer service staffing

Marketing campaign targeting

Seasonal sales strategy

Revenue and profitability optimization
