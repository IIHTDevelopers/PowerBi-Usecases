Objective: This README guides you through using the provided datasets to practice data cleaning, transformations, and analysis tasks in Power BI.

1. Overview of Datasets
Datasets Included:

CustomerData.csv
ProductData.csv
SalesData.csv

Each dataset has been intentionally modified with errors such as duplicates, missing values, inconsistent formatting, and incorrect data types to help you practice various data-cleansing and preparation tasks.

2. Power BI Task Instructions with Hints
A. Data Cleaning and Transformation with Power Query

Remove Duplicates:

Hint: Use Power Query’s “Remove Duplicates” function to identify and remove repeated entries. Check for duplicates in key columns (e.g., CustomerID, ProductID) in each table.
Handle Missing Values:

Hint: Use the “Replace Values” or “Fill Down” options in Power Query to handle missing data. For numeric columns (e.g., SalesAmount, Quantity, UnitCost), decide if missing values should be replaced with a default value (e.g., zero) or removed if necessary.
Standardize Text Fields:

Hint: Apply text transformations (e.g., “Lowercase,” “Uppercase,” or “Capitalize Each Word”) to columns like Region, ProductCategory, and Industry to ensure consistent formatting.
Correct Data Types:

Hint: Set the correct data type for each column, especially for SalesAmount, Quantity, and UnitCost, which should be numeric. For columns with non-numeric entries (e.g., “ErrorValue”), use the “Replace Errors” function to manage or remove them.
Convert SaleDate to Date Format:

Hint: If SaleDate is not already in date format, use Power Query’s “Data Type” transformation to convert it to a Date format.
B. Calculated Columns and Measures using DAX

Profit Margin:

Hint: Create a calculated column using DAX with the formula (UnitPrice - UnitCost) * Quantity in the SalesData table. Use RELATED to reference UnitCost from ProductData if necessary.
Customer Engagement Score:

Hint: Calculate a customer score based on metrics such as the total SalesAmount and the number of transactions. Use DAX functions like SUM and COUNT to develop this score.
Sales Growth Rate:

Hint: Use DAX time intelligence functions to calculate the growth rate by comparing current and previous periods (e.g., Year-over-Year growth).
Average Sales Per Transaction:

Hint: Use AVERAGE in DAX on the SalesAmount column to compute the average sales per transaction.
Customer Lifetime Value (CLV):

Hint: Calculate CLV by multiplying Average Sales Per Transaction by an assumed customer lifespan or count of repeat transactions.
C. Key Performance Indicators (KPIs)

Top 10 Customers by Revenue:

Hint: Create a visual sorted by total SalesAmount to identify the top customers.
Product Category Performance:

Hint: Use a bar chart to visualize total sales by ProductCategory.
Regional Sales Analysis:

Hint: Use a map or heat map to display sales distribution by Region.
D. Advanced Visualizations

Customer Segmentation by Industry:

Hint: Use a pie or donut chart to segment customers by Industry.
Sales Trends by Region and Product Category:

Hint: Use line or bar charts to compare sales trends over time by Region or ProductCategory.
Top Products by Sales:

Hint: Display a ranking of products by total SalesAmount.
Heat Map of Sales by Region and Product Category:

Hint: Use a matrix or heat map visual to analyze regional sales across different product categories.
E. Drill-Through Functionality

Hint: Enable drill-through by setting specific report pages to focus on customer or product details. This will allow users to click on a data point and view more detailed information.
F. Dynamic Reporting with Slicers and Filters

Add Slicers:
Hint: Add slicers for Date, Region, and ProductCategory to create interactive filtering on the dashboard.
G. Custom Tooltips and Interactions

Hint: Customize tooltips to provide additional context (e.g., show Profit Margin when hovering over a sales data point).
H. Bookmarks for Dashboard Views

Create Bookmarks:
Hint: Save specific report views using bookmarks to allow users to switch perspectives based on their role or interest (e.g., Sales View, Product View).
3. Saving and Exporting Files
After performing the tasks:

Save the Power BI file with a descriptive name (e.g., NovaTech_CaseStudy.pbix).
Export the report visuals and save the modified CSV files to document your data-cleaning steps