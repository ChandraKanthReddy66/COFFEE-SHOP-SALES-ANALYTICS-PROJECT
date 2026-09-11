☕ Coffee Shop Sales Analytics

📌 Project Overview
Coffee Shop Sales Analytics is a Microsoft Power BI project created to analyze coffee shop sales data and provide useful business insights through an interactive dashboard.
The project uses POS (Point of Sale) transaction data covering January 2023 to June 2023, with:
•	🧾 149,116 Transactions 
•	🏪 3 Store Locations 
•	☕ 80 Products 
•	📂 5 Product Categories 
•	📊 4 Power BI Report Pages 
The dashboard helps managers understand overall sales performance, product contribution, store performance, growth trends, and sales patterns by day and hour. 
________________________________________________________________________________________________________________________________________________________________
🎯 Project Objectives
The main objectives of this project are:
•	💰 Analyze Total Sales 
•	🧾 Track Total Orders 
•	🛒 Calculate Average Order Value 
•	📈 Analyze Month-over-Month (MoM) Growth 
•	📊 Analyze Quarter-over-Quarter (QoQ) Growth 
•	📅 Analyze Year-over-Year (YoY) Growth 
•	📆 Calculate YTD Sales 
•	🏆 Identify Top-Selling Products 
•	☕ Analyze Product Category Performance 
•	🏪 Compare Store Performance 
•	⏰ Identify Peak Sales Hours 
•	📅 Analyze Day-of-Week Sales Patterns 
•	🎯 Compare sales against a 10% growth target 
________________________________________________________________________________________________________________________________________________________________
🔄 Project Workflow
📂 Source Files
      ↓
📁 Folder Connection
      ↓
🔧 Power Query
      ↓
🧹 Data Transformation
      ↓
⭐ Star Schema
      ↓
🧮 DAX Measures
      ↓
📊 Power BI Dashboard
      ↓
☁️ Power BI Service
      ↓
🔌 On-Premises Data Gateway
      ↓
🔄 Dataset Refresh
________________________________________________________________________________________________________________________________________________________________
📂 Data Source
The project uses data from a POS (Point of Sale) transaction system.
The source data is available in Excel/CSV format.
Power BI is connected to the source files using a Folder connection, allowing the data to be processed and used for analysis.
Main Tables
🗂️ Table	📌 Type	📊 Purpose
🧾 Transactions	Fact	Transaction-level sales data
☕ Dim_Products	Dimension	Product and category information
🏪 Dim_Stores	Dimension	Store information
📅 dim_date	Dimension	Date and time analysis
The Transactions table contains fields such as transaction ID, transaction date/time, quantity, unit price, store ID and product ID. 
________________________________________________________________________________________________________________________________________________________________
🔧 Power Query
Power Query is used for data preparation and transformation before loading the data into the Power BI model.
Process
📁 Folder
   ↓
📥 Get Data
   ↓
🔗 Combine Files
   ↓
🔧 Transform Data
   ↓
🧹 Clean / Prepare Data
   ↓
📊 Load to Model
This creates a structured dataset that can be used for reporting and analysis.
________________________________________________________________________________________________________________________________________________________________
⭐ Data Model
The project uses a Star Schema.
                 📅 dim_date
                     │
                     │
                     ▼
☕ Dim_Products ──► 🧾 TRANSACTIONS ◄── 🏪 Dim_Stores
                                                   FACT TABLE
🧾 Fact Table
Transactions is the main fact table because it contains the transaction-level business data.
📅 Dimension Tables
•	📅 dim_date → Date and time analysis 
•	☕ Dim_Products → Product, category and product type 
•	🏪 Dim_Stores → Store location information 
This model supports efficient reporting and time-based analysis. 
________________________________________________________________________________________________________________________________________________________________
🧮 DAX
DAX stands for Data Analysis Expressions.
DAX is used to create calculations and business measures in Power BI.
Important Measures
💰 Total Sales
🧾 Total Orders
🛒 Average Order Value
📈 MoM Growth %
📊 QoQ Growth %
📅 YoY Growth %
📆 YTD Sales
🔄 Rolling 3M Sales
🔄 Rolling 6M Sales
🎯 Sales Target
The project specification includes a centralized measures table with 34 DAX measures. 
________________________________________________________________________________________________________________________________________________________________
📊 Dashboard Pages
1️⃣ Executive Overview
The Executive Overview provides a quick snapshot of the overall business.
Main KPIs
•	💰 Total Sales 
•	🧾 Total Orders 
•	🛒 Average Order Value 
•	📈 YoY Growth % 
•	📆 Sales YTD 
Visuals
•	📈 Monthly Sales Trend 
•	📊 Sales by Product Category 
•	🎯 Sales vs Target Gauge 
•	📋 KPI Summary 
The page is designed to help management quickly understand overall business performance. 
________________________________________________________________________________________________________________________________________________________________
2️⃣ Sales Trend Analysis
This page focuses on sales growth and time-based performance.
KPIs
•	📈 MoM Growth % 
•	📊 QoQ Growth % 
•	📅 YoY Growth % 
•	🔄 Rolling 3M Sales 
•	🔄 Rolling 6M Sales 
Visuals
•	📈 Cumulative Sales 
•	📊 MoM Growth by Month 
•	🔀 Current Year vs Prior Year 
•	📋 Quarterly Breakdown 
This page helps identify growth momentum and sales patterns over time. 
________________________________________________________________________________________________________________________
3️⃣ Product Performance
This page analyzes products and categories.
Main Analysis
•	🏆 Top 10 Products 
•	🌳 Sales by Category 
•	🏪 Category Sales by Store 
•	📋 Product Scorecard 
•	📈 Sales Contribution % 
•	🔥 Growth Status 
This helps identify the products and categories that contribute most to revenue. 
________________________________________________________________________________________________________________________
4️⃣ Store & Time Intelligence
This page focuses on store comparison and sales timing.
KPIs
•	🏪 Store Rank 
•	⏰ Peak Hour 
•	📆 Average Daily Sales 
•	📅 Sales WTD 
•	🔢 Store Count 
Visuals
•	🏪 Store Performance Comparison 
•	🌡️ Sales Heat Map 
•	📈 Daily Sales Trend by Store 
•	⭕ Orders vs Average Order Value 
The heat map analyzes sales by day of week and hour of day, helping identify peak selling periods. 
________________________________________________________________________________________________________________________
🎛️ Filters & Slicers
The dashboard includes interactive filters that allow users to analyze specific parts of the business.
Available Filters
•	📅 Year 
•	📆 Quarter 
•	🗓️ Month 
•	🏪 Store Location 
•	☕ Product Category 
When a user selects a slicer, the report visuals update based on the selected filter context.

