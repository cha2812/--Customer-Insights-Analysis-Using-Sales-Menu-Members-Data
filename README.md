# --Customer-Insights-Analysis-Using-Sales-Menu-Members-Data
Emphasizes the comprehensive nature of your project, covering customer behaviour analysis, sales data, menu items, and the SQL queries used for analysis

## Introduction
The Danny Ma restaurant dataset was provided with three(3) files which represented our tables. We have sales, menu and members which we created in PostgreSQL and I performed data analysis using SQL. The dataset contains information about various customer IDs, order dates, product IDs, prices, product names and the join date details.

## Problem Statement
I wanted to find a way to understand the business of Danny Ma and how the products he offered were been received by customers. Figure out the relationship between price, products and customers. 
The following questions were asked and the answers were provided to questions and problems below.
1. The most purchased item on the menu and how many times it was purchased by all customers.
2. The item that was the most popular for each customer.
3. The item that was purchased first by the customer after they became a member.
4. The item that was purchased just before the customer became a member.
5. The total items and amount spent for each member before they became a member.

## Data Analysis
The analysis was done using tables that were provided. The 3 tables provided were the sales table, the menu table and the members table. <br>
The sales table had 3 columns; customer id, order date, and product id. <br>
The menu table had 3 columns; product id, product name and total area price. <br>
The members table also had 2 columns; customer id, and join date. <br>

For problem 1, The most purchased item on the menu and how many times it was purchased by all customers. <br>
It achieves this by joining the "sales" and "menu" tables on the "product_id" column. Then, it groups the results by the product name and counts the occurrences of each product in the sales table. Finally, the results are ordered in descending order of purchase count, and the query limits the output to the first row to get the most purchased item.
