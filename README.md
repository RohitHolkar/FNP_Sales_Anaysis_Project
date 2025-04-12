# FNP_Sales_Anaysis_Project

📊 Excel Power Query & Data Model Project – Sales Analysis Dashboard
This project demonstrates how to transform raw data into meaningful insights using Power Query, Excel Data Model, and Pivot Tables, culminating in a dynamic dashboard for business decision-making.

🔍 Data Cleaning & Transformation (Power Query)
Column Profile

Enabled Column Profile to get a quick summary of each column's data distribution and quality.

Data Type Conversion

Converted Phone Number column from Whole Number to Text to retain country codes like +91.

Date & Time Transformations

Extracted Month Name from delivery_date column using Date.MonthName.

Extracted Hour from both delivery_time and order_time using Time.Hour.

Custom Column

Created a new column Diff_Order_Time to calculate the difference between delivery_date and order_date.

🔗 Data Modeling
Merge Queries

Merged Order Table with Product Table using Left Join on a common key.

Load to Data Model

Loaded transformed tables into a new worksheet and added them to the Data Model.

Data Model Enhancements

Created a calculated column:
Revenue = Order[Price] * Order[Quantity]
Renamed column to Revenue.

📈 Pivot Table Analysis
Total Revenue

Inserted Pivot Table from Data Model.

Added Revenue from the Order table to Values.

Average Delivery Time

Added Diff_Order_Time to Values and selected Average.

Month-wise Revenue

Used Month field in Rows and Revenue in Values for monthly analysis.

Top Products by Revenue

Added Product Name in Rows, Revenue in Values, then sorted in descending order.

Top 10 Cities by Number of Orders

Used City in Rows, Order ID in Values (Count), filtered Top 10 by value.

Order Quantity vs Delivery Quantity

Used =CORREL(Order[Quantity], Order[Delivery Quantity]) to find correlation.

Revenue Comparison Between Occasions

Compared Revenue across categories like festivals or events using slicers.

📊 Dashboard Creation
Insert Charts & KPIs

Created charts for Revenue trends, Top Products, City-wise Orders.

Interactive Filters

Inserted Slicers for fields like Month, Product, and City.

Added Timeline for Order Date to filter visuals dynamically.

📌 Tools Used:

Microsoft Excel (Power Query, Pivot Table, Data Model)

Data Visualization (Bar, Line, Pie Charts, KPIs)

Interactive Elements (Slicers, Timeline)
