<div align="center">

# 🛒 Customer Shopping Behavior Analysis

### End-to-end retail analytics on 3,900 e-commerce transactions

*From raw CSV → Python cleaning → PostgreSQL analysis → Power BI dashboard*

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</div>

---

## 📋 Project Overview

A retail analytics project that answers a simple business question: **what kinds of customers drive the most revenue, and where should marketing spend go?**

The pipeline ingests a raw e-commerce dataset, cleans it in Python, loads it into PostgreSQL for analytical queries, and surfaces results in an interactive Power BI dashboard that a non-technical stakeholder can navigate.

<br>

<div align="center">

### 📊 Dashboard Preview

<!-- Replace this with: ![Dashboard](dashboard.png) once you add the screenshot to the repo -->
<img src="dashboard.png" alt="Power BI Dashboard" width="800"/>

*Interactive Power BI dashboard with slicers for Subscription Status, Gender, Category, and Shipping Type*

</div>

---

## 🗂️ Repository Contents

| File | Description |
|------|-------------|
| `customer_behavior_analysis.ipynb` | Python notebook — data cleaning, feature engineering, PostgreSQL load |
| `customer_behavior_analysis_queries.sql` | 10 analytical SQL queries on the cleaned dataset |
| `customer_behavior_dashboard.pbix` | Power BI dashboard file |
| `Customer Shopping Behavior Analysis.pdf` | Full report with findings and visualizations |

---

## 🛠️ Workflow

### 1️⃣ Data Preparation (Python · Pandas)

- Loaded 3,900 transactions across 18 customer attributes
- Identified **37 missing values** in `Review Rating` and imputed them using **category-median** (each product category's own median), preserving the rating distribution
- Engineered a clean **age-group** feature: *Young Adult, Adult, Middle-aged, Senior*
- Connected to PostgreSQL via Python and loaded the structured dataset for SQL analysis

### 2️⃣ Exploratory Analysis (PostgreSQL)

10 targeted SQL queries on business metrics. Key questions answered:

- Who spends more — male vs. female customers?
- How much revenue does the subscriber base actually drive?
- Which age cohort is the top financial contributor?
- Which product category has the strongest sales?

### 3️⃣ Visualization (Power BI)

Connected the PostgreSQL database to Power BI to build an interactive dashboard:

- **Core KPIs:** 3.9K customers · $59.76 average purchase · 3.75 average rating
- **Slicers** for Subscription Status, Gender, Product Category, Shipping Type
- **Side-by-side category comparison** showing Clothing leads on both volume and revenue

---

## 🔍 Key Findings

> 💰 **Male customers generate 2× the revenue of female customers** — $157,890 vs. $75,191

> 🔁 **Subscribers are a small but reliable base** — 1,053 subscribers (27% of customers) drive $62,645 in stable recurring revenue, while 2,847 non-subscribers (73%) make up the rest

> 👥 **Young Adults are the top contributors** with $62,143 in sales

> 👕 **Clothing dominates** sales volume *and* revenue versus Accessories, Footwear, and Outerwear

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/mohiuddinmdakram-alt/customer_behavior_analysis.git
cd customer_behavior_analysis

# 2. Open the notebook
jupyter notebook customer_behavior_analysis.ipynb

# 3. Run the SQL queries against your PostgreSQL instance
psql -d your_database -f customer_behavior_analysis_queries.sql

# 4. Open customer_behavior_dashboard.pbix in Power BI Desktop
```

---

<div align="center">

### 👤 Author

**Mohammed Akram Mohiuddin**
M.Sc. Data Science · Hochschule Fulda

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohammedakrammohiuddin/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mohiuddinmdakram-alt)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mohiuddinmdakram@gmail.com)

⭐ If you found this useful, consider starring the repo!

</div>
