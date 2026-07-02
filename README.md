# 💰 Forecast vs Actual Financial Dashboard | Power BI FP&A Project

![Power BI](https://img.shields.io/badge/Power%20BI-Business%20Intelligence-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Financial%20Analytics-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-green)
![Excel](https://img.shields.io/badge/Dataset-Excel-success)
![License](https://img.shields.io/badge/License-MIT-brightgreen)

---

# 📌 Project Overview

The **Forecast vs Actual Financial Dashboard** is an interactive **Power BI** solution designed for **Financial Planning & Analysis (FP&A)**. It compares planned IT budgets (Forecast) with actual spending, enabling finance teams to monitor budget performance, identify variances, and make informed business decisions.

The dashboard analyzes **11,027 financial records** across **38 IT departments**, **25 cost elements**, **18 countries**, and **12 months (2020)** using Power BI, DAX, and Power Query.

---

# 🎯 Project Objectives

- Compare Forecast vs Actual spending
- Track budget variance ($ and %)
- Monitor departmental performance
- Analyze country-wise IT budgets
- Identify major cost drivers
- Enable interactive filtering and drill-down
- Build an executive-level FP&A dashboard

---

# 📊 Dataset Information

| Feature | Details |
|----------|----------|
| Dataset | Forecast.csv + Actual Dataset |
| Total Records | 11,027 |
| Departments | 38 |
| Cost Elements | 25 |
| Countries | 18 |
| Time Period | January 2020 – December 2020 |
| Tool | Microsoft Power BI |

---

# 📈 Financial Snapshot

| KPI | Value |
|------|-------|
| Total Forecast | **$261,051,603** |
| Positive Forecast | **$277,532,873** |
| Negative Forecast | **-$16,481,270** |
| Countries | **18** |
| IT Departments | **38** |
| Cost Elements | **25** |
| Peak Forecast Month | **October 2020 ($24.35M)** |
| Lowest Forecast Month | **January 2020 ($17.59M)** |

---

# 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel
- Data Modeling
- Business Intelligence
- Financial Planning & Analysis (FP&A)

---

# 📂 Repository Structure

```text
Forecast-Vs-Actual-Dashboard/
│
├── Forecast.csv
├── Actual.csv
├── ForecastVsActualDashboard.pbix
├── ForecastVsActual_Dashboard_Report.pdf
├── README.md
│
├── images/
│   ├── dashboard.png
│   ├── kpi_cards.png
│   ├── variance_chart.png
│   ├── waterfall.png
│   ├── treemap.png
│   └── dashboard_preview.png
```

---

# 📊 Dashboard Features

### KPI Cards

- Total Forecast
- Total Actual
- Variance ($)
- Variance (%)

### Interactive Visualizations

- Forecast vs Actual Monthly Trend
- Variance Waterfall Chart
- Department Treemap
- Country Donut Chart
- Cost Element Bar Chart
- Matrix Table with Conditional Formatting

### Interactive Filters

- Department
- Country
- Cost Element
- Month

---

# 📊 DAX Measures

### Total Forecast

```DAX
Total Forecast =
SUM(Forecast[Forecast])
```

### Total Actual

```DAX
Total Actual =
SUM(Actual[Actual])
```

### Variance

```DAX
Variance =
[Total Forecast] - [Total Actual]
```

### Variance %

```DAX
Variance % =
DIVIDE([Variance], ABS([Total Forecast]),0)
```

### YTD Forecast

```DAX
YTD Forecast =
TOTALYTD([Total Forecast],'Date'[Date])
```

---

# 🔍 Key Business Insights

- Total IT Forecast Budget reached **$261M**.
- **USA accounts for 83.4%** of the total IT budget.
- **External Labor** is the largest expense category, contributing **31%** of the budget.
- Combined **External + Internal Labor** represents **54.6%** of total spending.
- **R2 Department** has the highest forecast budget (**$49.36M**).
- Spending peaks in **October**, while **January** records the lowest forecast.
- Around **7.6%** of forecast records contain negative values representing credits or offsets.

---

# 📊 Dashboard Architecture

The dashboard follows a **dual-table financial model**:

```
Forecast Table
        │
        │
        ▼
     Date Table
        ▲
        │
        │
Actual Table
```

This structure enables dynamic Forecast vs Actual comparisons with time intelligence.

---

# 🧹 Power Query Transformations

- Date conversion
- Numeric cleaning
- Column renaming
- Whitespace removal
- Negative value validation
- Forecast & Actual table merge
- Data type conversion

---

# 📈 Skills Demonstrated

- Financial Data Modeling
- Power BI Dashboard Development
- DAX Calculations
- Time Intelligence
- Power Query ETL
- Variance Analysis
- KPI Design
- Interactive Reporting
- Data Visualization
- FP&A Reporting

---

# 💼 Business Value

This dashboard helps organizations:

- Monitor budget performance
- Detect overspending early
- Improve financial planning
- Compare Forecast vs Actual
- Support executive decision-making
- Analyze departmental spending
- Improve financial transparency

---

# 🚀 Future Enhancements

- Rolling Forecast
- Variance Drill-through Pages
- Budget Alert System
- Multi-Year Trend Analysis
- CAPEX vs OPEX Tracking
- Headcount Integration
- Currency Conversion
- Machine Learning Forecasting

---

# 📸 Dashboard Preview

Store dashboard screenshots inside the `images` folder.

```text
images/
├── dashboard.png
├── kpi_cards.png
├── variance_chart.png
├── waterfall.png
├── treemap.png
└── dashboard_preview.png
```

---

# ▶️ Getting Started

Clone the repository:

```bash
git clone https://github.com/your-username/ForecastVSactual_dashboard_powerbi.git
```

Open the `.pbix` file using **Microsoft Power BI Desktop**.

---

# 👨‍💻 Author

**Prince Maheta**

📊 Aspiring Data Analyst | Business Intelligence Developer

🔗 GitHub: https://github.com/princemaheta2627-glitch

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

---

# 📜 License

This project is intended for educational, learning, and portfolio purposes.
