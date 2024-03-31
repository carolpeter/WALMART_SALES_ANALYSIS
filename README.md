WALMART SALES DATA

ABOUT

This project seeks to analyze Walmart Sales data to identify the most successful branches and products, track the sales trends of various products, and examine customer behavior. The objective is to investigate opportunities for enhancing and optimizing sales strategies. The dataset originates from the Walmart Sales Forecasting Competition on Kaggle.

PURPOSE

The primary objective of this project is to analyze Walmart's sales data comprehensively, aiming to discern various factors influencing the sales performance across its different branches.

ABOUT THE DATA

This dataset contains sales transactions from a three different branches of Walmart, respectively located in Mandalay, Yangon and Naypyitaw. The data contains 17 columns and 995 rows.

Column	Data Type
Invoice_id	VARCHAR(30)
Branch	VARCHAR(5)
City	VARCHAR(30)
Customer_type	VARCHAR(30)
Gender	VARCHAR(10)
Product_line	VARCHAR(100)
Unit_price	DECIMAL(10, 2)
Quantity	INT
VAT	FLOAT(6, 4)
Total	DECIMAL(10, 2)
Date	DATE
Time	TIMESTAMP
Payment_method	DECIMAL(10, 2)
COG	DECIMAL(10, 2)
Gross_margin_percentage	FLOAT(11, 9)
Gross_income	DECIMAL(10, 2)
Rating	FLOAT(2, 1)

Approach Used

1.	Data Wrangling: This is the first step where inspection of data is done to make sure NULL values, missing values are detected, and data replacement methods are used to replace, missing or NULL values.
1.	Build a database
2.	Create table and insert the data.
3.	Select columns with null values in them. There are no null values in our database as in creating the tables
2.	Feature Engineering: This will help use generate some new columns from existing ones.
1.	Add a new column named time_of_day to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.
2.	Add a new column named day_name that contains the extracted days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri). This will help answer the question on which week of the day each branch is busiest.
3.	Add a new column named month_name that contains the extracted months of the year on which the given transaction took place (Jan, Feb, Mar). Help determine which month of the year has the most sales and profit.
   
Business Questions To Answer

Generic Question

1.	How many unique cities does the data have?
2.	In which city is each branch?
   
Product

1.	How many unique product lines does the data have?
2.	What is the most common payment method?
3.	What is the most selling product line?
4.	What is the total revenue by month?
5.	What month had the largest COGS?
6.	What product line had the largest revenue?
7.	What is the city with the largest revenue?
8.	What product line had the largest VAT?
9.	Fetch each product line and add a column to those product line showing "Good", "Bad". Good if its greater than average sales
10.	Which branch sold more products than average product sold?
11.	What is the most common product line by gender?
12.	What is the average rating of each product line?
    
Sales

1.	Number of sales made in each time of the day per weekday
2.	Which of the customer types brings the most revenue?
3.	Which city has the largest tax percent/ VAT (Value Added Tax)?
4.	Which customer type pays the most in VAT?
   
Customer

1.	How many unique customer types does the data have?
2.	How many unique payment methods does the data have?
3.	What is the most common customer type?
4.	Which customer type buys the most?
5.	What is the gender of most of the customers?
6.	What is the gender distribution per branch?
7.	Which time of the day do customers give most ratings?
8.	Which time of the day do customers give most ratings per branch?
9.	Which day fo the week has the best avg ratings?
10.	Which day of the week has the best average ratings per branch?
