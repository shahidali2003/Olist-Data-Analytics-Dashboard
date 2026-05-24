🚀 Olist E-Commerce Analytics | Power BI + PostgreSQL + Live Gateway Integration
📌 Project Overview

This project is a complete end-to-end Business Intelligence & Analytics solution built using Power BI, PostgreSQL, SQL, DAX, and Power BI Gateway.

The dashboard analyzes large-scale e-commerce sales data and provides deep insights into:

Revenue performance
Customer behavior
Product & category analytics
Delivery & logistics
Seller performance
Payment analysis
Customer reviews & ratings
KPI monitoring
Year-over-Year growth trends

The project is designed with a real-world BI architecture approach using:

SQL Views
Star Schema Modeling
Dynamic Date Table
DAX Measures
Direct Query
Live Data Refresh
On-Premises Gateway Integration
🛠️ Tech Stack
Technology	Usage
Power BI	Dashboarding & Visualization
PostgreSQL	Data Warehouse / Storage
SQL	Data Cleaning, Views, Query Optimization
DAX	KPIs, Measures, Time Intelligence
Power BI Gateway	Live Refresh & Cloud Sync
Direct Query	Real-Time Data Access
Power BI Service	Cloud Publishing & Refresh

📂 Project Architecture
Raw Dataset
    ↓
PostgreSQL Database
    ↓
SQL Views & Transformations
    ↓
Power BI Direct Query
    ↓
DAX Measures + Date Table
    ↓
Interactive Dashboards
    ↓
Power BI Service
    ↓
On-Premises Gateway
    ↓
Live Refresh & Cloud Analytics


🗄️ Database Engineering
PostgreSQL Database
Database Name:
Olist_DB
Key SQL Work Done
Created optimized SQL Views
Handled 200,000+ data rows
Reduced transformation load from Power BI
Implemented analytical layer using SQL
Structured data for faster visualization rendering
Views Created
bi_fact_sales
bi_fact_order
bi_fact_review_latest
bi_payments_order
bi_dim_product
📊 Data Modeling

Implemented a clean analytical model using:

Fact Tables
Dimension Tables
Star Schema Concepts
Relationships
Time Intelligence Model
Date Table

Custom Date Table created using DAX for:

YTD Analysis
Monthly Trends
Quarterly Analysis
Year-over-Year KPIs

Example:

DimDate =
ADDCOLUMNS (
    CALENDAR ( DATE(2017,1,1), DATE(2018,12,31) ),
    "Month", FORMAT([Date], "MMMM"),
    "Month No", MONTH([Date]),
    "Quarter", "Q" & FORMAT([Date], "Q")
)
⚡ Direct Query Implementation

Used Direct Query Mode instead of Import Mode to achieve:

Near Real-Time Reporting
Live Database Connectivity
Reduced PBIX Size
Dynamic Data Refresh
Scalable BI Architecture
🔄 Live Gateway Integration

Configured:

Power BI On-Premises Data Gateway
PostgreSQL Cloud Connection
Scheduled Refresh
Live Synchronization Between:
PostgreSQL
Power BI Service
Power BI Desktop

📈 Dashboard Modules
1️⃣ Executive Dashboard

Features:
Total Revenue
Total Orders
Total Customers
AOV
On-Time Delivery %
YOY Growth %
Revenue Trends
Order Status Analysis
Geo Revenue Mapping

2️⃣ Sales Trends Dashboard

Features:
Revenue vs Last Year
Rolling 30 Days Revenue
Revenue YTD
Category-Wise Sales
Orders & AOV Analysis


3️⃣ Category & Product Analytics

Features:
Top Categories by Revenue
Category Revenue Share
Ratings Analysis
Orders vs AOV Scatter Analysis


4️⃣ Payment Analytics

Features:
Payment Type Distribution
Installment Analysis
Payment Trend Analysis
Revenue by Payment Type

5️⃣ Seller Analytics

Features:
Seller Revenue
Seller State Performance
Seller Category Analysis
Geo Seller Mapping

6️⃣ Customer Analytics

Features:
Customer State Revenue
Customer City Revenue
Customer Category Analysis
Customer Distribution Mapping

7️⃣ Delivery & Logistics

Features:
Late Delivery %
Delivery Trend
Delivery Days Analysis
State-Level Delivery Insights

8️⃣ Review Analytics

Features:
Positive vs Negative Ratings
Rating Distribution
Avg Rating by Category
On-Time vs Rating Correlation
📌 Key KPIs
KPI	Description
Revenue	Total Business Revenue
Orders	Total Orders Count
AOV	Average Order Value
On-Time %	Delivery Performance
YOY %	Growth Analysis
Avg Rating	Customer Satisfaction
Late Orders	Logistics Performance
🎯 Advanced Features Implemented

✅ SQL Views Optimization
✅ Direct Query Architecture
✅ Dynamic DAX Measures
✅ Drillthrough Pages
✅ Geo Mapping
✅ Time Intelligence
✅ KPI Cards
✅ Interactive Filtering
✅ Cross-Filtering
✅ Power BI Service Deployment
✅ Gateway Integration
✅ Scheduled Refresh
✅ Real-Time Reporting Approach

📷 Dashboard Preview
Executive Dashboard
Business KPI Monitoring
Revenue Tracking
Geo Analytics
Sales Trends
YTD Analysis
Rolling Revenue
Trend Monitoring
Delivery & Logistics
Late Delivery Insights
Operational Analytics
Customer & Seller Analytics
State-Level Revenue
Performance Analysis
📚 Learning Outcomes

Through this project I learned:

Real-world BI architecture
PostgreSQL analytical engineering
Power BI optimization techniques
Gateway & Cloud Integration
Direct Query performance handling
DAX Time Intelligence
Interactive dashboard development
KPI storytelling
🚀 Future Improvements
Incremental Refresh
Row Level Security (RLS)
Azure Deployment
Automated ETL Pipelines
Python Forecasting Integration
AI Visual Insights
👨‍💻 Author
Shahid Ali

PMO & Data Analytics Professional
Power BI • SQL • PostgreSQL • DAX • Automation • Dashboarding
