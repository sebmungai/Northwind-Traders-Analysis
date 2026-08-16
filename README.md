 Northwind Traders Sales and Profitability Analysis

## Project Overview

This project is a Power BI dashboard built on the Northwind Traders dataset. It analyzes sales performance and product/category profitability over a multi year period (July 1996 to May 1998), giving a full picture of revenue trends, order behavior, and which products and categories drive the business.

The file `Northwind_Traders_analysis.pbix` contains the full interactive report with two pages:

1. Sales Performance Overview
2. Product and Category Profitability

## Objectives

The dashboard was built to answer these core business questions:

1. How is total revenue trending month over month and year over year?
2. Which product categories generate the most revenue and quantity sold?
3. Which individual products contribute most to revenue?
4. What is the average order value and how many orders are being placed?
5. How does revenue growth vary across categories (Revenue YoY %)?

## Tools Used

Power BI Desktop, used to build the data model, DAX measures, and interactive report
DAX (Data Analysis Expressions), used for calculated measures such as Total Revenue, Revenue YoY %, Revenue MoM Growth, and Average Order Value
Northwind Traders sample database as the data source (Orders, Order Details, Products, Categories tables)
Power Query, used for data cleaning and shaping prior to modeling

## Report Pages and Analysis

### 1. Product and Category Profitability

![Product and Category Profitability]https://github.com/sebmungai/Northwind-Traders-Analysis/blob/main/IMAGES/PRODUCT%20AND%20CATEGORY%20PROFITABILITY.png
This page drills into category and product level profitability.

Key metrics (KPI cards):
Revenue YoY %: 178.29 percent
Total Quantity Sold: 51K
Revenue Prior Month: 1.33M
Revenue MoM Growth: 1.49 percent

Visuals:
Total Revenue and Total Quantity Sold by CategoryName, comparing revenue and units sold side by side for each category
Total Revenue by ProductName, ranking top individual products by revenue
A summary table breaking down each category by Total Revenue, Total Quantity Sold, and Revenue YoY %


### 2. Sales Performance Overview

![Sales Performance Overview]https://github.com/sebmungai/Northwind-Traders-Analysis/blob/main/IMAGES/SALES%20PERFORMANCE%20OVERVIEW.png
This page tracks overall business performance across time.

Key metrics (KPI cards):
Total Revenue: 1.35M
Total Quantity Sold: 51,317
Order Count: 830
Average Order Value: 1.63K

Visuals:
Total Revenue and Order Count by Month (area/line chart) showing a generally upward trend in both revenue and order count from mid 1996 through early 1998, with a dip around September and a strong finish into the spring months
Total Quantity Sold by Month Year showing quantity sold trending downward over the period, which combined with rising revenue suggests an increase in average selling price or a shift toward higher value products
Total Revenue by CategoryName (bar chart) ranking categories by revenue contribution
Total Revenue by CategoryName (donut chart) showing the percentage share each category holds, led by Beverages at 21.15 percent, followed by Dairy Products at 18.56 percent and Confections at 13.16 percent

Category level breakdown from the summary table:

Beverages: 286,526.95 revenue, 9,532 units sold, 148.61 percent YoY
Condiments: 113,694.75 revenue, 5,298 units sold, 150.91 percent YoY
Confections: 177,099.10 revenue, 7,906 units sold, 147.54 percent YoY
Dairy Products: 251,330.50 revenue, 9,149 units sold, 185.32 percent YoY
Grains/Cereals: 100,726.80 revenue, 4,562 units sold, 215.87 percent YoY
Meat/Poultry: 178,188.80 revenue, 4,199 units sold, 196.11 percent YoY
Produce: 105,268.60 revenue, 2,990 units sold, 209.40 percent YoY
Seafood: 141,623.09 revenue, 7,681 units sold, 250.41 percent YoY
Total: 1,354,458.59 revenue, 51,317 units sold, 178.29 percent YoY

Both pages share the same filter panel, with a date range slicer (7/4/1996 to 5/6/1998) and a CategoryName dropdown, allowing the user to filter every visual on the page by time period and category.

## Key Insights

1. Beverages is the strongest category overall, leading in total revenue and holding the largest share of category revenue at just over 21 percent.
2. Seafood and Grains/Cereals show the fastest year over year growth, at 250.41 percent and 215.87 percent respectively, despite having lower total revenue than categories like Beverages or Dairy Products. This signals these categories may be smaller but rapidly gaining traction.
3. Revenue is growing faster than quantity sold. Total quantity sold trends downward over the period while total revenue trends upward, suggesting rising prices, a shift toward premium products, or larger average order values.
4. Overall business growth is strong, with Revenue YoY at 178.29 percent and steady month over month growth of 1.49 percent, plus a consistent upward trend in the monthly revenue chart.
5. Dairy Products and Confections round out the top performing categories alongside Beverages, together with Beverages accounting for over half of total category revenue share when combined.
6. Average order value sits at 1.63K across 830 orders, indicating a business built on relatively large individual transactions rather than high order volume.

## How to Use the Report

Open `Northwind_Traders_analysis.pbix` in Power BI Desktop
Use the Date range slicer to focus on a specific time window
Use the CategoryName dropdown to isolate a single product category across all visuals on the page
Navigate between the Sales Performance Overview and Product and Category Profitability pages using the navigation buttons on the left panel
