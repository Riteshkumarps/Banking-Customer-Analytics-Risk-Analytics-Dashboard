# 🏦 Banking Customer Analytics & Risk Analytics Dashboard

## 📌 Project Overview

**Banking Customer Analytics & Risk Analytics Dashboard** is an end-to-end banking analytics project focused on understanding **risk analytics in banking and financial services**.

The project analyzes customer financial and banking data to understand lending exposure, customer segments, deposits, loans, business lending, income, risk weighting, banking relationships, and customer characteristics.

The analysis combines **Python, SQL, and Power BI** to transform raw banking data into business insights and risk-aware recommendations.

---

## 🎯 Problem Statement

> **Develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.**

The project analyzes customer-level banking information to understand lending exposure and identify patterns across different customer and risk segments.

The objective is to understand how data can support:

- Lending-risk analysis
- Customer segmentation
- Financial exposure analysis
- Portfolio monitoring
- Customer relationship management
- Data-driven lending decisions

> **Note:** This project focuses on risk and lending-exposure analysis. It does not claim to predict loan defaults because the current dataset does not contain a validated loan-default target variable.

---

# 📁 Project Structure

```text
Banking Customer Analytics/
│
├── datasets/
│   ├── banking-clients.csv
│   ├── banking-relationships.csv
│   ├── Banking.csv
│   ├── gender.csv
│   └── investment-advisors.csv
│
├── .env
│
├── Banking_Customer_Analytics_Insights_Recommendations_V2.html
│
├── Banking_dashboard.pbix
│
├── BankingEDA.ipynb
│
└── README.md
```

---

# 📂 Dataset Files

The `datasets/` folder contains the source CSV files used for the project.

| File | Purpose |
|---|---|
| `Banking.csv` | Main banking/customer financial dataset |
| `banking-clients.csv` | Client/customer information |
| `banking-relationships.csv` | Banking relationship information |
| `gender.csv` | Gender lookup information |
| `investment-advisors.csv` | Investment advisor information |

---

# 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Database | MySQL |
| Query Language | SQL |
| Business Intelligence | Power BI |
| Dashboard | Power BI |
| Analysis Environment | Jupyter Notebook |
| Documentation | Markdown / HTML |

---

# 🔄 Project Workflow

```text
Raw Banking Data
       ↓
Data Understanding
       ↓
Data Validation
       ↓
Data Cleaning
       ↓
Exploratory Data Analysis
       ↓
Customer Segmentation
       ↓
Risk & Lending Exposure Analysis
       ↓
Correlation Analysis
       ↓
SQL Business Analysis
       ↓
Power BI Dashboard
       ↓
Business Insights
       ↓
Recommendations
```

---

# 📊 Dataset Overview

The main `Banking.csv` dataset contains:

- **3,000 customer records**
- **25 columns**
- **0 missing cells detected**

Important analytical variables include:

- Estimated Income
- Bank Deposits
- Bank Loans
- Business Lending
- Checking Accounts
- Saving Accounts
- Risk Weighting
- Fee Structure
- Loyalty Classification
- GenderId

---

# 🎯 Business Objectives

The project aims to:

1. Understand customer financial behavior.
2. Analyze lending exposure.
3. Compare lending exposure across risk-weighting groups.
4. Understand the relationship between income and loans.
5. Analyze deposits, checking accounts, and savings accounts.
6. Analyze business-lending exposure.
7. Segment customers based on financial characteristics.
8. Identify patterns that can support risk-aware decisions.
9. Build an interactive Power BI dashboard.
10. Generate actionable business recommendations.

---

# ❓ Business Questions

The project investigates questions such as:

1. How does lending exposure vary across risk-weighting groups?
2. Which customer segments have higher loan exposure?
3. How does estimated income relate to bank loans?
4. What is the relationship between Bank Deposits and Checking Accounts?
5. What is the relationship between Bank Deposits and Saving Accounts?
6. How does Business Lending relate to Bank Loans?
7. How does Business Lending relate to Bank Deposits?
8. Which customer segments may require closer monitoring?
9. How can customer financial behavior support risk-aware lending decisions?

---

# 📈 Key KPIs

| KPI | Value |
|---|---:|
| Total Customers | **3,000** |
| Total Bank Deposits | **$2.015B** |
| Total Bank Loans | **$1.774B** |
| Total Business Lending | **$2.600B** |
| Missing Cells | **0** |

---

# 🔍 Key Insights

## 1. Bank Deposits & Checking Accounts

The correlation between:

**Bank Deposits ↔ Checking Accounts = 0.844**

This is the strongest relationship identified in the analysis.

### Business interpretation

Customers with larger Bank Deposits tend to have larger Checking Account balances.

This relationship can be considered when analyzing:

- Customer relationships
- Deposit behavior
- Product opportunities
- Banking-product combinations

---

## 2. Bank Deposits & Saving Accounts

