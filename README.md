# E-commerce Customer Churn Analysis

##  Project Overview
Customer churn is a major challenge in e-commerce businesses, where customers can easily switch to competing platforms. This project analyzes customer purchasing behavior to identify churned customers and uncover patterns associated with long-term inactivity.

For this project, **customer churn is defined as customers who have not made any purchase in the last six (6) months**, relative to the most recent transaction date in the dataset.

The analysis focuses on transaction-level data and applies customer-level aggregation and behavioral metrics to support retention and revenue optimization strategies.

---

##  Project Objectives
The primary objectives of this project are to:

- Identify churned and active customers based on purchase inactivity
- Measure churn rates across customer segments
- Analyze purchasing behavior using Recency, Frequency, and Monetary (RFM) metrics
- Generate business insights that can inform customer retention strategies
- Demonstrate real-world data science workflows suitable for portfolio presentation

---

##  Business Context
In e-commerce, customer churn is rarely explicit (e.g., account deletion). Instead, it is typically inferred from prolonged inactivity. Understanding when and why customers stop purchasing enables businesses to:

- Reduce customer acquisition costs
- Improve customer lifetime value (CLV)
- Design targeted re-engagement campaigns
- Optimize marketing and retention spend

---

##  Dataset Description
The project uses the **Online Retail Dataset**, which contains historical transaction records from an e-commerce business.

### Key Features:
- **InvoiceNo**: Unique invoice number (cancellations indicated by prefix 'C')
- **StockCode**: Product identifier
- **Description**: Product description
- **Quantity**: Number of units purchased
- **InvoiceDate**: Date and time of transaction
- **UnitPrice**: Price per unit
- **CustomerID**: Unique customer identifier
- **Country**: Customer’s country of residence

---

##  Churn Definition
A customer is classified as **churned** if:
> They have not made any purchase in the last **6 months** from the most recent transaction date in the dataset.

This definition reflects common industry practice in e-commerce retention analytics.

---

##  Tools & Technologies
- **Python**
- **Pandas & NumPy** – data manipulation and analysis
- **Matplotlib & Seaborn** – data visualization
- **Jupyter Notebook** – exploratory analysis and reporting
- **Git & GitHub** – version control and portfolio presentation

---

##  Analysis Scope
The project covers the following analytical steps:

- Data loading and inspection
- Data cleaning and preprocessing
  - Removal of cancelled transactions
  - Handling missing customer identifiers
  - Validation of quantities and prices
- Customer-level aggregation
- Feature engineering using RFM metrics
- Churn labeling based on inactivity threshold
- Exploratory Data Analysis (EDA) and visualization
- Business insight generation

---

##  Project Structure
```text
ecommerce-churn-analysis/
│
├── data/
│   ├── raw/                # Original dataset
│   └── processed/          # Cleaned and transformed data
│
├── notebooks/
│   ├── 01_eda.ipynb        # Data Cleaning
|   ├── 02_eda.ipynb        # Feature Engineering
|   ├── 03_churn_eda.ipynb  # EDA
│
├── src/
│   ├── data_cleaning.py
│   ├── feature_engineering.py
│   └── utils.py
│
├── reports/
│   ├── figures/            # Generated charts and plots
│   └── summary.md          # Business insights summary
│
├── requirements.txt
└── README.md
