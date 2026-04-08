# 📊 Sales Performance Dashboard | Documentation

---

## 1. Problem Statement

The objective of this project is to analyze sales performance across different regions, products, and customer segments to support business decision-making.

The dashboard aims to:

- Monitor key business KPIs
- Identify revenue and profit trends
- Analyze customer behavior
- Evaluate product performance
- Compare actual performance against targets

---

## 2. Dataset Description

The dataset contains transactional sales data with the following fields:

- Order Date
- Product Name
- Category & Subcategory
- Customer Details
- Revenue, Profit, Orders, Returns
- Region and Country

The data represents sales activity across multiple regions including Europe, North America, and Pacific.

---

## 3. Data Cleaning & Transformation

Data preparation was performed using Power Query:

- Removed null and duplicate records
- Standardized column names for consistency
- Converted data types (Date, Numeric, Currency)
- Created new columns:
  - Year
  - Month
  - Revenue per Customer

---

## 4. Data Modeling

A **star schema** approach was used for efficient querying:

- **Fact Table:**

  - Sales

- **Dimension Tables:**
  - Customers
  - Products
  - Geography
  - Date

Relationships:

- One-to-many relationships between dimension tables and fact table
- A dedicated Date table was created for time-based analysis

---

## 5. DAX Measures

The project includes multiple DAX measures categorized as follows:

### 🔹 KPI Measures

- Total Revenue
- Total Orders
- Total Profit
- Return Rate

### 🔹 Time Intelligence Measures

- Previous Month Revenue
- Previous Month Orders
- Previous Month Profit
- Previous Month Returns

### 🔹 Target & Comparison Measures

- Order Target
- Profit Target
- Order Target Gap
- Profit Target Gap

### 🔹 Advanced Measures

- Rolling 10 Days Orders
- Rolling 90 Days Profit
- Revenue per Customer
- Average Retail Price

### 🔹 Category & Product Measures

- Category Orders
- Bike Sales
- Bike Returns
- Bulk Orders

These measures enable dynamic analysis, trend evaluation, and performance comparison across different dimensions.

## 6. Dashboard Pages & Features

### 🔹 Page 1: Executive Overview

- KPI Cards: Revenue, Orders, Profit, Return Rate
- Revenue Trend Analysis
- Orders by Category
- Top 10 Products (Revenue, Orders, Profit)
- Monthly performance summary

---

### 🔹 Page 2: Regional Analysis

- Region selector (Europe, North America, Pacific)
- Map visualization showing orders by country
- Helps identify geographical performance trends

---

### 🔹 Page 3: Performance vs Target

- Gauge charts for:
  - Orders vs Target
  - Revenue vs Target
  - Profit vs Target
- Trend analysis using field parameters
- Category contribution breakdown

---

### 🔹 Page 4: Customer Insights

- Unique Customers KPI
- Revenue per Customer
- Customer trend analysis
- Segmentation:
  - Occupation
  - Income level
  - Education
- Top 100 customers table

---

## 7. Key Features Implemented

- Interactive slicers (Year, Region)
- Drillthrough functionality for detailed analysis
- Dynamic field parameters for switching metrics
- Tooltips for enhanced insights
- Conditional formatting for KPIs
- Clean and user-friendly UI design

---

## 8. Key Insights

- Accessories category has the highest number of orders
- Revenue shows consistent growth after 2021
- A small set of products contributes significantly to profit
- Customer segments differ based on income and education
- Return rate is low (~2%), indicating good product satisfaction

---

## 9. Challenges Faced

- Managing multiple KPIs dynamically using field parameters
- Designing a clean layout with high information density
- Optimizing performance for large datasets
- Creating meaningful comparisons for target visuals

---

## 10. Future Improvements

- Add forecasting using time-series analysis
- Implement Row-Level Security (RLS)
- Integrate real-time data sources
- Enhance dashboard with AI-powered visuals

---

## 11. Tools & Technologies

- Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Excel / CSV dataset

---
