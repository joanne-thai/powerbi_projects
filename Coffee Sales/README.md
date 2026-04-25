![Coffee Sales hero](./images/hero.png)

# Coffee Sales Analytics: Pricing, Demand & Product Insights

Pinpointing which pricing and category shifts could unlock revenue growth across stores.

[![Open Interactive Power BI Report](https://img.shields.io/badge/Open-Interactive%20Power%20BI-F2C94C?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiNzlmYjhiMGItMjBkZC00ZGQ1LTgzODgtNjAzYWI2NDQyNTU5IiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)
[![Open PBIX File](https://img.shields.io/badge/Open-PBIX%20File-2F855A?style=for-the-badge)](./coffee_sales_project.pbix)
[![Back to All Projects](https://img.shields.io/badge/Back-All%20Projects-4C51BF?style=for-the-badge)](../README.md)


## At a Glance

| Area | Details |
| --- | --- |
| Business problem | Understand which products, pricing patterns, and operating periods are driving store-level sales performance. |
| Dataset scope | Multi-store transactional sales with product, quantity, price, timestamp, and location data. |
| Tools | Power BI, Python, Excel, DAX |
| Analysis focus | EDA, trend analysis, pricing strategy, demand analysis, product segmentation, KPI design |

## Dashboard Preview

[![Coffee Sales dashboard preview](./images/dashboard-preview.png)](https://app.powerbi.com/view?r=eyJrIjoiNzlmYjhiMGItMjBkZC00ZGQ1LTgzODgtNjAzYWI2NDQyNTU5IiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)

## Overview

This project analyses coffee shop transaction data to create a decision-ready view of revenue drivers, product performance, pricing behaviour, and time-based demand patterns across multiple store locations, with the goal of understanding customer spending and identifying practical opportunities to improve performance.

The dataset covers January to June 2023, generating approximately $698.8K in Total Sales across 149,116 Orders.

## Business Problem

The business needs to understand:

- Which products and categories drive Total Sales  
- How pricing affects demand  
- Which products perform well and which do not  
- Whether sales are growing steadily over time  

Without this, it is difficult to make decisions around pricing, product focus, and growth.

## Dataset

The dataset contains transactional sales across multiple stores, including product details, quantities sold, unit prices, timestamps, and store locations. A star schema model was built around a central fact table with supporting product, store, date, and time dimensions, plus a derived product summary table for segmentation analysis.

## Approach

- Modelled the data using a star schema with `fact_Sales` supported by product, store, date, and time dimensions.
- Built DAX measures for sales, orders, quantity sold, average unit price, and other comparative KPIs.
- Used correlation analysis and quadrant-style product segmentation to examine price, demand, and revenue relationships.
- Designed three analytical views covering monthly performance, product insights, and sales drivers with short-term forecasting.

## Key Metrics

- Total Sales: $698.8K  
- Orders: 149,116  
- Quantity Sold: 214,470  
- Avg Unit Price: $3.26  
- Avg Daily Sales: ~$3.9K  
- Revenue at Risk: $125.4K

## Analysis

### 1. Sales Distribution by Product
**Visuals Used:** Sales by Products (Treemap), Ranking by Sales (Bar Chart)

- Sales are unevenly distributed across products and categories. Coffee (\~$269.9K) and Tea (\~$196.4K) are the clear revenue engines of the business, with total revenue reaching about **$698.8K** from **149K orders** and **214K items sold**.
- A relatively small group of top-performing products drives most sales, while underperforming items still contribute roughly **15-20%** of revenue, pointing to clear product-mix inefficiency.

This shows that a small number of categories drive most of the revenue.

### 2. Customer Spending Behaviour
**Visuals Used:** Quantity Sold by Category (Area Chart), Sales by Products (Treemap)

- Categories with higher Total Sales also show higher Quantity Sold, especially Coffee and Tea.

This suggests that customers tend to repeatedly purchase the same core products, and revenue is driven by frequent purchases rather than one-time orders.

### 3. Price vs Demand
**Visual Used:** Price vs Demand (Scatter Plot)

Pricing behaves differently depending on the level of analysis.

- At the product level, higher prices are associated with lower demand, with a correlation of **-0.68**, showing meaningful price sensitivity.

This shows that customers buy less as prices increase, indicating price sensitivity across products.

### 4. Sales & Avg Unit Price Correlation by Store
**Visual Used:** Sales & Avg Unit Price Correlation by Store

- At the store level, there is a strong positive relationship (correlation = 0.93) between Avg Unit Price and Total Sales.

This does not mean that increasing the price leads to higher sales. Instead, higher-performing stores tend to have higher average prices, likely due to stronger demand, location differences, or product mix.
  
### 5. Product Positioning
**Visuals Used:** Product Positioning (Scatter Plot), Menu Class Breakdown

Products are grouped based on Total Sales and Quantity Sold:

- Top Performers: high sales and high volume  
- Growth Opportunities: high sales but lower volume  
- Volume Drivers: high volume but lower sales per item  
- Underperformers: low sales and low volume  

Underperforming products contribute approximately $125.4K in Total Sales.

### 6. Sales Trend & Forecast
**Visuals Used:** Sales Trend (Line Chart), Forecast

Demand patterns are highly routine, which makes them operationally useful.

- Total Sales show a steady increase from January to June, with Avg Daily Sales around **$3.9K**. The forecast suggests continued stable growth.
- Morning periods are consistently strong across the week, and Evening periods show occasional spikes that create additional upside rather than replacing core demand.

This indicates consistent demand without major fluctuations.

## Key Insights

- The business generates approximately $698.8K in Total Revenue from 149K orders and 214K items sold, with around 74% of transactions occurring on weekdays. Revenue is heavily concentrated in a small number of key categories, particularly Coffee and Tea, and customer behaviour is largely driven by repeat purchases, making high-frequency products critical to maintaining consistent sales performance.
- Pricing plays a significant but nuanced role. At the product level, higher prices are associated with lower demand, indicating clear price sensitivity. However, at the store level, stronger locations are able to sustain higher average prices, suggesting that performance differences are influenced by demand conditions, location, and product mix rather than pricing alone.
- The current product mix is not fully optimised. Underperforming products still contribute approximately $125.4K in Total Sales, highlighting inefficiencies, while clear product groupings create opportunities for better positioning and performance improvement.
- Store performance is relatively balanced overall, indicating that growth is less about fixing a single weak location and more about portfolio optimisation, better promotion timing, and activating off-peak demand to unlock additional revenue.

## Recommendations

The analysis suggests that growth opportunities lie in optimising product mix, refining pricing strategy, and leveraging demand patterns rather than making major structural changes.

### 1. Prioritise Top Performers  

- Focus product and promotional attention on high-performing core items, particularly Coffee and Tea.
- Maintain pricing strength on leading products and test targeted pricing changes only on weaker items with softer demand
- Ensure consistent availability and feature these items in bundles and promotions to reinforce their role as primary revenue drivers

Expected Impact: Protect and steadily grow the main sources of revenue.

### 2. Improve Growth Opportunities

- For products with strong sales but lower volume, apply targeted strategies such as slight pricing adjustments, increased visibility, and promotional efforts to encourage repeat purchases.

Expected Impact: Increase Quantity Sold while maintaining strong Total Sales

### 3. Optimise Volume Drivers

- For high-volume but lower-revenue products, introducing bundles to increase basket size  
- Test small price increases where demand remains stable and pair with higher-margin products

Expected Impact: Improve Total Sales per Order

### 4. Review Underperformers

- Evaluate underperforming items to determine whether they should be removed, repositioned, or repriced  
- Assess whether low performance is due to a lack of visibility or genuinely low demand.

Expected Impact: Reduce inefficiencies and focus on stronger products

### 5. Apply Store-Level Strategy

- Adjust pricing and product mix by store. Stronger locations may support premium pricing, while others may benefit from more competitive positioning
- Account for location-specific demand differences

Expected Impact: Better performance across different locations

### 7. Optimise Time-Based Operations  

- Align staffing levels with peak morning demand to reduce wait times and maintain service quality
- Avoid overstaffing during low-demand periods to improve cost efficiency
- Use targeted promotions and bundles to increase traffic during off-peak hours (afternoon/evening)
- Align inventory and preparation with predictable demand patterns to reduce stockouts and waste
- Leverage consistent demand trends to better plan scheduling and daily operations

Expected Impact: Improve operational efficiency, enhance customer experience, and unlock incremental revenue from underutilised time periods.

## Tools Used

- Power BI
- Python
- Excel
- DAX

## Project Visuals

| Cover | Dashboard |
| --- | --- |
| ![Coffee Sales cover](./images/hero.png) | ![Coffee Sales dashboard](./images/dashboard-preview.png) |

## Repository Contents

| File | Purpose |
| --- | --- |
| [`coffee_sales_project.pbix`](./coffee_sales_project.pbix) | Power BI dashboard file |
| [`data.xlsx`](./data.xlsx) | Source dataset used for analysis |
| [`images/hero.png`](./images/hero.png) | Project cover image used in the README |
| [`images/dashboard-preview.png`](./images/dashboard-preview.png) | Dashboard screenshot preview |
