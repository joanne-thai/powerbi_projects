# Pizza Sales Analytics Dashboard (Power BI)

## Overview

This project presents an end-to-end analysis of pizza sales performance using Power BI, focusing on revenue drivers, customer behaviour, product performance, and operational patterns. The dataset captures transactional sales across a full year, enabling a comprehensive evaluation of business performance.

The analysis shows that the business is supported by stable demand and a strong core of high-performing products, while also revealing opportunities to optimise product mix, pricing strategy, and operational efficiency.

---

## Objectives

The goal of this project is to transform transactional sales data into actionable business insights. The dashboard aims to evaluate overall performance, identify peak demand patterns, understand customer purchasing behaviour, assess product and ingredient efficiency, and support data-driven decision making.

---

## Dataset

The dataset covers a full year of operations, generating approximately **$817.9K in revenue** from **21K orders** and **50K pizzas sold**. Customers purchase an average of **2 pizzas per order**, resulting in an average order value of **$38.3**.

The data includes product details, order quantities, timestamps, and ingredient-level information, allowing analysis across time, product, and operational dimensions.

---

## Data Model

The project follows a structured modelling approach using a central transactional table supported by derived summary tables. Aggregated tables are created to support product-level analysis, ingredient impact evaluation, and menu engineering segmentation.

This approach enables efficient calculation of key metrics, correlation analysis, and performance comparisons across products and categories.

---

## Key Insights

Sales performance remains stable throughout the year, indicating consistent demand rather than strong seasonality. Revenue is driven primarily by predictable lunch and evening peaks, with the highest sales occurring between **12 PM and 3 PM**, followed by strong end-of-week performance, particularly on Fridays.

Customer behaviour shows a strong preference for multi-item purchases, with **over 60% of orders containing multiple pizzas**. This highlights the importance of bundling strategies and value-based purchasing behaviour.

At the category level, Classic pizzas lead in both volume and revenue, while other categories contribute relatively evenly, suggesting a balanced product portfolio. However, differences between demand and revenue indicate that higher sales volume does not always translate into higher value contribution.

Product-level analysis reveals a clear performance gap, where a small number of pizzas generate the majority of revenue, while several items contribute minimally. This indicates inefficiencies in the product portfolio and opportunities for optimisation.

Ingredient analysis shows that demand is concentrated around a few key ingredients, while others are rarely used, suggesting inefficiencies in inventory management. Not all ingredients contribute equally to revenue, highlighting opportunities to improve procurement and reduce waste.

Menu engineering further confirms that **over half of total revenue is driven by top-performing products**, while a significant portion of the menu underperforms. This imbalance highlights the need for a more strategic product mix.

---

## Dashboard Features

The dashboard is structured to provide both high-level and detailed views of performance. The overview page highlights key metrics, sales trends, and peak demand patterns. Product-focused views provide insights into category performance, product rankings, and sales distribution. Ingredient and segmentation visuals support deeper analysis of operational efficiency and menu design.

Interactive filters allow users to explore performance across time, product categories, and individual items.

---

## Techniques Used

This project applies a range of analytical techniques, including time-based analysis, product performance ranking, ingredient impact evaluation, and menu engineering segmentation. DAX is used extensively to calculate key metrics, revenue contribution, and performance comparisons.

Advanced analysis includes revenue versus demand segmentation, correlation-based evaluation, and distribution analysis to identify inefficiencies and opportunities.

---

## Recommendations

Operational resources should be aligned with peak demand periods, particularly during lunch hours and end-of-week periods, to improve efficiency and service delivery.

The strong presence of multi-item orders suggests that bundling and upselling strategies can further increase average order value and revenue.

The product portfolio should be optimised by focusing on high-performing items while reviewing or redesigning underperforming products. Ingredient usage should be streamlined by prioritising high-demand components and reducing low-usage inventory.

Applying menu engineering principles more strategically can help improve the balance of the product portfolio and maximise overall revenue contribution.

---

## Conclusion

This project demonstrates how transactional sales data can be transformed into meaningful business insights. By combining structured data modelling, analytical techniques, and effective visualisation, the dashboard provides a clear understanding of performance drivers and operational opportunities.

The results highlight both the strengths of the current business model and areas for improvement, supporting more informed and strategic decision making.

---

## Tools & Technologies

- Power BI
- DAX (Data Analysis Expressions)
- Data Modelling
- Data Visualisation