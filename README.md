# E-Commerce-Dashboard-Major-Project
Using Power BI

## Overview
The attached dataset contains ecommerce orders of a company from multiple countries in 2023. It is a mobile accessories ecommerce company with a global footprint. The company is headquartered in Bangalore in India. The supply chain of the company is very strong: customers are located in 14 countries and they receive orders within a week.

There are various ways in which a customer can order. An order can be placed using the company’s app, its website, using Whatsapp and also via other sources (for example: dialing in the 24*7 support helpline number). Customers are divided into 5 categories: A, B, C, D, E.

The sales team in the company is structured into 5 teams: Alpha, Beta, Gamma, Delta and Epsilon. Every team has multiple Sales Managers and a few Sales POCs, typically 3-4. Every sales POC is given individual targets and the sum of the targets of the sales POCs is the target of the Sales Manager.

## Dataset
There are 3 tables within the Excel file: Orders, Customers and Sales Targets.
1. Orders: It contains data corresponding to orders in 14 countries. The Order ID is unique for every order. One customer can place more than one order. The Order Datetime specifies the timestamp (GMT) when the order was placed. The Order Source specifies the source of the order: App, Website, WhatsApp or Other. Every order has a Sales POC associated with it. The Order Value is in rupees.
2. Customers: The Customer ID is a unique ID for each customer. The age, gender, country and category which the customer is classified into is given in this table.
3. Sales Targets: This table contains the Sales POC → Sales Manager mapping as well as the Sales Team of every Sales POC (Point of Contact) and hence Sales Manager. It also contains the targets that each Sales POC has been given.

Note that Sales POCs are not limited to any customer or country. This means that a Sales POC can be responsible for orders placed by Customer A in Country X as well as for orders placed by Customer B in Country Y.

## Detailed Problem Statement (Stepwise)
As an analyst, your goal is to help the company derive insights from the data. These insights will help the company take decisions w.r.t. Orders. Eventually it will help the company increase the number of orders, value of orders and hence revenue. Your manager asks you to perform the following operations and get answers to key questions.
1. Import all the tables in Power BI Desktop.
2. At the start of the new financial year, there was a bug in the system which led to inadequate capturing of the Sales Channel.
* Identify the first and last timestamps when we weren't capturing this data.
* Handle these missing values appropriately.
* Why did you use the above approach for imputing the missing values?
3. Combine the first name and last name to create a Sales Manager Column in Power Query.
4. Create a Data Model with the three tables.
5. We want to understand the Sales Targets and their completion rates.
* Define three buckets: Target not met, Target Met, Exceeded Target for Sales POCs and plot the three categories on an appropriate chart to see the counts.
* Which Sales Teams were given how much total sales targets in total. Plot on a chart to see the comparison. Which sales manager was given the highest target? Did he/she meet that target?
* On average, how much short were actual sales from targets for the Sales POCs who did not complete them.
* Plot the % target reached per Sales Manager in each team.
6.  In each country, display which Sales Managers have been most successful.
* in terms of sales value
* in terms of number of orders and customers
7. We want to understand the order patterns to forecast demand better. Create an Orders trend (number of orders as well as value) across months. This will allow us to gauge which months were best for the company from a sales standpoint.
8. We want to understand which country fared how well in terms of number of orders and average order value. Plot both values by country on a map.
9. In each category and gender of customers, what % of customers did not place an order.
10. Which order source proved to be most used by customers across various countries? Plot an appropriate chart to demonstrate the same.
11. The category of customers stores a lot of hidden insights. Which Category of customers:
* Has most Indian males
* Is the youngest on average
* Has the highest sales
* Has the greatest number of Sales POCs in the Delta team
Show all this data using Appropriate Charts.
12.	Create a ‘Sales Targets’ page. Create a KPI chart w.r.t actual sales and target sales. The page must include Sales POC, Sales Manager and Sales Team slicers.
13.	Add a Q&A for increasing interactivity of the report.
14.	Create a Drill Through report from a Map of Total Sales in each country to the Sales Managers’ individual sales in those countries.
15.	Beautify the report using colours, themes, buttons, borders, shadows and more.
16.	To present the sales data to stakeholders, create a Slideshow using Bookmarks: a bookmark for each Sales Team.
17.	Many of your report viewers will see the report on their mobile. Create a compelling Mobile View for them: it should only include the top 4-5 visuals per page.
18.	Create roles for all Sales teams for row level security. Each sales team must view the data only for their team and only for the POCs whose Sales Target was not met.
19.	Create an Admin role: who can see all the data corresponding to all teams.
20.	Save and share the PBIX file.

## Solution Approach
