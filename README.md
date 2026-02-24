# Banking Customer Analytics — SQL Server + Python EDA + Power BI Dashboard

<p align="center">
  <img src="BANKLOGO.png" alt="Project logo" width="540"/>
</p>

End-to-end analytics mini-project where I:
1) connected a **SQL Server** database (via SSMS) to **Power BI** to build an interactive dashboard, and  
2) performed **Exploratory Data Analysis (EDA)** in **Python (Jupyter Notebook)** after connecting to the same database.

---

## Project Files

- **`BankingDash2026.pbix`**  
  Power BI dashboard/report (KPIs, segmentation, and portfolio views).

- **`Banking.ipynb`**  
  Jupyter notebook with Python EDA (data overview, distributions, segmentation, correlation analysis, and plots).

- **`Banking.csv`**  
  Extract of the customer dataset used for EDA (mirrors the SQL Server table used in the dashboard).

---

## Tools & Tech

- **Database:** Microsoft SQL Server (SSMS 2022)
- **BI / Visualization:** Power BI Desktop
- **Python (EDA):** pandas, numpy, matplotlib, seaborn
- **Environment:** Jupyter Notebook

---

## Dataset Overview (High-level)

The dataset represents banking customers with fields related to:
- Demographics (e.g., Gender, Nationality, Occupation)
- Products / engagement (e.g., credit cards, accounts)
- Financial behavior (e.g., deposits, loans, card balance, savings)
- Segmentation attributes (e.g., Fee Structure, Loyalty Classification, Risk Weighting)

---

## What I Built

### 1) Python EDA (Jupyter)
Key EDA components:
- Data shape, column types, descriptive statistics
- Missing value + distribution checks
- Income banding and categorical breakdowns
- Numerical distributions (histograms + KDE)
- Correlation heatmap for key financial variables

Notebook: **`Banking.ipynb`**

### 2) Power BI Dashboard
Dashboard focuses on:
- KPI cards (portfolio totals / exposure-style metrics)
- Customer segmentation views (Income Band, Loyalty, Risk Weighting)
- Drilldowns by demographics and product engagement
- Filters/slicers for interactive exploration

Report: **`BankingDash2026.pbix`**

---

## How to Run

### A) Open the Power BI Report
1. Install/launch **Power BI Desktop**
2. Open: `BankingDash2026.pbix`
3. If prompted to refresh data:
   - Update the SQL Server connection (Server/Database) OR
   - Point queries to `Banking.csv` (depending on how your model is set up)

### B) Run the Python Notebook
1. Open `Banking.ipynb` in Jupyter
2. Install dependencies if needed:
   ```bash
   pip install pandas numpy matplotlib seaborn
