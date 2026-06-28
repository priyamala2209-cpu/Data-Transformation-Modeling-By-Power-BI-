## Data-Modeling-Using-Power-BI
 
This Power BI analysis addresses the critical business challenge of measuring actual sales performance against predefined monthly and category-wise targets. By identifying performance gaps and variance, it enables stakeholders to make informed, data-driven decisions.
    
 #🎯 Project Overview
 Business Problem:

 The organization faced challenges in systematically tracking and evaluating actual sales performance against predefined monthly and category-wise targets. This lack of visibility made it difficult to identify performance shortfalls, measure profitability across segments, and provide leadership with data-driven insights for strategic decision-making.
     
 # Objective:

The objective of this project is to transform raw transactional sales data into a clean, structured analytical model within Power BI to enable accurate performance tracking and variance analysis.

**Specific Goals:**

- **Data Preparation:** Clean and standardize the Orders, Order Details, and Sales Target datasets using Power Query
  
- **Data Transformation:** Apply text formatting, calculated columns, conditional logic, grouping, and table merges to create an analysis-ready model
 
- **Model Development:** Establish relationships and optimize the data model for reporting performance
  
# Target Audience:
This Power BI solution is designed for two key stakeholder groups who require visibility into sales performance against defined targets:

 - **Executive Leadership:** Provides high-level KPI summaries and variance analysis to monitor overall sales performance vs. strategic targets, assess organizational health, and guide board-level decisions
   
 - **Sales Operations Teams:** Enables detailed tracking of category-wise and monthly performance to identify shortfalls, analyze root causes, and adjust sales strategies and resource allocation

 # 🗃️ Data Sources & Architecture

   **Source Data :**
   The analysis uses three primary datasets: Orders, Order Details, and Sales Target, containing transactional and goal-setting data required for performance comparison.

   **Architecture & Tools:**
   
   **Power Query:** Serves as the ETL layer for data ingestion, cleaning, transformation, and preparation before loading into the model
   
   **Power BI Desktop:** Primary environment for data modeling, establishing table relationships, DAX measure creation, and dashboard development
    
**Data Volume:**
The project utilizes three structured datasets covering one complete fiscal year of business operations:

  **-Orders Dataset (List of Orders.csv):** Approximately 2,000 customer order records spanning April 2018 to March 2019. Contains order-level metadata including Order ID, Order Date, and Customer details
  
  **-Order Details Dataset (Order Details.csv):** Approximately 500 rows of product-level transaction data. Includes Amount, Profit, Quantity, Category, and Sub-Category for granular analysis
  
 **-Sales Target Dataset (Sales Target.csv):** 36 rows representing monthly category-wise targets across Furniture, Clothing, and Electronics for the full year
 
 **-Timeframe:**  → Full fiscal year analysis enabling YoY and monthly trend evaluation
 
Storage Mode: Power BI Import Mode selected for all datasets

# ⚙️ Data Transformation (ETL)

   **-Tool Used :** Power Query Editor served as the primary ETL environment for all data preparation activities.
   
**Key Transformations Applied:**

   **- Data Merging:** Combined the Orders and Order Details tables using Order ID as the primary key to create a unified fact table for analysis
   
   **- Column Standardization:** Applied text formatting, data type conversions, and null handling across all datasets to ensure consistency
   
   **- Calculated Columns:** Created new columns including Total Sales, Profit Margin, and Target Achievement % to enable variance analysis
   
   **- Conditional Logic:** Implemented business rules for categorization and flagging performance exceptions
   
   **- Grouping & Aggregation:** Structured data at appropriate grain for monthly and category-level reporting
   
 # 🧠 Data Model 

  Model Type - Star Schema
 The data model follows star schema architecture optimized for analytical performance and intuitive reporting.

 **Structure:**
 Fact Tables:
  
  **-Sales Fact** — consolidated from merged Orders and Order Details. Contains quantitative metrics including Amount, Profit, Quantity, and foreign keys to dimensions
  
Dimension Tables
  
  **-Date** — Calendar dimension for time-based analysis by month, quarter, year
  
  **-Category** — Product categories and sub-categories for dimensional slicing
  
  **-Sales Target** — Monthly targets by category for variance analysis

 # 🖥️ Dashboard Features
 The Power BI dashboard delivers interactive analytics across key business functions:

  **1. Sales vs Target Analysis**
Compare actual sales performance against monthly and category-wise targets. Features variance indicators, achievement %, and gap analysis to highlight over or under performance across Furniture, Clothing, and Electronics.

  **2. Profitability Insights**
Monitor total profit, profit margin %, and category profitability. Includes drill-down capabilities to identify loss-making products, sub-categories, and time periods requiring attention.

  **3. Interactive Filtering**
Slicers for Date, Category, and Sub-Category enable dynamic segmentation. Cross-filtering between visuals allows users to explore specific performance drivers.

**4. KPI Summary Cards**
High-level metrics display Total Sales, Total Profit, Target Achievement %, and Profit Margin for instant executive overview.

# 🚀 How To Use
**Prerequisites:**

Steps to Access:
Ensure Power BI Desktop is installed before accessing the dashboard file. Latest version recommended for full feature compatibility.

**Download Power BI Desktop:** Visit the Microsoft Power BI official site and download the latest version

**Install Application:** Run the installer and follow on-screen prompts to complete setup

**Verify Installation:** Open Power BI Desktop. Go to Help > About to confirm version is current

**Launch Dashboard:** Open the provided .pbix file by double-clicking or using File > Open in Power BI Desktop

**Refresh Data:** Click Home > Refresh if prompted to update data connections

              Thank You