The correlation between:

**Bank Deposits ↔ Saving Accounts = 0.755**

This indicates a strong positive association in the dataset.

Customers with larger deposit balances tend to have larger savings balances.

---

## 3. Income & Bank Loans

The correlation between:

**Estimated Income ↔ Bank Loans = 0.330**

This indicates a positive association between income and loan exposure.

Higher-income customer segments show higher average loan balances in the dataset.

---

## 4. Business Lending & Bank Loans

The correlation between:

**Business Lending ↔ Bank Loans = 0.417**

This indicates a moderate positive association between business lending and bank loans.

---

## 5. Business Lending & Bank Deposits

The correlation between:

**Business Lending ↔ Bank Deposits = 0.441**

This indicates a positive association between business lending and bank deposits.

---

# 👥 Income Segmentation

Customers are divided into three income bands:

| Income Band | Definition |
|---|---|
| Low | ≤ $100K |
| Mid | $100K–$300K |
| High | > $300K |

### Segment Analysis

| Income Band | Customers | Avg Deposits | Avg Loans | Avg Business Lending |
|---|---:|---:|---:|---:|
| Low | 562 | $486,223 | $436,410 | $636,062 |
| Mid | 962 | $719,400 | $621,286 | $913,226 |
| High | 1,476 | $929,822 | $840,951 | $1,231,755 |

The High-income segment contains the largest number of customers and has the highest average deposits, loans, and business lending.

---

# ⚠️ Risk Analysis

The dataset contains five Risk Weighting levels.

| Risk Weighting | Customers |
|---:|---:|
| 1 | 836 |
| 2 | 1,222 |
| 3 | 460 |
| 4 | 322 |
| 5 | 160 |

Risk Weighting can be analyzed together with:

```text
Risk Weighting
       +
Bank Loans
       +
Business Lending
       +
Estimated Income
       +
Bank Deposits
```

This provides a more complete view of customer financial exposure.

---

# 💡 Business Recommendations

## 1. Risk-Aware Customer Segmentation

Combine customer financial characteristics with Risk Weighting to create meaningful segments.

Potential segmentation variables:

- Income
- Bank Deposits
- Bank Loans
- Business Lending
- Risk Weighting

---

## 2. Monitor High Lending Exposure

Customers with higher loan or business-lending exposure can be analyzed alongside their risk group.

This can support:

- Portfolio monitoring
- Credit review
- Relationship management
- Risk analysis

---

## 3. Deposit & Savings Cross-Sell Analysis

Because Bank Deposits and Checking Accounts have a strong relationship, customers with high deposit balances can be investigated for additional banking-product opportunities.

Potential areas:

- Savings products
- Cash-management services
- Banking bundles
- Relationship products

---

## 4. Income-Based Lending Analysis

Income segments can be compared with loan exposure to understand how lending differs across customer financial profiles.

This can support customer segmentation and portfolio analysis.

---

## 5. Business Banking Opportunities

Customers with Business Lending exposure and significant Bank Deposits or Bank Loans can be investigated for deeper business-banking relationships.

Potential areas:

- Working-capital products
- Cash-management services
- Business banking
- Relationship-based services

---

# 🐍 Python EDA

The `BankingEDA.ipynb` notebook is used for exploratory data analysis.

Typical analysis includes:

### Load the dataset

```python
import pandas as pd
import numpy as np

df = pd.read_csv("datasets/Banking.csv")
```

### Dataset shape

```python
df.shape
```

### Dataset information

```python
df.info()
```

### Statistical summary

```python
df.describe()
```

### Missing-value analysis

```python
df.isnull().sum()
```

### Correlation analysis

```python
df["Bank Deposits"].corr(df["Checking Accounts"])
```

### Income segmentation

```python
df["Income Band"] = pd.cut(
    df["Estimated Income"],
    bins=[0, 100000, 300000, float("inf")],
    labels=["Low", "Mid", "High"],
    include_lowest=True
)
```

---

# 🗄️ SQL Analysis

SQL can be used to perform business-oriented analysis on the banking data.

### Average loan by risk weighting

```sql
SELECT
    RiskWeighting,
    AVG(BankLoans) AS AverageLoans
FROM banking_customer
GROUP BY RiskWeighting
ORDER BY RiskWeighting;
```

### Total lending exposure

```sql
SELECT
    SUM(BankLoans) AS TotalBankLoans,
    SUM(BusinessLending) AS TotalBusinessLending
FROM banking_customer;
```

### Customer lending exposure

```sql
SELECT
    ClientID,
    EstimatedIncome,
    BankDeposits,
    BankLoans,
    BusinessLending,
    RiskWeighting
FROM banking_customer
ORDER BY BankLoans DESC;
```

---

# 📊 Power BI Dashboard

The `Banking_dashboard.pbix` file contains the Power BI dashboard.

The dashboard is designed to provide an interactive view of:

