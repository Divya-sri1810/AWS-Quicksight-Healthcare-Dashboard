# 🏥 Healthcare Analytics Dashboard using Amazon QuickSight

This project is a comprehensive **Business Intelligence (BI) dashboard** built using **Amazon QuickSight** to visualize and analyze key metrics in the healthcare domain. It provides meaningful insights into patient demographics, hospital performance, billing trends, and medical conditions.

---

## 📌 Objective

To help healthcare professionals and administrators make data-driven decisions by analyzing patient records, billing details, and hospital-level metrics using interactive visualizations.

---

## 💡 Features & Visuals
- ✅ KPIs: Total Patients, Avg Billing, Most Common Condition, etc.
- 📊 Bar Charts: Top 5 Doctors, Avg Billing by Hospital
- 📈 Line Chart: Admission Trends Over Time
- 🗺️ Map: Condition Distribution by Hospital
- 📌 Filters: Admission Type, Month, Hospital

## 📊 Key Dashboards & Visuals

| Visualization                          | Type             | Insight Provided                              |
|----------------------------------------|------------------|-----------------------------------------------|
| Total Admissions                       | KPI              | Total number of patient admissions            |
| Average Billing Amount                 | KPI              | Mean billing per admission                    |
| Avg Length of Stay (Days)             | KPI              | Treatment duration trend                      |
| Gender Ratio                           | Donut Chart      | Gender distribution of patients               |
| Unique Doctors                         | KPI              | Total unique doctors involved                 |
| Age Distribution                       | Histogram        | Patient age spread                            |
| Blood Type Distribution                | Bar Chart        | Frequency of each blood group                 |
| Most Prescribed Medications            | Bar Chart        | Top medications across all patients           |
| Top 5 Doctors by Patient Count         | Bar Chart        | Most consulted doctors                        |
| Top Medical Conditions                 | Bar Chart        | Most common diagnoses                         |
| Admission Type Over Time              | Line Chart       | Emergency vs Elective admission trends        |
| Admissions per Hospital                | Horizontal Bar   | Hospital-level admission volume               |
| Hospitals Handling Most Urgent Cases   | Stacked Bar      | Urgent case load by hospital and gender       |
| Test Results Breakdown                 | Pie Chart        | Normal vs Abnormal test results               |
| Map of Medical Conditions (Optional)   | Points on Map    | Geographic clustering of diseases             |

---
## 🛠️ Tools & Technologies

- **Amazon QuickSight** – Data visualization and BI
- **Amazon Redshift** – Custom SQL-based dataset (optional)
- **CSV File** – Input dataset (healthcare records)
- **AWS Cloud** – Hosting and processing
- **GitHub** – Project documentation and source control

---

## 🔍 Insights Generated

- High admission rates during specific months
- Certain medications like **Lipitor** and **Paracetamol** are most prescribed
- Some hospitals handle more urgent cases than others
- Billing amounts vary widely across conditions
- Female patients form a slightly higher share of the dataset
- Medical conditions like **Diabetes**, **Asthma**, and **Arthritis** are more common

---
## 📊 Visual Decisions & Why

| Visual | Reason |
|--------|--------|
| **KPIs (cards)** | Provide quick-glance insights on total metrics |
| **Donut Chart** (Gender Ratio) | Effective for binary/categorical comparison |
| **Histogram** (Age) | Suitable for grouping continuous numerical values |
| **Bar Charts** (Medications, Conditions, Doctors) | Best for comparing discrete categories |
| **Stacked Bars** (Urgent Cases by Hospital & Gender) | Helps compare grouped segments |
| **Line Chart** (Admission Type Over Time) | Ideal for trend analysis |
| **Pie Chart** (Test Result Breakdown) | Good for categorical proportions |

---

## 🧠 Calculated Fields

| Name | Formula | Purpose |
|------|---------|---------|
| **Avg Length of Stay** | `dateDiff({discharge date}, {date of admission}, 'DD')` | To track hospital efficiency |
| **Top 5 Doctors** | Filtered by `Top N on count(doctor)` | Spotlight most visited doctors |
| **Total Unique Doctors** | `countDistinct(doctor)` | Measure resource diversity |
| **Gender Ratio** | Visual group by `gender` | Demographic analysis |

---

## 🧩 Filters Applied

- **Top N** filters for doctors, hospitals, medications
- **Date filters** to analyze time-based trends
- **Admission Type** for specific focus on Emergency, Urgent, Elective

---
## 🔐 Assumptions

- The dataset is anonymized and structured correctly
- Hospital names are unique identifiers
- All dates are in consistent format (`yyyy-mm-dd`)
- Location data (if used) is consistent with geospatial standards

---

## ✅ Learnings & Outcomes

- Designed a full BI solution from raw dataset to insight delivery
- Applied best practices in data visualization and dashboard storytelling
- Demonstrated strong grasp of Amazon QuickSight’s capabilities

---

## 📎 Use Cases
- Identifying top-performing doctors
- Monitoring average billing across hospitals
- Analyzing frequent medical conditions
- Understanding geographic spread of illnesses




