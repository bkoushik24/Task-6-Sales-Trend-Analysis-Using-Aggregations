# Task-6-Sales-Trend-Analysis-Using-Aggregations
This task analyzes monthly sales performance using SQL aggregation functions. The dataset (online_sales) contains order details with dates, amounts, and product IDs. Queries extract monthly revenue (SUM(amount)) and order volume (COUNT(DISTINCT order_id)) grouped by year and month. The results help identify seasonal trends, peak sales months.

Task 6 – Sales Trend Analysis Using Aggregations

📌 Objective
The goal of this task is to analyze monthly sales trends using SQL aggregation functions. We calculate total revenue and order volume for each month to identify seasonal patterns, peak performance periods, and potential promotional opportunities.

🛠 Tools & Technologies
- **Database**: MySQL / PostgreSQL / SQLite
- **Language**: SQL
- **Client**: MySQL Workbench / pgAdmin / DB Browser for SQLite

📂 Dataset Structure
The `online_sales` table contains:
- **order_id** – Unique ID for each order
- **order_date** – Date when the order was placed
- **amount** – Order value
- **product_id** – ID of the purchased product

   GROUP BY year, month
   ORDER BY year, month;