- Customer overview
- Bank deposits
- Bank loans
- Business lending
- Risk weighting
- Income segmentation
- Customer classification
- Financial exposure
- Banking relationships

### Suggested Dashboard Pages

#### Page 1 — Executive Overview

KPIs:

- Total Customers
- Total Deposits
- Total Loans
- Total Business Lending

#### Page 2 — Risk Analytics

Visuals:

- Customer count by Risk Weighting
- Average Loan by Risk Weighting
- Business Lending by Risk Weighting
- Lending Exposure by Segment

#### Page 3 — Customer Segmentation

Visuals:

- Customers by Income Band
- Deposits by Income Band
- Loans by Income Band
- Loyalty Classification
- Fee Structure

#### Page 4 — Product & Relationship Analysis

Visuals:

- Checking Accounts
- Saving Accounts
- Bank Deposits
- Bank Loans
- Business Lending
- Product relationships

---

# 📄 Insights & Recommendations

The file:

```text
Banking_Customer_Analytics_Insights_Recommendations_V2.html
```

contains the detailed business interpretation of the analysis.

It includes:

- Executive summary
- Key findings
- Income analysis
- Risk exposure analysis
- Correlation analysis
- Business recommendations
- Portfolio storyline
- Data validation notes

---

# 🔐 Environment Variables

The project contains a `.env` file for environment/database configuration.

### Important

**Do not upload real credentials to GitHub.**

Add the following to `.gitignore`:

```gitignore
.env
.ipynb_checkpoints/
__pycache__/
```

If `.env` contains database credentials, keep it local and provide a safe example file if required:

```text
.env.example
```

Example:

```env
DB_USERNAME=your_username
DB_PASSWORD=your_password
DB_HOST=localhost
DB_DATABASE=your_database
```

Never commit actual passwords or secrets.

---

# 🚀 How to Run the Project

## Step 1 — Clone the repository

```bash
git clone <your-github-repository-url>
cd Banking-Customer-Analytics
```

## Step 2 — Install Python libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Step 3 — Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
BankingEDA.ipynb
```

## Step 4 — Open Power BI

Open:

```text
Banking_dashboard.pbix
```

If Power BI asks for the CSV file location, update the data-source paths to:

```text
datasets/
```

---

# 📌 Project Limitations

The current project performs:

- Customer analytics
- Lending exposure analysis
- Risk segmentation
- Correlation analysis
- Business intelligence

However, the dataset does not provide a validated loan-default target.

Therefore, the project should **not** be described as a loan-default prediction system.

A future version could include a validated target such as:

```text
Default = 0 / 1
```

and then develop a supervised machine-learning model for probability-of-default analysis.

---

# 🎯 Skills Demonstrated

### Data Analytics

- Data understanding
- Data validation
- Exploratory Data Analysis
- Data cleaning
- Statistical analysis
- Correlation analysis
- Customer segmentation

### SQL

- SELECT
- WHERE
- GROUP BY
- ORDER BY
- Aggregate functions
- Business queries
- Risk-analysis queries

### Power BI

- Data modeling
- KPI cards
- Interactive dashboards
- Slicers
- Filters
- Data visualization
- Business storytelling

### Risk Analytics

- Lending exposure
- Risk segmentation
- Customer financial profiling
- Portfolio analysis
- Risk-aware recommendations

---

# 📈 End-to-End Business Story

```text
Customer Data
      ↓
Data Validation
      ↓
EDA
      ↓
Customer Segmentation
      ↓
Risk Weighting Analysis
      ↓
Loan & Business Lending Analysis
      ↓
Correlation Analysis
      ↓
Power BI Dashboard
      ↓
Business Insights
      ↓
Risk-Aware Recommendations
```

The project demonstrates how banking customer data can be transformed into a structured analytics solution for understanding financial exposure and supporting data-driven banking decisions.

---

# ⭐ Project Summary

### Banking Customer Analytics & Risk Analytics Dashboard

**Objective:** Analyze banking customer data to understand lending exposure, risk segments, customer financial behavior, and relationships between deposits, loans, income and business lending.

**Dataset:** 3,000 customers and 25 columns.

**Tools:**

```text
Python
Pandas
NumPy
SQL
MySQL
Power BI
DAX
Jupyter Notebook
```

**Core Areas:**

```text
Customer Analytics
Risk Analytics
Lending Exposure
Customer Segmentation
Financial Analysis
Business Intelligence
Data Visualization
Business Recommendations
```

---

# 👨‍💻 Author

**Ritesh Kumar**

B.Tech — Computer Science & Engineering

### Skills

`Python` `Pandas` `SQL` `MySQL` `Power BI` `DAX` `Excel` `Data Analytics` `Business Intelligence` `Risk Analytics`
## 📄 License

This project is licensed under the MIT License.

See the [LICENSE](LICENSE) file for more information.