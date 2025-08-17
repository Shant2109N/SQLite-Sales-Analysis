# SQLite-Sales-Analysis
 
## 📝 Project Overview

As part of my Data Analyst Internship at Elevate Labs, I worked on Task 7, which involved extracting and visualizing sales data from a small SQLite database using Python. The goal was to demonstrate the integration of SQL queries within Python and present meaningful insights in both textual and visual formats.
 
## 🎯 Objective

Leverage Python’s built-in SQLite support to pull simple sales metrics — total quantity sold and total revenue — and visualize them with a basic bar chart.

## 🛠 Tools & Technologies Used

* **Python** (`sqlite3`, `pandas`, `matplotlib`)
* **SQLite** (lightweight, serverless database)
* **Jupyter Notebook** (for development)

## 📂 Steps & Approach

1. **Database Setup**
   Created a small SQLite database file (`sales_data.db`) with a single `sales` table containing `product`, `quantity`, and `price`.

2. **SQL Query Execution**
   Connected to the database using Python’s `sqlite3` module and ran aggregation queries:

   SELECT product, 
          SUM(quantity) AS total_qty, 
          SUM(quantity * price) AS revenue 
   FROM sales 
   GROUP BY product;
 

3. **Data Loading**
   Imported query results into a Pandas DataFrame for easy manipulation.

4. **Data Output**
   Displayed summarized sales data using `print()` statements.

5. **Visualization**
   Created a simple bar chart with Matplotlib to show product-wise revenue.

6. **Export**
   Saved the visualization as `sales_chart.png` for sharing and reporting.

 
## 📊 Key Learning Outcomes

* Practical integration of SQL queries within Python for real-time data analysis.
* Using Pandas to transform SQL results into structured DataFrames.
* Basic data visualization techniques to make results more insightful.
* Understanding of lightweight database workflows using SQLite.

 
