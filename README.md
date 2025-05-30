# SQL-for-Data-Analysis3
Ecommerce SQL Project
This project uses MySQL to manage and analyze a sample e-commerce dataset.
The goal is to create tables, insert data, run queries, and optimize performance using indexes.

📁 Files Included
ecommerce_sample.sql: Contains database schema creation, data insertion, indexing, and SQL queries.
query_results.csv: Exported results from SELECT queries.
Screenshots: Images showing successful query execution in MySQL Workbench.
🧪 Features Demonstrated
SELECT, WHERE, ORDER BY, GROUP BY
SQL JOINs between Customers, Orders, and Products
Aggregate Functions like SUM and AVG
Subqueries for filtering
Performance optimization using INDEXES
🛠 Tools Used
MySQL Workbench
GitHub
🛒 Ecommerce SQL Project
This project demonstrates how to use SQL to manage and analyze a basic e-commerce database using MySQL Workbench.

📦 What’s Included
File	Description
ecommerce_sample.sql	Full SQL script to create and populate the database, add indexes, and run sample queries
query_results.csv or .xlsx	Sample export of a query output (e.g., products in the Electronics category)
screenshot.png	Screenshot showing MySQL Workbench result and action log
README.md	Project description and summary of what was done
✅ Features Implemented
Created 3 related tables: Customers, Products, and Orders
Inserted test data to simulate order activity
Used SQL features:
SELECT, WHERE, ORDER BY, GROUP BY
JOIN across tables
Aggregate Functions: SUM, AVG
Subqueries
Performance optimized with INDEX on:
Foreign keys (customer_id, product_id)
Search fields (country, category)![Screenshot (52)](https://github.com/user-attachments/assets/e51c6511-86b4-459e-838b-da3656803e56)
![Screenshot (51)](https://github.com/user-attachments/assets/bf276ddf-333d-4957-b7d7-4953ca0ba79e)

![Screenshot (50)](https://github.com/user-attachments/assets/84c0c851-1a70-4839-b469-d1ef0ef19f49)
![Screenshot (49)](https://github.com/user-attachments/assets/d480c48c-f2cf-4468-8bf3-58952320e7b3)
![Screenshot (45)](https://github.com/user-attachments/assets/3575e951-676c-48b8-ab0d-74af87077c4f)

![Screenshot (48)](https://github.com/user-attachments/assets/01475873-7e42-4ba6-ba2f-2df82c3f2d3e)
![Screenshot (47)](https://github.com/user-attachments/assets/122e072c-60fc-4406-95fa-7d615a5c90d9)
![Screenshot (46)](https://github.com/user-attachments/assets/e54bc113-66c0-4a2d-aa3b-62ff7299909f)

💡 Example Queries Used
-- Join example
SELECT c.customer_name, p.product_name, o.total_amount
FROM Orders o
JOIN Customers c ON o.customer_id = c.customer_id
JOIN Products p ON o.product_id = p.product_id;

-- Group by example
SELECT category, AVG(price) AS avg_price
FROM Products
GROUP BY category;

-- Subquery example
SELECT customer_name
FROM Customers
WHERE customer_id IN (
    SELECT customer_id
    FROM Orders
    WHERE quantity > 1
);

