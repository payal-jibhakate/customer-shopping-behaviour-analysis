# 🛍️ Customer Shopping Behaviour Analysis

> Analysing 3,900 retail transactions using Python, SQL & Power BI to uncover customer spending patterns, segment behaviour, and drive strategic business decisions.

---

## 📌 Business Problem

A leading retail company wanted to better understand its customers' shopping behaviour in order to improve sales, customer satisfaction, and long-term loyalty. The management team noticed changes in purchasing patterns across demographics, product categories, and sales channels.

**Central Business Question:**

> *"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"*

---

## 🎯 Project Objective

To perform an end-to-end data analysis of customer transaction data — cleaning and transforming it in Python, running structured business queries in SQL, and presenting actionable insights through an interactive Power BI dashboard.

---

## 📊 Dataset Overview

| Property | Details |
|---|---|
| **Total Records** | 3,900 rows |
| **Total Features** | 18 columns |
| **Missing Values** | 37 (Review Rating column) |
| **Source** | Retail customer transaction data |

**Feature Categories:**
- **Demographics** — Age, Gender, Location, Subscription Status
- **Purchase Details** — Item Purchased, Category, Purchase Amount (USD), Season, Size, Color
- **Behaviour** — Discount Applied, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type, Payment Method

---

## 🗂️ Repository Structure

    customer-shopping-behaviour-analysis/
    ├── dataset/
    │   └── customer_shopping_behaviour.csv
    ├── python_cleaning/
    │   └── customer_shopping_cleaning.ipynb
    ├── sql_queries/
    │   └── customer_shopping_queries.sql
    ├── powerbi_dashboard/
    │   └── customer_behaviour_dashboard.pbix
    ├── screenshots/
    │   └── SCREENSHOT.png
    └── README.md

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python (Pandas)** | Data Cleaning & Feature Engineering |
| **PostgreSQL** | Structured Business Analysis (10 SQL Queries) |
| **Power BI Desktop** | Interactive Dashboard & Visualization |
| **Jupyter Notebook** | Python Development Environment |
| **SQLAlchemy** | Python to PostgreSQL Connection |

---

## 🔄 Project Workflow

| Phase | Task | Status |
|---|---|---|
| Phase 1 | Data Preparation (Python) | ✅ Done |
| Phase 2 | Business Analysis (SQL) | ✅ Done |
| Phase 3 | Dashboard (Power BI) | ✅ Done |

---

## 🐍 Phase 1 — Data Preparation (Python)

Performed in Jupyter Notebook using Pandas:

- ✅ Loaded dataset and explored structure using df.info() and .describe()
- ✅ Detected and imputed 37 missing values in review_rating using category-wise median
- ✅ Standardised all column names to snake_case for consistency
- ✅ Engineered 2 new features:
  - age_group — binned customer ages into Young Adult / Adult / Middle-aged / Senior
  - purchase_frequency_days — derived from purchase frequency data
- ✅ Identified and dropped redundant column promo_code_used (correlated with discount_applied)
- ✅ Connected Python to PostgreSQL using SQLAlchemy and loaded clean data for SQL analysis

---

## 🗄️ Phase 2 — Business Analysis (SQL / PostgreSQL)

Executed 10 structured SQL queries to answer key business questions:

| # | Query | Key Finding |
|---|---|---|
| 1 | Revenue by Gender | Male: $157,890 vs Female: $75,191 |
| 2 | High-Spending Discount Users | 839 customers spent above average even with discounts |
| 3 | Top 5 Products by Rating | Gloves (3.86), Sandals (3.84), Boots (3.82) |
| 4 | Shipping Type Comparison | Express ($60.48) vs Standard ($58.46) |
| 5 | Subscribers vs Non-Subscribers | 1,053 subscribers vs 2,847 non-subscribers |
| 6 | Discount-Dependent Products | Hat (50%), Sneakers (49.7%), Coat (49.1%) |
| 7 | Customer Segmentation | Loyal: 3,116 · Returning: 701 · New: 83 |
| 8 | Top 3 Products per Category | Used RANK() window function per category |
| 9 | Repeat Buyers & Subscriptions | 2,518 repeat buyers are non-subscribers |
| 10 | Revenue by Age Group | Young Adult: $62,143 (highest contributor) |

---

## 📈 Phase 3 — Dashboard (Power BI)

Built a single-page interactive dashboard with:

**KPI Cards:**
- 👥 3.9K Total Customers
- 💰 $59.76 Average Purchase Amount
- ⭐ 3.75 Average Review Rating

**Visuals:**
- 🍩 Donut Chart — Subscription Status (73% No, 27% Yes)
- 📊 Bar Charts — Revenue and Sales by Category
- 📊 Bar Charts — Revenue and Sales by Age Group

**Slicers (Interactive Filters):**
- Subscription Status · Gender · Category · Shipping Type

---

## 📷 Dashboard Preview

![Dashboard Preview](screenshots/SCREENSHOT.png)

---

## 💡 Key Insights & Findings

| # | Insight | Finding |
|---|---|---|
| 1 | **Gender Revenue Gap** | Male customers generate 2x more revenue ($157,890 vs $75,191) |
| 2 | **Subscription Rate** | 73% of customers are non-subscribers — large untapped base |
| 3 | **Top Age Group** | Young Adults are highest revenue group at $62,143 |
| 4 | **Loyalty vs Subscription** | 80% customers are Loyal but most are NOT subscribed |
| 5 | **Discount Risk** | Hat, Sneakers and Coat over-discounted (~50%) — margin risk |

---

## 📋 Business Recommendations

| Recommendation | Rationale |
|---|---|
| 🔔 **Boost Subscriptions** | 73% non-subscription rate is an untapped retention opportunity |
| 🏆 **Loyalty Programs** | Reward the 3,116 Loyal customers with exclusive perks |
| 📉 **Review Discount Policy** | Limit discounts on Hat/Sneakers/Coat to protect margins |
| 🌟 **Product Positioning** | Feature top-rated products (Gloves, Sandals) in campaigns |
| 🎯 **Targeted Marketing** | Focus on Young Adults and Express shipping users |

---

## 📁 Skills Demonstrated

Data Cleaning · Exploratory Data Analysis · Feature Engineering · Missing Value Imputation · SQL Window Functions · Customer Segmentation · KPI Analysis · Business Intelligence · Dashboard Design · Data Storytelling

---

## 👩‍💻 Author

**Payal Jibhakate**
Aspiring Data Analyst | Python | SQL | Power BI

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/payal-jibhakate-900694378)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/payal-jibhakate)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:payaljibhakate2004@gmail.com)

---

*This project was completed as part of a Data Science portfolio to demonstrate end-to-end data analysis skills for business decision-making.*

---

⭐ *If you found this project helpful, please give it a star!* ⭐
