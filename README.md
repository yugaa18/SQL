📚 Online Bookstore – SQL Data Analysis Project

📌 Project Overview
This project analyzes a relational dataset for an online bookstore using PostgreSQL. It covers database design, data import, and a series of SQL queries — from basic filtering to multi-table joins and aggregations — to answer real business questions about sales, customers, and inventory.

🎯 Project Objective
Design a normalized relational schema for Books, Customers, and Orders.
Import and validate transactional data.
Answer business questions using SQL: revenue, top sellers, customer behavior, and stock levels.
🛠️ Tech Stack
Database: PostgreSQL
Techniques used: Multi-table JOINs (INNER, LEFT), GROUP BY, HAVING, aggregate functions (SUM, AVG, COUNT), WHERE filtering, ORDER BY / LIMIT, DISTINCT, COALESCE
🗂️ Schema

Books (500 records)

Column	Type
Book_ID	SERIAL, Primary Key
Title	VARCHAR(100)
Author	VARCHAR(100)
Genre	VARCHAR(50)
Published_Year	INT
Price	NUMERIC(10,2)
Stock	INT

Customers (500 records)

Column	Type
Customer_ID	SERIAL, Primary Key
Name	VARCHAR(100)
Email	VARCHAR(100)
Phone	VARCHAR(15)
City	VARCHAR(50)
Country	VARCHAR(150)

Orders (500 records)

Column	Type
Order_ID	SERIAL, Primary Key
Customer_ID	FK → Customers
Book_ID	FK → Books
Order_Date	DATE
Quantity	INT
Total_Amount	NUMERIC(10,2)

📊 Key Business Questions Answered

Which books belong to the "Fiction" genre?

Which books were published after 1950?

Which customers are located in Canada?

Which orders were placed in November 2023?

What is the total stock of books available?

What is the most expensive book in the catalog?

Which orders had a quantity greater than 1?

Which orders exceeded $20 in total amount?

What genres exist in the catalog?

Which book has the lowest stock?

What is the total revenue generated from all orders?

What is the total number of books sold per genre?

What is the average price of books in the "Fantasy" genre?

Which customers placed 2 or more orders?

Which book has been ordered the most times?

What are the top 3 most expensive Fantasy books?

What is the total quantity sold by each author?

Which cities have customers who spent over $30?

Which customer spent the most overall?

What is the remaining stock for each book after fulfilling all orders?

💡 Key Findings
Run the queries above against the dataset and fill in the actual results here — for example:

--Highest-spending customer: [run query #18]
![image alt](https://github.com/yugaa18/SQL/blob/048b3bb38576cfd8a43426ef3f6180f8a8154a2b/SQL-QUERY%20(SCREENSHOT1).png)

--List customers who have placed at least 2 orders: [run query #14]
![image alt](https://github.com/yugaa18/SQL/blob/6133e26491e3cbd2d369e69fc9e3129cb1d8a66e/SQL-QUERY(SCREENSHOT2).png)

--List the cities where customers who spent over $30 are located: [run query #17]
![image alt]


👨‍💻 Author

Yuga Bhagat — B.Tech Graduate | Aspiring Data Analyst
