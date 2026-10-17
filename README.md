# Telecom-Customer-Churn-Analysis

An end-to-end data analytics project that turns a messy raw telecom customer dataset into a clean, interactive Power BI dashboard for tracking churn, revenue and customer retention.

![Dasboard Preview](https://github.com/samridhdeshwar01-hue/Telecom-Customer-Churn-Analysis/blob/main/Dashboard%20Screenshot.png). 

---

## 🎯 Business Problem

Telecom companies lose revenue every time a customer leaves. This project answers questions such as:

- What is the overall churn rate, and how much revenue is at stake?
- Which contract types and subscription plans see the most churn?
- Which states and customer groups bring in the most revenue?
- How do payment methods relate to churn and retention?

---

## 📝 Description

This project takes a raw telecom customer dataset of 540+ records and 18 columns and turns it into clear business insights. I cleaned the data with Python (pandas and numpy) by removing duplicates, standardizing text values, filtering invalid ages and negative charges, handling missing values and fixing date formats. I then created new metrics such as customer value, monthly revenue, tenure groups, senior flag and churn flag. The cleaned data was loaded into MySQL and then into Power BI through Power Query. Finally, I built an interactive dashboard to track total customers, churn rate, retained customers, revenue, average tenure and monthly charges by contract type, subscription type, state, gender and payment method.

---

## 🔄 Project Workflow

```
Excel (raw data) → Python / Jupyter (cleaning) → MySQL (storage) → Power Query → Power BI (dashboard)
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 📗 **Excel** | Source of the raw, unclean churn dataset |
| 🐍 **Python (pandas, numpy)** | Data cleaning and feature engineering |
| 📓 **Jupyter Notebook** | Documented the cleaning workflow step by step |
| 🔌 **SQLAlchemy and PyMySQL** | Connected Python to MySQL and loaded the cleaned data |
| 🗄️ **MySQL** | Stored the cleaned customer data |
| 📂 **Power Query** | Loaded the MySQL data into Power BI |
| 📊 **Power BI Desktop** | Built the interactive dashboard |
| 🧠 **DAX** | Calculated measures such as Churn Rate, Retained Customers and Total Revenue |

---

## 📊 Dashboard Highlights

**KPIs:** 445 Total Customers | 105 Churned | 340 Retained | 23.60% Churn Rate | 22.16M Total Revenue | 35.95 Months Average Tenure | 1.36K Average Monthly Charges

**Visuals:** churn by contract type, churn by subscription type, revenue by state, revenue by gender, and retained customers by state and contract type, with a payment method slicer for filtering.

---

## 🔍 Key Insights

- **Roughly 1 in 4 customers churned**, with a churn rate of 23.60% (105 of 445 customers).
- **Standard and Premium plans account for most churn**, with Basic showing the least.
- **Churn is spread across all contract types.** Two-Year contracts show slightly higher churn than Month-to-Month, which is worth investigating further.
- **Delhi, Gujarat and UP lead in revenue**, while Maharashtra generates the least among the five states.
- **Female customers contribute 56.18% of revenue** (12.45M) compared to 43.82% for male customers (9.71M).

---

## 💡 Recommendations

1. Review pricing and service quality on Standard and Premium plans, since they lose the most customers.
2. Investigate why long-term contract customers are churning, for example through renewal offers or loyalty benefits.
3. Focus retention campaigns on high-revenue states such as Delhi, Gujarat and UP.
4. Track churn by payment method to spot billing-related friction.

---

## 📁 Repository Structure

```
├── Churn_Unclean_Project.xlsx      # Raw dataset
├── Churn_Dataset_Cleaning.ipynb    # Python cleaning notebook
├── Clean_Churn_Data.csv            # Cleaned dataset
├── Telecom_Churn_Dashboard.pbix    # Power BI dashboard
├── Dashboard_Screenshot.png        # Dashboard preview
└── README.md
```







