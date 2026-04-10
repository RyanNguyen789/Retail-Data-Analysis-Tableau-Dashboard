# Retail-Data-Analysis-Tableau-Dashboard
Exploratory data analysis and interactive Tableau dashboard examining consumer and small business. The goal was to explore customer behavior, identify balance  trends, uncover product concentration risks, and deliver actionable  insights for leadership through an interactive Tableau dashboard.

Link to dashboard: https://public.tableau.com/app/profile/ryan.nguyen5507/viz/RetailBankingDashboard_17754849836060/2024RetailBanking

## 2024 Retail Banking Data Analysis

### Project Overview
This project analyzes 2024 retail banking data for 500 customers 
and 862 accounts, split evenly between Consumer and Small Business 
segments. The goal was to explore customer behavior, identify balance 
trends, uncover product concentration risks, and deliver actionable 
insights for leadership through an interactive Tableau dashboard.

### Business Questions Answered
- How did account balances change throughout 2024?
- Which product types contribute the most to total balances?
- Which customer segments and age groups drive the most value?
- Which states contribute the most to balances?
- How does account tenure relate to customer value?
- Where are the cross-sell and growth opportunities?

### Dataset
Two datasets provided in Excel format:
- RetailBanking_Customers — 500 unique customers
  - Customer ID, Date of Birth, State
- RetailBanking_Accounts — 862 accounts
  - Account Number, Product Type, Customer ID,
    Account Open Date, Monthly Balances (Jan–Dec 2024)

Note: This dataset contains dummy/synthetic data only.
No real customer information is included.

### Data Preparation & Cleaning
- Removed 366 duplicate customer rows
  (866 raw rows → 500 unique customers)
- Joined two tables on Customer ID using Left Join
- Derived Customer Segment from ID prefix
  (CUST = Consumer, BUS = Small Business)
- Calculated Age as of Dec 31, 2024
  and grouped into 5 cohorts
- Unpivoted 12 monthly balance columns
  into Month + Balance fields (10,392 total rows)
- Calculated Account Tenure and grouped
  into 4 bands (1–3, 4–6, 7–9, 10+ years)
- Flagged 37 zero-balance accounts
  as potentially dormant

### Key Findings
1. Total balances declined 5.4% from $49.1M
   in January to $46.5M in December
2. Mortgage accounts represent 61% of total
   balances ($346.9M) from just 12% of accounts
3. 65+ customers hold the largest balance
   at $164.6M but represent a declining cohort
4. Small businesses represent 50% of customers
   but only 19% of total balances — limited
   to Savings and Money Market only
5. Customers with 10+ years hold $256.5M —
   nearly 3x the 1–3 year cohort
6. Florida leads all states at $72.3M, linked
   to retiree concentration

### Recommendations
- Launch a 65+ retention program to slow
  balance drawdowns
- Expand small business product suite —
  introduce Checking, Time Deposits,
  and commercial lending
- Target 35–49 age segment for cross-sell
  campaigns
- Reduce mortgage concentration risk by
  growing deposit product balances
- Build a younger customer acquisition
  strategy for long-term growth

### Tools & Technologies
- Tableau Public — dashboard and visualization
- Microsoft Excel — raw data source
- PowerPoint — executive presentation

### Dashboard
View the live interactive Tableau dashboard here:
[Insert your Tableau Public link]

### Files in This Repository
- RetailBankingDataset.xlsx — raw data
- RetailBanking_Analysis_2024.xlsx
  — cleaned and analyzed data with Tableau-ready
  flat table
- 2024_Retail_Banking_Presentation.pptx
  — executive presentation slides
- README.md — project documentation
