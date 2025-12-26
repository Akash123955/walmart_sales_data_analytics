# 🛒 Walmart Data Analysis: End-to-End SQL + Python Project + Tableau

## 📌 Project Overview

![Project Pipeline](https://github.com/Akash123955/walmart_sales_data_analytics/blob/main/project_pipeline.png)

This project is an **end-to-end data analytics solution** built on Walmart sales data to extract meaningful business insights and present them through an interactive Tableau dashboard.

The project simulates a **real-world retail analytics workflow**, where raw transactional data is cleaned, stored in a relational database, analyzed using SQL, and finally visualized for business stakeholders.

Unlike simple visualization projects, this solution emphasizes:
- Strong **SQL-based business analysis**
- Clean separation between **data processing, analysis, and visualization**
- Business-oriented insights aligned with retail decision-making

## 🎯 Business Objectives
Retail businesses like Walmart rely heavily on data to understand customer behavior, optimize operations, and improve profitability.

The goal of this project is to answer **business-critical questions**, such as:
- How do customers prefer to pay?
- Which product categories drive the most sales and profit?
- How do customer ratings vary across branches and cities?
- When do most transactions occur (day and shift)?
- Which branches are experiencing revenue decline?
---

## 🧰 Tech Stack
- **Python** – Data cleaning and preprocessing  
- **Pandas** – Data manipulation  
- **MySQL** – Relational data storage and querying  
- **SQL** – Business analysis and insight generation  
- **Tableau Public** – Interactive data visualization  

---

## 📂 Dataset
- Dataset was **downloaded directly from the Kaggle website**
- No Kaggle API was used
- Data processed entirely in a local environment
- Dataset contains transactional sales data including:
  - Branch
  - Product category
  - Payment method
  - Quantity sold
  - Profit
  - Customer ratings
  - Transaction date and time
---

## 🔄 Project Workflow

### 1️⃣ Data Cleaning & Preparation (Python)
Raw Walmart data was first explored and cleaned using **Pandas**.

Key steps included:
- Handling missing and inconsistent values
- Correcting data types (dates, numeric fields)
- Creating derived columns (day name, shift, etc.)
- Preparing the dataset for relational storage

The cleaned dataset was saved as:
`walmart_cleaned_data.csv`
This step ensures the data is reliable before loading it into a database.

---

### 2️⃣ Database Setup & Data Loading (MySQL)
- Created a MySQL database and tables
- Loaded cleaned data into MySQL using **SQLAlchemy** and **PyMySQL**
- Designed schema optimized for analytical queries

---

### 3️⃣ Business Analysis Using SQL
- Solved all business questions using **SQL**
- Techniques used:
- `GROUP BY`
- Aggregate functions
- Conditional logic
- Date-based analysis
- All queries stored in:
`walmart_insights_mysql`
This ensures transparency and reproducibility of analysis.

---

### 4️⃣ Exporting SQL Results (JSON per Question)
- Each business question’s SQL output was **exported as a separate JSON file**
- These JSON files were used directly as data sources in Tableau

```
result insights/
├── q1.json
├── q2.json
├── q3.json
├── ... 
```


This approach ensures a clean separation between **data processing, analysis, and visualization**.

---

### 5️⃣ Data Visualization (Tableau)
- Imported JSON outputs into **Tableau**
- Built:
  - KPI cards
  - Bar charts
  - Heatmaps
  - Stacked charts
- Designed a **professional, interactive dashboard** aligned with business requirements

---

## 📊 Tableau Dashboard
🔗 **Live Dashboard:**  
https://public.tableau.com/app/profile/satish.varma.vejarla8567/viz/walmartsalesinsights_17667039196760/Dashboard1

---

## 📁 Repository Structure
```
├── my_env1/ # Python virtual environment
├── project.ipynb # Data cleaning & transformation
├── Walmart.csv # Raw dataset
├── walmart_cleaned_data.csv # Cleaned dataset
├── walmart_insights_mysql.sql # SQL queries for all business questions
├── result insights/ # JSON outputs (per question)
│ ├── q1.json
│ ├── q2.json
│ ├── q3.json
│ └── ...
├── project_pipeline.png # Project architecture diagram
├── Walmart_Business_Problems.pdf
├── requirements.txt
├── README.md
```
---

## 📈 Key Insights Visualized
- Payment Method Usage and Preferences
- Quantity Sold and Profit by Category
- Average Customer Ratings by Branch and City
- Transaction Trends by Day and Shift
- Branches with Year-over-Year Revenue Decline

---

## 🧠 Key Learnings
- Built an end-to-end analytics workflow similar to real industry projects
- Strengthened SQL skills for business-driven problem solving
- Learned how to integrate SQL outputs with Tableau using JSON
- Designed executive-level dashboards for decision-making

---

## 🚀 How to Run the Project

### Install Dependencies
```bash
pip install pandas pymysql sqlalchemy psycopg2-binary

