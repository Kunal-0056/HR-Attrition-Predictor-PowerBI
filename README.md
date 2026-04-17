# HR Workforce Insights & Employee Attrition Predictor

![Dashboard Preview](Dashboard_Preview.png)

## 📌 Project Overview
Employee attrition is a significant cost multiplier for modern organizations. This project serves as an end-to-end Business Intelligence solution that not only visualizes historical HR metrics but also integrates a **Machine Learning predictive model** to proactively identify flight-risk employees before they leave.

## 🛠️ Tech Stack & Tools
* **Data Visualization & Modeling:** Power BI, Power Query, DAX
* **Machine Learning & Scripting:** Python (Pandas, Scikit-Learn)
* **Algorithms Used:** Logistic Regression

## 🚀 Key Features & Methodologies

### 1. Python-Powered Predictive Analytics
Instead of relying purely on historical trends, this dashboard features an embedded Python script running a Logistic Regression model.
* **The Process:** The model ingests live Power BI data, splits it into training and testing sets, and evaluates features such as `MonthlyIncome`, `PerformanceScore`, `Age`, and `TrainingHours`.
* **The Output:** It generates a binary `Attrition_Prediction` flag (1 = High Risk, 0 = Low Risk) for every active employee, automatically feeding back into the Power BI data model.

### 2. Advanced Data Transformation
* Executed complex data merging and cleaning via Power Query (handling null values, standardizing datatypes, and bypassing firewall privacy limits for Python integration).
* Engineered a custom `DateTable` hierarchy to ensure accurate time-series analysis without breaking Python type constraints.

### 3. Executive Dashboard Design
Designed utilizing standard BI UX principles (Z-Pattern layout, dedicated left-hand filter pane, and high-contrast visuals):
* **Risk Scatter Plot:** Visually highlights the exact correlation between low income, low performance, and predicted flight risk.
* **Intervention Table:** A dynamic, sorted action list allowing HR managers to immediately identify and contact at-risk employees.
* **Trend & Demographics:** Breakdown of attrition by Department, Gender, and Hiring Cohort.

## 💡 How to Use This Dashboard
1. Download the `HR_Attrition_Predictor.pbix` file from this repository.
2. Open the file in **Power BI Desktop**.
3. Note: To run the Python script locally, ensure you have Python installed along with the `pandas` and `scikit-learn` libraries.
