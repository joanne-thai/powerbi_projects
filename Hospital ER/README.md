# Healthcare ER Analytics Dashboard (Power BI)

## Overview

This project presents an end-to-end analysis of Emergency Room (ER) operations using Power BI, focusing on patient flow, operational efficiency, and patient experience. The dataset captures patient-level interactions over time, enabling a comprehensive evaluation of healthcare service performance.

The analysis reveals consistent demand patterns and highlights key operational challenges, while also identifying opportunities to improve efficiency and enhance patient experience.

---

## Objectives

The objective of this project is to transform patient-level data into actionable insights. The dashboard aims to analyse ER demand patterns, evaluate waiting time and satisfaction, understand patient demographics and referral behaviour, and support data-driven improvements in healthcare operations.

---

## Dataset

The dataset spans **April 2019 to October 2020**, covering **9,216 patient visits**. During this period, the ER maintained steady demand, with an average waiting time of approximately **35 minutes** and an average satisfaction score of **5.47 out of 10**.

Approximately **3,816 patients were referred to departments**, while the majority of cases were handled without escalation. Admissions are evenly distributed, with around half of patients admitted for further treatment.

---

## Data Model

The project uses a simplified modelling approach centred on a single fact table, `Hospital ER`, supported by `DimDate` and `DimTime`. Given the relatively small and flat structure of the dataset, demographic and categorical attributes were retained within the main table to reduce complexity while maintaining analytical flexibility.

This structure supports efficient calculation of operational metrics and enables analysis across time, patient groups, and referral categories.

---

## Key Insights

ER demand remains relatively consistent across the analysis period, indicating a stable flow of patient visits rather than highly seasonal or irregular patterns. Demand peaks on Mondays, followed by Tuesdays and Saturdays, with the busiest periods occurring during midday and evening hours. This suggests that operational pressure is predictable and can be planned for more effectively.

The average waiting time remains around **35 minutes**, while the average satisfaction score is **5.47 out of 10**, indicating a moderate patient experience. However, patient-level correlation analysis shows **almost no linear relationship (-0.002)** between waiting time and satisfaction. This suggests that delays alone do not explain patient experience, and that other factors such as communication, care quality, and treatment outcomes likely have a greater influence.

A large proportion of patients do not require referrals, indicating that many ER visits involve non-critical conditions. Among referred cases, General Practice and Orthopedics handle the highest volumes, highlighting their importance within the escalation pathway.

From a demographic perspective, the ER primarily serves the working-age population, with the highest concentration of patients between **20 and 39 years old**. Gender distribution is balanced, and the dataset reflects a diverse patient population, although some demographic information is not disclosed.

Admissions are split almost evenly between admitted and non-admitted patients, indicating a balanced triage system in which roughly half of cases require further medical attention.

---

## Dashboard Features

The dashboard is designed to provide both operational and patient experience perspectives. The main overview presents patient volume, waiting time, satisfaction, referral activity, and temporal demand patterns. Additional views highlight patient demographics, department performance, and the relationship between waiting time and satisfaction.

Interactive slicers support exploration by date, patient groups, and operational categories, allowing flexible analysis of ER performance.

---

## Techniques Used

This project applies time-based analysis, demographic segmentation, referral distribution analysis, and patient-level correlation analysis. DAX is used to calculate KPIs, operational measures, and satisfaction-related metrics.

The dashboard design emphasises clarity and interpretability, with visuals chosen to support both high-level performance monitoring and deeper analytical exploration.

---

## Recommendations

Operational resources should be better aligned with peak demand periods, particularly during midday and early weekdays, to reduce congestion and improve patient flow.

Given that many visits do not require specialist referrals, introducing fast-track pathways for non-critical cases could improve efficiency and reduce pressure on ER resources.

Since waiting time shows little correlation with satisfaction at the patient level, improvement efforts should extend beyond speed alone and focus more broadly on communication, care quality, and transparency in the patient experience.

Variations in referral activity and department performance also suggest opportunities to standardise practices and improve consistency across service pathways.

---

## Conclusion

This project demonstrates how patient-level operational data can be transformed into actionable healthcare insights. By combining data modelling, performance analysis, and effective visualisation, the dashboard provides a clear view of ER demand, service efficiency, and patient experience.

The findings highlight both the strengths of the current system and the areas where operational and experiential improvements can be made, supporting more informed healthcare decision making.

---

## Tools & Technologies

- Power BI
- DAX (Data Analysis Expressions)
- Data Modelling
- Data Visualisation