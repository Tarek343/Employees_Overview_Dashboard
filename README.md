# Employees_Overview_Dashboard
# 👥 HR Workforce Analysis & Headcount Dashboard

## 🌟 Project Overview and Goal

This Power BI solution was developed to deliver an *interactive and executive-level overview* of the organization’s Human Resources data. The analysis focuses on workforce composition, key cost drivers, and talent retention metrics across *689 employees*.

* *Objective:* To empower HR leadership with data-driven insights for strategic headcount planning, budget allocation, and proactive identification of high-risk turnover areas.
* *Time Frame:* Analysis covers the period from 2018 to the present day.
* *Key Finding Summary:* The dashboard successfully identified that the highest turnover (25%) is concentrated in the Sales department among employees with less than 2 years of service.

---

## 🛠 Tools and Technologies Used

| Tool/Technology | Purpose and Application |
| :--- | :--- |
| *Power BI Desktop* | Visualization, Data Modeling, and design of an intuitive user interface. |
| *Power Query (M Language)* | Advanced ETL (Extract, Transform, Load) processes, including data standardization, merging employee master files with salary tables. |
| *DAX* | Creation of crucial HR metrics: *Headcount, **Turnover Rate (%), **Average Salary by Band, and **FTE (Full-Time Equivalent)*. |
| *Data Source* | Raw HR Records (covering 689 employees and a total annual salary spend of $1.4 Million). |

---

## ⚙ Analysis Methodology

### 1. Data Preparation and Cleaning
* *Source Data:* The project started with two disparate files: an Employee Master List and a Salary Ledger.
* *Key Transformations:* Used Power Query to merge these two files using the Employee ID as the unique key. Null values in the 'Salary' field were identified and imputed using a median calculation specific to the employee’s job band to avoid bias. *Departmental naming inconsistencies were standardized.*

### 2. Data Modeling and Key Calculations
* *Model Structure:* A single table model was utilized for simplicity and speed, with crucial calculated columns added for analysis.
* *Calculations:* Custom DAX measures were built to calculate:
    * *Turnover Rate:* Calculated as (Total Leavers / Avg. Headcount) = *18% overall*.
    * *Average Service Length:* Calculated at *4.5 years*.
    * *Age and Tenure:* Calculated based on raw dates to create meaningful demographic segments.

---

## 💡 Key Insights and Business Findings

The HR analysis delivered the following actionable insights:

* *Headcount Distribution:* The *Manufacturing department* holds the largest portion of the workforce, accounting for *38%* of the total headcount (262 employees).
* *Turnover Risk:* The *Sales department* has the highest recorded turnover rate at *25%*, which is 7 percentage points higher than the company average. This risk is concentrated among junior-level employees.
* *Compensation:* The average salary across the organization is *$61,000 USD*. Analysis showed a high correlation between employees earning below $50k and the overall turnover rate.
* *Demographics:* The workforce is predominantly male (*62%*) with a median age of 32 years.
