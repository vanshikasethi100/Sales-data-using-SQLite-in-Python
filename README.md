# Sales-data-using-SQLite-in-Python
This project demonstrates how to use SQLite inside Python to perform basic sales analysis. It connects to a small SQLite database, runs SQL queries to calculate total quantity sold and total revenue per product, and visualizes the results using a simple bar chart.
Tools Used-
1) Python
2) SQLite (via sqlite3 module)
3) pandas
4) matplotlib

Dataset-
A small SQLite database file:
sales_data.db
It contains one table:

Table: sales
Column	Type	Description
product	TEXT	Product name
quantity	INTEGER	Units sold
price	REAL	Price per unit

SQL Query Used-
SELECT product,
       SUM(quantity) AS total_quantity,
       SUM(quantity * price) AS total_revenue
FROM sales
GROUP BY product;

Output-
1) Printed sales summary table
2) Bar chart showing revenue by product

What I Learned-
1) Creating and connecting to SQLite databases in Python
2) Writing SQL queries with GROUP BY and SUM
3) Loading SQL results into pandas
4) Visualizing results using matplotlib
5) Understanding the end-to-end flow: Database → SQL → Python → Visualization
