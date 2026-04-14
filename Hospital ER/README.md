![Hospital ER hero](./images/hero.png)

# Emergency Room Operations Analytics

Understanding patient flow, waiting times, and referral patterns to improve ER operations.

[![Open Interactive Power BI Report](https://img.shields.io/badge/Open-Interactive%20Power%20BI-F2C94C?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiYzgzYTQ2ZmItYTJiZS00NGFkLWI3ZjgtYzVlOWZjZDY1MDFkIiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)
[![Open PBIX File](https://img.shields.io/badge/Open-PBIX%20File-2F855A?style=for-the-badge)](./hospital_er_project.pbix)
[![Back to All Projects](https://img.shields.io/badge/Back-All%20Projects-4C51BF?style=for-the-badge)](../README.md)

> GitHub does not support live Power BI iframes inside README files, so the dashboard preview below links out to the interactive report.

## At a Glance

| Area | Details |
| --- | --- |
| Business problem | Clarify when ER demand peaks, how patient experience behaves, and which referral pathways create the most operational pressure. |
| Dataset scope | 9,216 patient visits from April 2019 to October 2020 with timing, waiting time, satisfaction, demographics, admissions, and referrals. |
| Tools | Power BI, DAX, Data Modelling, Data Visualization |
| Analysis focus | Time-series analysis, operational flow analysis, correlation analysis, demographic segmentation |

## Dashboard Preview

[![Hospital ER dashboard preview](./images/dashboard-preview.png)](https://app.powerbi.com/view?r=eyJrIjoiYzgzYTQ2ZmItYTJiZS00NGFkLWI3ZjgtYzVlOWZjZDY1MDFkIiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)

## Overview

This project analysed emergency room operations to surface demand patterns, patient experience drivers, and workflow bottlenecks across more than a year of patient visits.

## Business Problem

The ER needed a clearer operational picture of when demand peaked, how waiting time related to satisfaction, and which patient groups and referral pathways created the most pressure on service delivery.

## Dataset

The dataset spans April 2019 to October 2020 and includes 9,216 patient visits. It captures visit timing, admission status, waiting time, satisfaction score, patient demographics, and referral activity, modelled with a main `Hospital ER` table supported by `DimDate` and `DimTime`.

## Approach

- Built operational KPIs in Power BI to track patient volume, waiting time, satisfaction, admissions, and referral counts.
- Used time-based analysis to identify demand peaks by weekday and hour.
- Segmented patients by age, gender, and referral outcome to understand service mix and escalation patterns.
- Tested the relationship between waiting time and satisfaction using patient-level correlation analysis.

## Key Insights

- Demand is steady across the period, with the busiest periods occurring on Mondays and during midday to evening hours.
- Average waiting time is about 35 minutes and average satisfaction is 5.47 out of 10, but waiting time alone shows almost no linear relationship with satisfaction.
- Most visits do not require referrals, while General Practice and Orthopedics account for the largest share of referred cases.

## Recommendations

- Align staffing and operational resources more closely to midday and early-week demand peaks.
- Introduce or expand fast-track pathways for non-critical patients to reduce congestion and improve flow.
- Improve patient experience through clearer communication and service consistency, not just shorter wait times.

## Tools Used

- Power BI
- DAX
- Data Modelling
- Data Visualization

## Project Visuals

| Cover | Dashboard |
| --- | --- |
| ![Hospital ER cover](./images/hero.png) | ![Hospital ER dashboard](./images/dashboard-preview.png) |

## Repository Contents

| File | Purpose |
| --- | --- |
| [`hospital_er_project.pbix`](./hospital_er_project.pbix) | Power BI dashboard file |
| [`Hospital ER.csv`](./Hospital%20ER.csv) | Source dataset used for analysis |
| [`images/hero.png`](./images/hero.png) | Project cover image used in the README |
| [`images/dashboard-preview.png`](./images/dashboard-preview.png) | Dashboard screenshot preview |
