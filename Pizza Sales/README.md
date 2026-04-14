![Pizza Sales hero](./images/hero.png)

# Pizza Sales & Product Performance Analytics

Linking sales patterns, menu performance, and ingredient usage to smarter product decisions.

[![Open Interactive Power BI Report](https://img.shields.io/badge/Open-Interactive%20Power%20BI-F2C94C?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiZmI2M2FiNDgtYTIzMy00NmIzLWFjZWUtNzk2YzZiZjU1NWViIiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)
[![Open PBIX File](https://img.shields.io/badge/Open-PBIX%20File-2F855A?style=for-the-badge)](./pizza_sales_project.pbix)
[![Back to All Projects](https://img.shields.io/badge/Back-All%20Projects-4C51BF?style=for-the-badge)](../README.md)

> GitHub does not support live Power BI iframes inside README files, so the dashboard preview below links out to the interactive report.

## At a Glance

| Area | Details |
| --- | --- |
| Business problem | Identify which products and categories drive revenue, where menu inefficiency sits, and how operational demand patterns should shape staffing and inventory decisions. |
| Dataset scope | Full-year pizza sales transactions with product, quantity, timestamp, and ingredient-level information. |
| Tools | Power BI, DAX, Data Modelling, Data Visualization |
| Analysis focus | Time-series analysis, product performance analysis, menu engineering segmentation, demand vs revenue analysis |

## Dashboard Preview

[![Pizza Sales dashboard preview](./images/dashboard-preview.png)](https://app.powerbi.com/view?r=eyJrIjoiZmI2M2FiNDgtYTIzMy00NmIzLWFjZWUtNzk2YzZiZjU1NWViIiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)

## Overview

This project turned a full year of pizza sales transactions into a clear view of revenue drivers, customer order behaviour, menu efficiency, and operational demand patterns.

## Business Problem

The business needed to understand which products and categories were truly driving revenue, whether customer demand translated into value, and where menu and inventory inefficiencies were limiting performance.

## Dataset

The dataset covers a full year of operations, generating about $817.9K in revenue from 21K orders and 50K pizzas sold. It includes product details, quantities, timestamps, and ingredient-level information, with derived summary tables supporting product, ingredient, and menu engineering analysis.

## Approach

- Built KPI measures for revenue, orders, pizzas sold, average pizzas per order, and average order value.
- Analysed sales by daypart, weekday, category, and product to isolate stable demand patterns and peak periods.
- Used menu engineering and demand-versus-revenue comparisons to classify product performance.
- Evaluated ingredient concentration and low-usage components to identify inventory and procurement inefficiencies.

## Key Insights

- The business generated approximately **$817.9K** in revenue from **21K orders** and **50K pizzas sold**, with an average order value of about **$38.3** and roughly **2 pizzas per order**. Sales are stable across the year with only minor fluctuations, which suggests a dependable business pattern rather than sharp seasonality.
- Demand is concentrated in very specific trading windows. **Fridays** are the strongest sales day, followed by **Thursdays** and **Saturdays**, while the **12 PM - 3 PM** period drives the highest revenue and evening hours provide the next-largest contribution, making lunch and dinner the critical operating dayparts.
- Order composition is a real commercial strength, not just a descriptive stat. Around **61.6%** of orders contain multiple pizzas, which confirms strong bundle-style purchasing behaviour and creates a solid case for combo offers, upselling, and promotions designed around multi-item baskets.
- Category and product performance are uneven in ways that matter strategically. **Classic** pizzas lead both in volume and revenue at roughly **$220K**, while products such as **The Classic Deluxe Pizza** and **Barbecue Chicken Pizza** stand out against weaker items like **The Brie Carre Pizza** and **Mediterranean Pizza**, showing that menu breadth is not translating evenly into value.
- Ingredient and menu-engineering analysis both point to portfolio inefficiency. High-usage ingredients such as **Garlic**, **Tomatoes**, and **Red Onions** dominate demand, while low-usage ingredients add complexity with limited payoff; at the same time, top performers contribute about **51.5%** of revenue while underperformers still account for about **37.5%**, reinforcing the need to simplify and rebalance the menu.

## Recommendations

- Staff and prep more aggressively for lunch and end-of-week peaks to support faster service during high-demand periods.
- Use bundles and upsell offers to build on strong multi-item ordering behaviour and increase average order value.
- Refine the menu by prioritising high-performing pizzas and reducing low-value products and ingredients that add complexity without strong revenue contribution.

## Tools Used

- Power BI
- DAX
- Data Modelling
- Data Visualization

## Project Visuals

| Cover | Dashboard |
| --- | --- |
| ![Pizza Sales cover](./images/hero.png) | ![Pizza Sales dashboard](./images/dashboard-preview.png) |

## Repository Contents

| File | Purpose |
| --- | --- |
| [`pizza_sales_project.pbix`](./pizza_sales_project.pbix) | Power BI dashboard file |
| [`data_pizza.xlsx`](./data_pizza.xlsx) | Source dataset used for analysis |
| [`data_dictionary.xlsx`](./data_dictionary.xlsx) | Data dictionary for business fields and definitions |
| [`images/hero.png`](./images/hero.png) | Project cover image used in the README |
| [`images/dashboard-preview.png`](./images/dashboard-preview.png) | Dashboard screenshot preview |
