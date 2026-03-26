# ☕ Coffee Sales Dashboard (Power BI)

## Overview

This project presents an end-to-end analysis of coffee shop sales performance using Power BI, focusing on revenue drivers, pricing dynamics, product performance, and time-based demand patterns. The dataset captures transactional data across multiple store locations, product categories, and time periods, enabling a comprehensive evaluation of business performance.

The analysis shows that the business is driven by a strong core of high-performing products and consistent daily demand, while also revealing opportunities to optimise product mix, pricing strategy, and time-based sales performance.

---

## Objectives

The goal of this project is to transform raw transactional data into actionable business insights. The dashboard aims to identify key revenue drivers, understand customer purchasing behaviour, evaluate product performance, and uncover operational patterns that can support data-driven decision making.

---

## Dataset

The dataset contains sales transactions across multiple stores, including information on product details, pricing, quantities sold, order timestamps, and store locations. It enables analysis across several dimensions such as product category, time, and geography.

Key metrics derived from the dataset include total sales, total orders, total quantity sold, and average unit price.

---

## Data Model

The project follows a structured data modelling approach using a star schema. The central fact table (`fact_Sales`) captures transactional data, including sales amount, quantity, and unit price. This is supported by dimension tables such as `dim_Product`, `dim_Store`, `dim_Date`, and `dim_Time`, which provide descriptive attributes for analysis.

A derived `Product Summary` table is used for advanced analysis such as product segmentation and correlation calculations. This enables efficient evaluation of product performance and supports visuals such as scatter plots and portfolio classification.

---

## Key Insights

Revenue is highly concentrated in coffee and tea products, with a small number of top-performing items contributing the majority of total sales. This indicates a strong core product offering that drives business performance.

Pricing exhibits a dual impact on performance. At the product level, higher prices are associated with lower demand, indicating price sensitivity among customers. However, at the store level, higher average pricing is strongly correlated with increased revenue, suggesting that premium pricing strategies remain effective overall.

The product portfolio shows clear inefficiencies, as underperforming products still contribute a noticeable share of revenue despite lower performance. This highlights opportunities for optimisation through better product positioning and selection.

Sales patterns are consistent and predictable. Demand is strongest during morning hours across all days, reflecting routine consumption behaviour, while evening periods show higher peak sales driven by occasional spikes. Overall, sales remain stable with a slight upward trend over time.

---

## Dashboard Features

The dashboard is structured into three main analytical views to support different levels of insight. The Monthly Overview provides a high-level summary of key performance indicators, sales trends, and operational patterns. The Product Performance page focuses on product-level insights, including category performance, demand behaviour, and sales contribution. The Sales Drivers & Forecast page highlights key revenue drivers, product segmentation, and short-term sales forecasting.

Interactive slicers allow users to filter by date, store location, and product category, enabling flexible exploration of the data. Advanced visuals such as scatter plots, heatmaps, treemaps, and decomposition trees are used to present insights clearly and effectively.

---

## Techniques Used

This project applies a range of analytical and data modelling techniques to enhance insight quality. DAX is used extensively to calculate key metrics, growth rates, correlations, and custom aggregations. Correlation analysis is implemented to evaluate relationships between price, demand, and revenue. Product segmentation is performed using a quadrant-based approach to classify products into performance groups.

Time-based analysis is used to identify peak demand periods and consumption patterns, while forecasting techniques are applied to project short-term sales trends. The dashboard design emphasises clarity, consistency, and visual hierarchy to improve user experience.

---

## Recommendations

The analysis suggests that the product mix should be optimised by reviewing underperforming items for potential removal, repositioning, or bundling, while focusing resources on high-performing products. Pricing strategies should be maintained for strong-performing products, with targeted adjustments applied to weaker items to improve demand.

Growth opportunity products should be further developed through increased visibility and promotion, with the aim of converting them into stronger contributors. Operational efficiency can be improved by aligning staffing and inventory with peak morning demand and leveraging evening sales opportunities through targeted campaigns.

---

## Conclusion

This project demonstrates how data can be used to uncover meaningful insights into business performance and support strategic decision making. By combining data modelling, analytical techniques, and effective visualisation, the dashboard provides a clear and actionable view of sales performance across multiple dimensions.

The results highlight both the strengths of the current business model and the opportunities for improvement, making this analysis a valuable tool for driving future growth.

---

## Tools & Technologies

- Power BI
- DAX (Data Analysis Expressions)
- Data Modelling (Star Schema)
- Data Visualisation
