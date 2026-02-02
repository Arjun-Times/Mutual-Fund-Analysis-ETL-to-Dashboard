# Mutual Fund Performance Analysis & ETL Pipeline
This project provides an end-to-end data engineering and analytics solution for evaluating Mutual Fund performance. It covers the entire lifecycle of data: from initial Exploratory Data Analysis (EDA) and cleaning in Python, to MySQL database integration, and finally Power BI visualization.

## 🚀 Project Workflow
### Data Cleaning & Wrangling:

- Handled missing values in returns_3yr and returns_5yr based on the fund_age_yr.

- Standardized financial metrics (Alpha, Beta, Sharpe, etc.) by replacing null placeholders (-) with numeric zeros to ensure SQL compatibility.

- Engineered a unique Primary Key (ID) by combining scheme_name and returns_1yr to ensure data integrity during database loading.

### Database Integration (ETL):

- Established a connection between Python and a local MySQL server using mysql-connector-python.

- Automated the creation of the Mutual_Funds table and populated it row-by-row using an optimized insertion loop.

### Visualization:

Developed a Power BI Dashboard (image included in the repo) to track risk levels, expense ratios, and multi-year returns across different fund categories.

## 🛠️ Tech Stack
- Language: Python (Pandas, NumPy)

- Database: MySQL

- BI Tool: Power BI


## 📂 Key Insights from Data
- Category Distribution: The dataset primarily focuses on Equity (308 funds) and Debt (282 funds).

- Risk Profile: Evaluated funds based on Sortino and Sharpe ratios to determine risk-adjusted performance.
