# Banking Customer Analytics

Exploratory data analysis and dashboarding project on a synthetic retail banking
customer dataset. The project investigates customer demographics, income bands,
account holdings, and risk profiles, and visualizes the findings through Python
notebooks and a Power BI dashboard.

## Project Contents

| File | Description |
|---|---|
| `Banking_Project.csv` | Source dataset — 1,000 customer records with demographic and financial attributes |
| `Banking_project.ipynb` | Jupyter notebook with data loading, cleaning, and exploratory data analysis |
| `Banking_project.pbix` | Power BI dashboard built on the same dataset |

## Dataset Overview

The dataset contains 1,000 customer records with fields including:

- **Demographics**: Client ID, Name, Age, Nationality, Occupation, Gender
- **Banking relationship**: Joined Bank (date), Banking Contact, Loyalty Classification, Fee Structure
- **Financial profile**: Estimated Income, Superannuation Savings, Bank Loans,
  Bank Deposits, Checking Accounts, Saving Accounts, Foreign Currency Account,
  Business Lending, Credit Card Balance, Amount of Credit Cards
- **Risk & ownership**: Risk Weighting, Properties Owned, Branch/Region IDs (`BRId`, `IAId`)

## Analysis Performed

The notebook covers:

1. **Data ingestion** — loading customer data (originally sourced from a MySQL database)
2. **Initial exploration** — `.head()`, `.describe()`, `.info()`, shape checks
3. **Feature engineering** — binning customers into Income Bands (Low / Med / High)
   based on Estimated Income
4. **Univariate analysis** — distribution plots for categorical fields (Nationality,
   Occupation, Fee Structure, Loyalty Classification, etc.)
5. **Bivariate analysis** — relationships between categorical predictors and
   Gender / Nationality
6. **Numerical analysis** — histograms and distribution checks for financial
   metrics (income, savings, loans, deposits, balances)
7. **Correlation analysis** — heatmap of correlations across numerical financial
   features

## Power BI Dashboard

`Banking_project.pbix` presents an interactive dashboard view of the same data,
suitable for business-facing reporting (income segmentation, account balances,
customer demographics, etc.). Open it with Power BI Desktop to explore.

## Getting Started

### Requirements
