# Adventure Works Cycle - Power BI Data Analysis

## 📌 Project Overview
This project is an end-to-end Business Intelligence solution developed using **Microsoft Power BI**. The objective of this project is to transform raw, unstructured data into a comprehensive, interactive dashboard that provides real-time insights into the sales, returns, and customer demographics for the Adventure Works Cycle company.

*(Note: Due to confidentiality, the underlying `.pbix` source file is not included in this repository. This repository contains the project report and documentation of the methodologies used).*

---

## 🛠️ Technology Stack & Skills Demonstrated
*   **Business Intelligence Tool:** Microsoft Power BI (Desktop & Service)
*   **Data Transformation:** Power Query (ETL)
*   **Data Modeling:** Relational Database Design (Star Schema)
*   **Calculations:** DAX (Data Analysis Expressions)
*   **Data Visualization:** Interactive Dashboards and Reports

---

## ⚙️ Data Pipeline & Methodology

### 1. Data Extraction & Transformation (ETL)
Connected Power BI to raw data sources (Flat files, Databases) and used **Power Query Editor** to shape the data:
*   **Data Cleaning:** Removed anomalies and handled missing values.
*   **Custom Columns:** Added conditional columns (e.g., categorizing `OrderQuantity` into "One Item" or "Multiple Items").
*   **Index Columns:** Created sequential unique IDs to establish proper relationships.
*   **Pivoting/Unpivoting:** Restructured data tables from horizontal to vertical layouts for better analysis.

### 2. Data Modeling & Normalization
Designed a robust relational data model optimized for performance:
*   **Fact Tables:** `Sales_Data`, `Returns_Data`
*   **Dimension (Lookup) Tables:** `Calendar`, `Product_Lookup`, `Customer_Lookup`, `Territory_Lookup`
*   **Relationships:** Established **One-to-Many** cardinality between Lookup tables and Data tables using Primary/Foreign keys (e.g., `ProductKey`, `CustomerKey`).
*   Configured **Cross-Filter Directions** (Single and Two-Way) to ensure accurate data filtering across the model.

### 3. DAX (Data Analysis Expressions)
Created complex calculations to drive the dashboard visuals:
*   **Calculated Columns:** Added new attributes to existing tables.
*   **Measures:** Developed dynamic measures for aggregations, including weighted averages and time intelligence formulas to track rolling revenue and year-over-year growth.

---

## 📊 Dashboard & Visualizations
The final report is divided into interactive tabs utilizing standard and custom marketplace visuals:

### 1. Executive Summary
Provides a high-level overview of overall performance, tracking total orders, revenue, and returns against target KPIs. Features dynamic slicers for date and geographical filtering.

### 2. Product Details
Focuses on individual product performance. Tracks metrics like Adjusted Price, Weekly Profit, and Weekly Return Volume using line charts and KPI indicators.

### 3. Customer Detail
Analyzes the customer base, segmenting users by occupation, income level, and age. Highlights top customers (e.g., Mr. Maurice Shan) by total orders and revenue.

---

## 📄 Full Report
For a deep dive into the ER Diagrams, Data Flow Diagrams, and step-by-step implementation, please review the complete project report:
[Download the Adventure Work Cycle Project Report (PDF)](./1Adventure_Work_Cycle_project_Report.pdf)
