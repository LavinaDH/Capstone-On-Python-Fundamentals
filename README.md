# 📊 Python Capstone Project: Employee & Project Data Analysis

## 📌 Project Overview
This project demonstrates an end-to-end data analysis workflow designed to simulate real-world corporate data management. Using **Python** and **Pandas**, I developed a system to manage, clean, and transform employee and project datasets based on complex business rules such as performance-based promotions, financial bonuses, and cost aggregations.

The simulation tracks how an organization’s workforce evolves based on project outcomes, age demographics, and budgetary constraints.

## 🎯 Key Objectives
* **Data Architecture:** Creating structured relational datasets using Pandas.
* **Data Integrity:** Handling missing values and data cleaning (e.g., string splitting and mapping).
* **Business Logic:** Implementing conditional rules (Bonuses, Promotions, Demotions).
* **Relational Operations:** Merging disparate datasets into a single source of truth.
* **Statistical Insights:** Performing group-level aggregations and filtering.

## 🛠 Tools & Technologies
* **Language:** Python 3.x
* **Library:** Pandas (Data Manipulation & Analysis)
* **Environment:** Jupyter Notebook / Anaconda
* **Output:** CSV (Data Persistence)

## 🧩 Technical Workflow
The project was executed in a modular 10-task approach:

### 1. Data Wrangling & Cleaning
* **Missing Value Imputation:** Replaced null project costs using a running average logic.
* **Feature Engineering:** Split full names into First/Last names and applied gender-based prefixes ("Mr./Mrs.") using `lambda` functions.
* **Relational Joins:** Executed a 3-way merge between Employee, Seniority, and Project tables.

### 2. Business Logic Implementation
* **Bonus Allocation:** Applied a 5% bonus calculation for all "Finished" projects.
* **Performance-Based Demotions:** Automated designation changes for failed projects, including logic to remove records exceeding Level 4 seniority.
* **Promotion Cycles:** Implemented age-based promotion logic for employees over 29.

### 3. Aggregation & Analytics
* **Cost Analysis:** Utilized `groupby()` and `sum()` to calculate the total financial weight handled by individual employees.
* **Geospatial Filtering:** Used `str.contains()` to filter records based on specific city naming conventions.

## 🔍 Key Insights
* **Workforce Efficiency:** 5 core employees remained active after all business-rule filters were applied.
* **Financial Impact:** Managed a total project portfolio of approximately **₹26 Million**.
* **Top Performer:** Mrs. Nina was identified as the lead contributor, managing **~₹9.5 Million** in project costs.
* **Incentive Alignment:** The bonus distribution successfully rewarded completed projects, reinforcing performance-driven data modeling.

## 📈 Final Outputs
The analysis produced three primary reporting files:
1. `Final_after_task8.csv` – The consolidated, "cleaned" master dataset.
2. `TotalProjCost.csv` – A summary of financial responsibility per employee.
3. `Employees_City_with_O.csv` – A targeted geographical subset of the workforce.

---
### 🎓 Key Learnings
This capstone project solidified my ability to apply **modular Python code** to solve non-linear business problems. It demonstrates proficiency in data transformation, handling relational data structures, and generating actionable insights from raw CSV files.
