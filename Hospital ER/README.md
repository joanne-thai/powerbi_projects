![Hospital ER hero](./images/hero.png)

# Emergency Room Operations Analytics

Understanding patient flow, waiting times, and referral patterns to improve ER operations.

[![Open Interactive Power BI Report](https://img.shields.io/badge/Open-Interactive%20Power%20BI-F2C94C?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiYzgzYTQ2ZmItYTJiZS00NGFkLWI3ZjgtYzVlOWZjZDY1MDFkIiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)
[![Open PBIX File](https://img.shields.io/badge/Open-PBIX%20File-2F855A?style=for-the-badge)](./hospital_er_project.pbix)
[![Back to All Projects](https://img.shields.io/badge/Back-All%20Projects-4C51BF?style=for-the-badge)](../README.md)

## At a Glance

| Area | Details |
| --- | --- |
| Business problem | Clarify when ER demand peaks, how patient experience behaves, and which referral pathways create the most operational pressure. |
| Dataset scope | 9,216 patient visits from April 2019 to October 2020 with timing, waiting time, satisfaction, demographics, admissions, and referrals. |
| Tools | Power BI, DAX, Data Modelling, Data Visualisation |
| Analysis focus | Time-series analysis, operational flow analysis, correlation analysis, demographic segmentation |

## Dashboard Preview

[![Hospital ER dashboard preview](./images/dashboard-preview.png)](https://app.powerbi.com/view?r=eyJrIjoiYzgzYTQ2ZmItYTJiZS00NGFkLWI3ZjgtYzVlOWZjZDY1MDFkIiwidCI6IjhiNmM0ZDY5LTc5OTMtNDgyYy04OGU5LTZmOWM5ZjlhMDBiOSJ9)

## Overview

This project analyses emergency room (ER) data to understand patient flow, waiting times, and satisfaction levels. The goal is to identify operational bottlenecks and areas for improvement in service delivery.

The dataset covers April 2019 to October 2020, with a total of 9,216 patient visits.

## Business Problem

The ER needs to manage patient demand efficiently while maintaining a good level of service. Key questions include:

- How long are patients waiting, and is it within target?  
- What factors affect patient satisfaction?  
- When does demand peak, and are resources aligned?  
- Which departments or patient groups require attention?  

Without clear visibility into these areas, it becomes difficult to improve patient experience, reduce delays, and allocate resources effectively.

## Key Metrics
- Total Patients: 9,216  
- Avg Waiting Time: 35.26 minutes  
- Avg Satisfaction Score: 5.47 / 10  
- Total Patients Referred: 3,816  
- Patients Within Target Waiting Time: ~59%  
- Patients Missing Target: ~41%  

## Data Model
The dataset is structured around patient-level records, including:

- Patient details (age, gender, race)  
- Visit information (date, hour, admission status)  
- Department referrals  
- Waiting time and satisfaction score  

Given the relatively small size of the dataset, it is kept in a single table rather than being fully normalised into separate fact and dimension tables. This simplifies the model and avoids unnecessary complexity while still supporting all required analysis.

## Approach

- Built operational KPIs in Power BI to track patient volume, waiting time, satisfaction, admissions, and referral counts.
- Used time-based analysis to identify demand peaks by weekday and hour.
- Segmented patients by age, gender, and referral outcome to understand service mix and escalation patterns.
- Tested the relationship between waiting time and satisfaction using patient-level correlation analysis.

## Analysis

### 1. Patient Flow & Admission Status
**Visuals Used:** Patient Admission Status, Total Patients KPI  

- The number of admitted (4,612) and non-admitted patients (4,604) is almost evenly split.
- The ER is handling a balanced mix of critical and non-critical cases.

**Impact:**  
This can create pressure on resources, as both types of patients require different levels of attention and care.

### 2. Waiting Time Performance
**Visuals Used:** Avg Waiting Time KPI, Total Patients by Waittime Status  

- The average waiting time is 35.26 minutes. Around 59% of patients are seen within the target time, while 41% experience delays.
- A significant portion of patients are not being seen within the expected timeframe.

**Impact:**  
Delays can affect patient experience and indicate capacity or process inefficiencies.

### 3. Patient Demand by Time
**Visuals Used:** Total Patients by Day and Hour (Heatmap & Bar Chart)  

- Patient volume varies by both day and hour, with clear peak periods.
- Demand is not evenly distributed and spikes during certain hours.

**Impact:**  
If staffing does not match these peak periods, it can lead to longer waiting times and overcrowding.



## Key Insights

- The ER handled **9,216 patient visits** across a **19-month** period, with average waiting time at about **35 minutes** and average satisfaction at **5.47 out of 10**. This points to a consistently busy service with moderate patient experience and clear room to improve the operational journey.
- Demand is steady rather than erratic, with the heaviest pressure falling on **Mondays**, followed by **Tuesdays** and **Saturdays**, and activity clustering around midday to evening hours. Because those peaks are predictable, staffing and flow interventions can be timed more precisely instead of treating congestion as random.
- Waiting time on its own does not explain the experience gap as well as teams might expect. The report shows an almost zero linear relationship between waiting time and satisfaction at **-0.002**, which suggests communication, care quality, and treatment outcomes likely matter more than speed alone for many patients.
- Referral activity shows that a large share of visits are relatively low-acuity, with roughly **5,400** patients needing no referral at all, while **General Practice (~1,800)** and **Orthopedics (~1,000)** handle the largest referred volumes. The patient base is concentrated in the **20-39** age range, gender split is balanced, and admissions are close to **50/50**, indicating a fairly even triage mix between patients who require further treatment and those who can be discharged.

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
