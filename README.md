# About
This project aims to explore the Walmart Sales data to understand top performing branches and products, sales trend of of different products, customer behaviour. The aims is to study how sales strategies can be improved and optimized. The dataset was obtained from the [Kaggle Walmart Sales Forecasting Competition](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting).

"In this recruiting competition, job-seekers are provided with historical sales data for 45 Walmart stores located in different regions. Each store contains many departments, and participants must project the sales for each department in each store. To add to the challenge, selected holiday markdown events are included in the dataset. These markdowns are known to affect sales, but it is challenging to predict which departments are affected and the extent of the impact." [source] (https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting)

# Purpose
The main goal of this project is to obtain insight into Walmart's sales data in order to comprehend the various elements that influence sales at various branches.

# Data
The Walmart Sales Forecasting Competition on Kaggle provided the dataset. The sales transactions from three separate Walmart branches—one each in Mandalay, Yangon, and Naypyitaw—are included in this dataset. There are 1000 rows and 17 columns in the data:

| Column                  | Description                             | Data Type      |
|-------------------------|-----------------------------------------|----------------|
| invoice_id              | Invoice of the sales made               | VARCHAR(30)    |
| branch                  | Branch at which sales were made         | VARCHAR(5)     |
| city                    | The location of the branch              | VARCHAR(30)    |
| customer_type           | The type of the customer                | VARCHAR(30)    |
| gender                  | Gender of the customer making purchase  | VARCHAR(10)    |
| product_line            | Product line of the product solf        | VARCHAR(100)   |
| unit_price              | The price of each product               | DECIMAL(10, 2) |
| quantity                | The amount of the product sold          | INT            |
| VAT                     | The amount of tax on the purchase       | FLOAT(6, 4)    |
| total                   | The total cost of the purchase          | DECIMAL(10, 2) |
| date                    | The date on which the purchase was made | DATE           |
| time                    | The time at which the purchase was made | TIMESTAMP      |
| payment_method          | The total amount paid                   | DECIMAL(10, 2) |
| cogs                    | Cost Of Goods sold                      | DECIMAL(10, 2) |
| gross_margin_percentage | Gross margin percentage                 | FLOAT(11, 9)   |
| gross_income            | Gross Income                            | DECIMAL(10, 2) |
| rating                  | Rating                                  | FLOAT(2, 1)    |

# Analysis List

1. List Analysis 
Analyze the data to identify the various product lines, the ones that are doing well, and the ones that want improvement.

2. Analysis of Sales
The goal of this investigation is to provide an answer to the query about product sales trends. The outcome of this can assist us in gauging the success of every sales technique the company employs and the adjustments required to increase sales.

3. Customer Analysis
The many customer segments, purchasing patterns, and profitability of each customer category are the focus of this investigation.

# Approach Used

"Data Wrangling": This is the first step where inspection of data is done to make sure NULL values and missing values are detected and data replacement methods are used to replace, missing or NULL values.
1. Build a database
2. Create table and insert the data.
3. Select columns with null values in them. There are no null values in our database as in creating the tables, we set NOT NULL for each field, hence null values are filtered out.
"Feature Engineering": This will help use generate some new columns from existing ones.
1. Add a new column named time_of_day to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.
2. Add a new column named day_name that contains the extracted days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri). This will help answer the question on which week of the day each branch is busiest.
3. Add a new column named month_name that contains the extracted months of the year on which the given transaction took place (Jan, Feb, Mar). Help determine which month of the year has the most sales and profit.
"Exploratory Data Analysis (EDA)": Exploratory data analysis is done to answer the listed questions and aims of this project.


