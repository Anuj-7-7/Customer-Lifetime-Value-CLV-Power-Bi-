# Customer Lifetime Value (CLV) Analysis & Dashboard — Power BI

## Project Overview
Customer Lifetime Value (CLV) helps businesses understand how much revenue a customer generates over the course of their relationship with the company.  
This project focuses on **historic CLV** to support data-driven decisions around customer retention, acquisition strategy, and long-term revenue planning.

The goal of this analysis is to move beyond short-term sales metrics and identify **high-value customers, segments, regions, and product categories** using transactional data.

---

## Dataset
- **Source:** Superstore dataset (Kaggle)
- **Data Type:** Transaction-level sales data
- **Time Period:** 2014–2017
- **Key Fields:** Customer, Order Date, Sales, Product, Category, Segment, Region

---

## Key Metrics Calculated
- Total Sales  
- Total Orders  
- Active Customers  
- Average Purchase Value (APV / AOV)  
- Average Purchase Frequency (APF)  
- Average Revenue per Customer (ARPC)  
- Monthly Churn Rate (adjusted)  
- Average Customer Lifespan (1 / churn)  
- Customer Lifetime Value (CLV = ARPC × Customer Lifespan)

---

## Data Preparation & Modeling
- Cleaned and transformed data using **SQL (MySQL)**, **Python**, and **Excel**
- Handled missing values, refunds (negative sales), and date inconsistencies
- Built a star schema with a Sales fact table and Customer, Product, Location, and Date dimensions
- Created a Month-level date key to enable accurate time-based analysis and churn calculations

---

## Dashboard Structure (Power BI)
The Power BI report is organized into three pages:

### 1. Executive Overview
- High-level KPIs: Sales, Orders, Active Customers, CLV
- Trend analysis of customer value over time

### 2. CLV Drivers & Trends
- Analysis of APV, APF, and ARPC trends
- Scatter plot showing **CLV vs Active Customers** to compare customer value vs scale

### 3. Customer & Segment Insights
- CLV by customer segment, region, and product category
- Top N customers by lifetime value
- Actionable insights for retention, acquisition, and cross-sell strategies

---

## Key Business Insights
- CLV varies significantly across customer segments and regions
- High CLV is often driven by lower churn rather than higher order value alone
- Retention improvements can increase lifetime value without increasing acquisition spend
- Identifying high-LTV customers enables targeted loyalty and upsell strategies

---

## Tools & Technologies
- Power BI (DAX, data modeling, visualization)
- SQL (MySQL)
- Python (pandas)
- Excel

---

## Repository Contents
- `/dashboard` — Power BI `.pbix` file  
- `/screenshots` — Dashboard page screenshots  
- `/data` — Dataset (optional)  

---

## Notes
This project uses **historic CLV**, not predictive CLV.  
All calculations are based on observed customer behavior within the available time period.

---

