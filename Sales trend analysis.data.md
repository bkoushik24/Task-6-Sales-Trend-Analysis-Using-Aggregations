**1.Sales Trend Analysis Using Aggregations**



**Query:**

SELECT 

&nbsp;   EXTRACT(YEAR FROM order\_date) AS year,

&nbsp;   EXTRACT(MONTH FROM order\_date) AS month,

&nbsp;   SUM(amount) AS total\_revenue,

&nbsp;   COUNT(DISTINCT order\_id) AS total\_orders

FROM online\_sales

GROUP BY year, month

ORDER BY year, month;



**2.Filtering for a Specific Time Period**

**Example: Show trends only for 2024**



**Query:**

SELECT 

&nbsp;   EXTRACT(YEAR FROM order\_date) AS year,

&nbsp;   EXTRACT(MONTH FROM order\_date) AS month,

&nbsp;   SUM(amount) AS total\_revenue,

&nbsp;   COUNT(DISTINCT order\_id) AS total\_orders

FROM online\_sales

WHERE EXTRACT(YEAR FROM order\_date) = 2024

GROUP BY year, month

ORDER BY month;



**3. Sample Output (Example Data)**



year	month	total\_revenue	total\_orders

2024	1	12,500.00	95

2024	2	14,200.00	110

2024	3	10,800.00	87

2024	4	16,900.00	132

2024	5	18,400.00	145

