🧾 Task 6: Sales Trend Analysis Using Aggregations

🎯 Objective

* To analyze monthly revenue and order volume trends from the Online Sales Dataset using SQL aggregation functions.
* This helps identify high-performing months, seasonal trends, and business growth patterns across different regions and product categories.

🧰 Tools & Technologies

* Jupyter Notebook
* SQLite 
* Python (Pandas, SQLite3)
* SQL Aggregations

🗂️ Dataset Overview

Dataset Name: Online Sales Dataset – Popular Marketplace Data
The dataset contains global transaction details across product categories.

Column Name	                 Description
Transaction ID	     -       Unique identifier for each transaction
Date	               -       Transaction date
Product Category	   -       Category of the product sold
Product Name	       -       Name of the product
Units Sold	         -       Quantity sold
Unit Price	         -       Price per unit
Total Revenue	       -       Total sale value (Units × Unit Price)
Region	             -       Geographical region of the transaction
Payment Method	     -       Mode of payment used

⚙️ SQL Tasks 

🅰️ Extract Month and Year
Used STRFTIME() (SQLite) / EXTRACT() (PostgreSQL) / MONTH() (MySQL) to extract month and year from the date column.

🅱️ Group by Year and Month
Grouped transactions by month and year to prepare for monthly aggregation.

🅲 Calculate Monthly Revenue
Used SUM(total_revenue) to compute total monthly sales.

🅳 Count Distinct Orders
Used COUNT(DISTINCT transaction_id) to calculate monthly order volume.

🅴 Sort Results
Sorted aggregated results using ORDER BY year, month.

🅵 Filter by Specific Time Period
Used WHERE and LIMIT clauses to focus on a specific year (e.g., 2024).

🧠 Insights & Conclusion

* Monthly aggregation reveals clear sales seasonality across quarters.
* The highest revenue and order volume were observed in Q2 2024, indicating peak demand.
* The use of SQL aggregation (SUM, COUNT DISTINCT) efficiently summarized large datasets.
* These insights can assist in forecasting demand and optimizing marketing efforts during high-performing months.
