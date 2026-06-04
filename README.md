# E-Commerce Sales Dashboard using Power BI

## Project Overview
This project is an interactive Power BI dashboard created to analyze e-commerce sales data.  
It helps to understand total sales, profit, quantity, orders, and profit margin.

## Tools Used
- Power BI
- CSV Dataset
- DAX
- Data Visualization
  
## Dataset
The project uses two CSV files:

- Orders.csv
- Details.csv

## Key KPIs
- Total Sales
- Total Profit
- Total Quantity
- Total Orders
- Profit Margin %

## DAX Measures

```DAX
Total Sales = SUM(Details[Amount])

Total Profit = SUM(Details[Profit])

Total Quantity = SUM(Details[Quantity])

Total Orders = DISTINCTCOUNT(Orders[Order ID])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
