# Retail Sales Data Warehouse & BI Analysis

## Project Overview

This project builds a simplified retail data warehouse and performs business intelligence (BI) analysis using SQL and Python. The focus is on demonstrating how to structure data into multiple tables and analyze it using JOIN operations.

---

## Objective

The goal of this project is to:

* Transform a flat dataset into a structured data model
* Practice SQL joins across multiple tables
* Perform BI-style analysis on sales and customers
* Create clear and meaningful visualizations
* Derive concise, data-driven insights

---

## Tools & Technologies

* Python (Pandas)
* SQL (SQLite)
* Matplotlib
* Jupyter Notebook (VS Code)

---

## Data Modeling

The original dataset was split into four tables to simulate a basic data warehouse (star schema):

### Dimension Tables

* **customers**: customer_id, customer_name, segment
* **orders**: order_id, order_date, ship_date, ship_mode, customer_id
* **products**: product_id, product_name, category, sub_category

### Fact Table

* **sales**: order_id, product_id, sales

This structure allows for more realistic SQL queries using joins.

---

## Process

### 1. Data Loading & Cleaning

* Standardized column names
* Converted date columns to datetime format
* Removed duplicate rows
* Verified data structure using `.info()`

---

### 2. SQL Analysis (JOIN-Based)

The following analyses were performed using SQL joins:

* Total Sales by Category
* Total Sales by Customer Segment
* Monthly Sales Trend
* Top 10 Customers by Total Sales
* Average Order Value by Customer Segment

---

### 3. Data Visualization

The following visualizations were created:

* Total Sales by Category (bar chart)
* Total Sales by Customer Segment (bar chart)
* Monthly Sales Trend (line chart)
* Average Order Value by Segment (bar chart)

---

## Key Insights

* Technology generates the highest total sales, although the difference compared to other categories is moderate.

* The Consumer segment contributes the largest share of total sales, followed by Corporate and Home Office, indicating that individual consumers are the primary revenue drivers.

* Monthly sales show noticeable volatility but follow an overall upward trend over time.

* Average order value is similar across all customer segments, suggesting that differences in total sales are driven more by order volume rather than order size.

---

## Conclusion

This project demonstrates how to structure data into a relational model and perform SQL-based BI analysis using multiple tables. The results highlight the importance of joins, aggregation, and correct data granularity in producing meaningful business insights.

---

## Project Structure

```text
Retail_Sales_Data_Warehouse_&_BI_Analysis/
├── data/
│   ├── customers.csv
│   ├── orders.csv
│   ├── products.csv
│   ├── sales.csv
├── retail_data_warehouse_analysis.ipynb
```
