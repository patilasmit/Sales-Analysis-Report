# Sales Analysis Dashboard with Power BI

This project is a comprehensive sales analysis dashboard built in Power BI to provide actionable insights into sales performance across different time periods, product categories, and regions. The dashboard showcases key metrics such as revenue, gross profit, and growth trends (Month-over-Month and Quarter-over-Quarter).
It is designed to help businesses visualize data trends, identify growth opportunities, and monitor performance effectively. This project also includes DAX measures for advanced calculations and a well-structured date table to enhance time-based analysis.

# Key Features
Dynamic Filters:
Country-level filtering (Czech Republic, Denmark, Germany).
Year and month filters for flexible time-based analysis.

# KPI Metrics:
Total Units Sold: Track the quantity sold across all products.
Gross Profit (87M): Measure profitability after deducting costs.
Total Revenue (126M): Total revenue generated from sales.

# Visual Insights:
Pie Chart: Revenue contribution by subcategories (Extra, Super, Micro, Regular).
Bar Chart: Revenue breakdown by product name and subcategories.
Line Charts:
Month-over-Month (MoM) growth trends.
Quarter-over-Quarter (QoQ) growth trends.
Table View: Average revenue across months with dynamic trend indicators (arrows for up/down trends).

# Advanced Calculations with DAX:
Time Intelligence: Month names, week numbers, and previous period calculations.
Profitability Analysis: Total cost, gross profit, and growth metrics.
Custom Growth Metrics: Month-over-Month and Quarter-over-Quarter growth rates.

# DAX Calculations
Date Table
DateMaster: Created using CALENDAR() to generate a complete date range for analysis.
Derived Columns: Year, month name, week numbers, and weekday names for granular filtering and analysis.

# Metrics
Revenue Calculation:
Total Revenue = Sales[Units] * RELATED('Product'[RetailPrice])
Captures total revenue from product sales.
Profitability:
Gross Profit = Sales[Total Revenue] - Sales[Total Cost]
Measures the profitability of sales.
Growth Analysis:
Month-over-Month (MoM) Growth:
([Total Profit] - [Previous Month GRP]) / [Previous Month GRP]
Tracks changes in profitability over months.
Quarter-over-Quarter (QoQ) Growth:
([Total Rev] - [Previous Quarter Revenue]) / [Previous Quarter Revenue]
Tracks revenue growth across quarters.

# Time Intelligence Functions
Previous Month and Previous Quarter metrics help in comparing sales performance with past periods.
Weekday and week number columns enhance granular insights.

# Key Learnings
Power BI Techniques:
Designing interactive dashboards with slicers and filters.
Customizing visualizations for better storytelling.

# DAX Mastery:
Creating time-intelligence functions for advanced growth analysis.
Writing complex measures for profitability and cost analysis.

# Data-Driven Insights:
Understanding trends in revenue and profit over time.
Identifying top-performing products and regions.

# Use Cases
Business Performance Monitoring:
Track key metrics like revenue, profit, and sales growth to assess business health.
Product Insights:
Identify top-performing products and subcategories for strategic decisions.
Time-Based Analysis:
Monitor sales trends over months, quarters, and years.
