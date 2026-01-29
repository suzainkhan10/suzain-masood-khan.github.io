# Sales Performance Analysis (SQL)

## Project Overview
This project analyzes sales data using SQL to identify revenue trends, top-performing products, and regional performance.

## Dataset
- Source: Sales transaction data (CSV)
- Fields include: Order Date, Product, Category, Region, Quantity, Unit Price

## Tools Used
- SQL (SQLite)
- Visual Studio Code

## Analysis Performed
- Total revenue calculation
- Revenue by region
- Best-selling products
- Monthly sales trend analysis

## Sample Query
```sql
SELECT Category,
       SUM(Quantity * Unit_Price) AS revenue
FROM sales
GROUP BY Category
ORDER BY revenue DESC;