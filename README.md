# sales-Bi-Dashboard
📊 Sales Performance Dashboard | Power BI
📌 Project Overview

This project is an interactive Sales Performance Dashboard built using Microsoft Power BI.
It provides a comprehensive analysis of Sales vs Budget, Customer Performance, and Product Performance across different years, months, and cities.
The dashboard is designed using a star schema data model and supports dynamic filtering for deeper business insights.

🎯 Business Objectives
Track actual sales vs budget
Identify top-performing customers and products
Analyze monthly and yearly sales trends
Understand regional (city-wise) sales distribution
Enable data-driven decision-making for stakeholders

🗂️ Dataset Description
Fact Tables
FACT_InternetSales
SalesAmount
OrderDateKey
CustomerKey
ProductKey
FACT_Budget
Date
Monthly Budget
Dimension Tables
DIM_Calendar
Date, Month, Quarter, Year
DIM_Customers
Customer Name, Gender, City
DIM_Products
Product Name, Category, Sub-Category

🧩 Data Model
Star Schema design
One-to-many relationships:
Calendar → Sales & Budget
Customers → Sales
Products → Sales
Calendar table marked as Date Table
This structure ensures high performance and accurate DAX calculations.

📈 Report Pages & Features

1️⃣ Sales Overview
KPI: Sales vs Budget
Sales variance with conditional indicators
Top 10 Customers & Products
Category-wise sales distribution
Monthly sales vs budget trend
City-wise sales map

2️⃣ Customer Details
Total Sales & Budget KPIs
Top customers by sales
Customer-wise monthly sales matrix
Sales by customer city (map)
Interactive slicers for filtering

3️⃣ Product Details
Product-wise sales performance
Top 10 products
Product category analysis
Monthly product sales matrix
Regional sales impact

📐 Key DAX Measures
Total Sales = SUM(FACT_InternetSales[SalesAmount])

Total Budget = SUM(FACT_Budget[Budget])

Sales Variance = [Total Sales] - [Total Budget]

Variance % = DIVIDE([Sales Variance], [Total Budget])

🎛️ Filters & Interactivity
Year
Month
Customer City
Product Category
Sub-Category
Product Name
All visuals are cross-filtered for seamless exploration.

🛠️ Tools & Technologies
Microsoft Power BI
DAX
Power Query
Data Modeling (Star Schema)

📊 Key Insights
Sales performance varies significantly across cities and products
Certain top customers contribute a large portion of total revenue
Budget targets were not met in some periods, highlighting improvement areas
Monthly trends help identify peak and low-performing periods

🚀 Future Enhancements
Year-over-Year (YoY) growth analysis
Profit & margin calculations
Tooltip pages for detailed insights
Forecasting using Power BI analytics

