# Accounts & Liquidity Overview | Banking Analytics Dashboard

An interactive **Power BI** analytics dashboard designed to monitor liquidity performance, account volume distribution, customer demographics, and historical balance trends across various account types and branch locations.

---

## 📊 Executive Summary & Key Metrics

* **Total Balance:** $4.0 Billion
* **Active Balance:** $4.0 Billion
* **Total Accounts:** 95,000
* **Total Customers:** 48,000

### Key Insights
1. **Account Type Portfolio Share:**
   * **Savings Accounts:** Represent the largest share at **50%** (~$2B) of total deposits.
   * **Current Accounts:** Hold **20%** (~$1B) of total balances.
   * **Salary Accounts:** Account for **15%** (~$1B) of liquidity.
   * **Fixed Deposit & NRI:** Account for **10%** and **5%** respectively.
2. **Branch Distribution:** Balances are evenly distributed across ~150 branch IDs, with each branch consistently managing around $25M–$30M in total balances.
3. **Historical Trend:** Total balance maintained stability near $200M per annum from 2005 through 2024 before experiencing a sharp drop-off in recent years (2025–2026).
---


<img width="1201" height="749" alt="Accounts   Liquidity Overview" src="https://github.com/user-attachments/assets/e4efebb3-9a41-4ae0-b00c-b0b22e42d567" />

---

## 🛠️ Tech Stack
* **Business Intelligence:** Microsoft Power BI Desktop
* **Data Transformation:** Power Query
* **Data Modeling & Calculations:** DAX (Data Analysis Expressions)
* **Visuals:** KPI Cards, Donut Chart, Funnel/Bar Visual, Column Chart, Line Trend Visual, Interactive Slicers

---

## 📈 Dashboard Layout & Visual Features

* **KPI Summary Header:** Instant snapshot of core liquidity KPIs (Total Balance, Active Balance, Account Volume, Customer Base).
* **Portfolio Mix (Donut & Funnel Charts):** Breakdown of balance contribution across Savings, Current, Salary, Fixed Deposit, and NRI account categories.
* **Branch Liquidity (Column Chart):** Micro-level tracking of balance totals per branch across ~150 locations.
* **Time-Series Analysis (Line Chart):** Multi-year trend line capturing total liquidity trajectories from 2005 to 2026.
* **Interactive Filtering Panel:** Dynamic slicers for filtering by account **Status** and **Account Type**.

---

## ⚙️ Data Transformations & DAX Measures

### Power Query Preparation
* Cleaned and transformed transaction/account tables to handle null values in account types.
* Standardized branch ID structures and formatted date dimensions.

### Core DAX Measures

```dax
Total Balance = SUM(Accounts[Balance])
