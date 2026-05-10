# Telecom Customer Churn Analysis

## Project Overview
This project focuses on analyzing customer churn behavior for a telecom company using Python, SQL, and Power BI. The objective was to identify the key factors contributing to customer attrition and provide data-driven business recommendations to improve customer retention.

The analysis was performed on 7,043 customer records containing demographic information, service usage patterns, contract details, payment methods, and churn status.

## Business Problem
The telecom company was experiencing a high customer churn rate of 26.54%, leading to revenue loss of $139K at risk.

This project aims to answer:
- Why are customers leaving?
- Which customer segments are at highest risk?
- What business actions can reduce churn?

## Tools & Technologies Used
- **Python** — Pandas, NumPy, Matplotlib, Seaborn
- **SQL** — CTEs, Window Functions, Cohort Analysis (SQLite)
- **Power BI** — KPIs, Dynamic Filters, DAX
- **Jupyter Notebook**

## Key Insights
- Month-to-month contracts: **43% churn rate** vs 3% for two-year contracts
- New customers (tenure <12 months): **47% churn rate**
- Electronic check users: **45% churn rate**
- Fiber Optic internet users showed **elevated churn behavior**
- High-risk segment (month-to-month + tenure ≤12 months + charges >$65): **~65% churn probability**
- Revenue at risk: **$139K**

## Dashboard Preview
![Customer Churn Dashboard](images/dashboard_screenshot.png)

## Key Analysis Performed

### Exploratory Data Analysis (EDA)
- Customer churn distribution analysis
- Contract type churn analysis
- Monthly charges vs churn analysis
- Tenure-based churn trend analysis
- Internet service churn analysis
- Payment method analysis
- Senior citizen churn analysis

### SQL Analysis
- Overall churn rate calculation
- Tenure cohort segmentation
- Window functions for risk ranking
- CTEs for high-churn segment identification
- Business KPI analysis

### Dashboard Development
An interactive Power BI dashboard developed to visualize:
- Overall churn metrics and revenue at risk
- Contract-wise and internet service churn trends
- Payment method analysis
- Dynamic filtering using slicers

## Business Recommendations
- Offer incentives for long-term contracts to reduce month-to-month churn
- Improve onboarding experience for new customers (first 12 months critical)
- Investigate Fiber Optic service quality issues
- Encourage automatic payment methods through discounts
- Develop targeted retention strategies for high-risk segments

## Project Structure

telecom-churn-analysis/
├── data/
│   └── raw/
│       └── CustomerChurn.csv
├── notebooks/
│   └── Customer_Churn_Analysis.ipynb
├── sql/
│   └── churn_queries.sql
├── dashboard/
│   └── churn_dashboard.pbix
├── images/
│   └── dashboard_screenshot.png
├── requirements.txt
└── README.md

## How to Run
1. Clone the repo
git clone https://github.com/AnanyaRaj-agr/telecom-churn-analysis.git
2. Install dependencies
pip install -r requirements.txt
3. Open `notebooks/Customer_Churn_Analysis.ipynb` in Jupyter
4. For Power BI dashboard, open `dashboard/churn_dashboard.pbix`

## Outcome
This project demonstrates practical skills in data cleaning, exploratory data analysis, SQL-based business analysis, data visualization, dashboard development, and business problem solving.
