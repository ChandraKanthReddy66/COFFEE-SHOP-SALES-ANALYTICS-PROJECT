☕ Coffee Shop Sales Analytics

Project Overview

Coffee Shop Sales Analytics is a Power BI project created to analyze coffee shop sales performance using POS transaction data.

The project covers 149,116 transactions, 3 store locations, and 80 products from January 2023 to June 2023.

Project Objectives
Analyze Total Sales
Analyze Total Orders
Calculate Average Order Value
Track MoM, QoQ and YoY Growth
Identify top-selling products
Analyze product category performance
Compare store performance
Identify peak sales hours and day patterns
Track performance against the 10% growth target
Data Source

Source: POS Transaction System

Format: Excel / CSV

Main Tables:

Transactions
Dim_Products
Dim_Stores
dim_date
Data Preparation

Folder Connection → Power Query → Data Transformation → Data Model

Power Query was used to prepare and transform the source data before loading it into Power BI.

Data Model

The project uses a Star Schema.

Fact Table: Transactions

Dimension Tables: Dim_Products, Dim_Stores, dim_date

The Transactions table contains transaction-level information such as transaction ID, date, quantity, price, product ID and store ID.

DAX

DAX was used to create business calculations and KPIs.

Important measures include:

Total Sales
Total Orders
Average Order Value
MoM Growth
QoQ Growth
YoY Growth
YTD Sales
Rolling 3M Sales
Rolling 6M Sales
Sales Target

The project specification contains 34 DAX measures.

Dashboard Pages
1. Executive Overview

Provides a high-level business summary using:

Total Sales
Total Orders
Average Order Value
YoY Growth
Sales YTD
Monthly Sales Trend
Sales by Product Category
Sales vs Target Gauge
2. Sales Trend Analysis

Focuses on:

MoM Growth
QoQ Growth
YoY Growth
Cumulative Sales
Current Year vs Prior Year
Quarterly Analysis
Rolling Sales
3. Product Performance

Analyzes:

Top 10 Products
Sales by Category
Category Sales by Store
Product Scorecard
Sales Contribution
Growth Status
4. Store & Time Intelligence

Analyzes:

Store Performance
Peak Sales Hour
Average Daily Sales
Sales WTD
Sales by Day and Hour
Daily Sales Trend
Orders vs Average Order Value
Filters

The dashboard includes:

Year
Quarter
Month
Store Location
Product Category
