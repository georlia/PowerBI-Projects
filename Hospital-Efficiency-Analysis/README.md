# 🏥Case Study: Analyzing Healthcare Data 

> **Stakeholder:**  Datacamp.   
> **Objective:**  Identify hospital efficiency opportunities by analyzing Length of Stay (LOS) and Cost.

## Project Overview
In this case study, I acted as a consultant for **HealthStat** to uncover insights into hospital operational efficiency. The analysis focuses on New York State-wide hospital discharge data, specifically targeting patients who underwent **elective hip replacement surgery**.

## Dashboard Walkthrough
![Media/walkthrough_hosp.gif]([Media/walkthrough_hosp.gif)

## Motivation & Problem Statement
Efficiency in healthcare is defined by avoiding waste—minimizing the misuse of equipment, energy, and ideas. 
* **The Challenge:** High **Length of Stay (LOS)** increases operational costs and reduces a hospital's capacity to serve more patients.
* **The Goal:** To create an engaging dashboard that allows stakeholders to:
    * Identify outlier hospitals with high costs and LOS relative to the state average.
    * Understand the impact of surgical program size on efficiency.
    * Perform **Root Cause Analysis** to find factors influencing LOS.

## Technology & Process
* **Tool:** Power BI
* **Dataset:** 1 year of New York State-wide discharge data.
* **The Process:**
    1. **Data Cleaning:** Filtered for elective hip replacements and handled outliers in LOS and cost.
    2. **Metric Creation:** Developed DAX measures for Average LOS, State Averages, and Cost-to-LOS ratios.
    3. **Data Modeling:** Optimized a flat-file dataset for performance and logical flow.

## Key Insights (Business Questions Answered)
* **Outlier Identification:** Spotted specific facilities where costs exceed the state average by more than 20% without a proportional increase in illness severity.
* **Program Size:** Evaluated whether larger surgical programs achieve better "throughput" (lower LOS) due to specialization.
* **Root Cause:** Determined that **Severity of Illness** and **Patient Disposition** (destination after discharge) are the strongest predictors of prolonged hospital stays.

## Challenges & Limitations
* **Scope:** The analysis is limited to a specific procedure (Hip Replacement) and may not represent overall hospital efficiency.
* **Data Privacy:** The dataset is de-identified; therefore, patient-level longitudinal tracking (readmissions) was not possible.

## Repository Contents
* `/Backgrounds`: The backgrounds of every dashboard page.
* `/Dataset`: The dataset.
* `/Media`: A video walthrough of the dashboard.
* `/Template`: The template of the dashboard.
* `Hospital-Efficiency-Analysis.pbix`: The final Power BI interactive dashboard.

