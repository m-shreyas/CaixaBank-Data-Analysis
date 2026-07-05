# 🏦 Banking Financial Performance Dashboard

**A full-year 2010 KPI dashboard built in Tableau Public — analyzing $54.2M in banking transaction data across all 12 months to track spending, transaction volume, customer growth, and card activity.**

🔗 **Live Dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/shreyas.mupparapu/viz/BankFinancialDashboard/BankingPerformanceTrends2010)
🌐 **Portfolio:** [m-shreyas.github.io](https://m-shreyas.github.io)

---

## 📌 Key KPIs (Full Year 2010)

| Metric | Value |
|---|---|
| Total Spend | $54.23M |
| Avg Transaction Value | $43.71 |
| Max Active Customers | 1,133 |
| Max Active Cards | 2,841 |

---

## 📊 Dashboard Insights

- **Monthly spend** held steady between $4.1M and $4.7M all year — no material decline.
- **Transaction volume** stayed consistent (~93K–108K/month).
- **Average transaction value** was flat near $43.70, indicating stable spending behavior.
- **Active customers** grew steadily from 1,083 to 1,133 across the year.

The story: a healthy, stable year with consistent activity and steady customer growth.

---

## 🔍 Data Quality Catch

An earlier version of this dashboard showed a sharp "May collapse" in spend and volume. Rather than report it as a business decline, I traced it back to the source:

- The dashboard was fed by a **pre-aggregated extract that had been truncated mid-May** and stopped at 5 months.
- The raw source (`transactions_data.csv`, ~13M rows) actually contained a **complete May and a full Jan–Dec year**.
- I **rebuilt the monthly KPI aggregation from the raw source** for all 12 months, which removed the false cliff and revealed the true, stable trend.

**Takeaway:** validate data completeness before interpreting a trend. A single truncated month nearly turned normal data into a false crisis narrative.

---

## 🛠️ Tools & Technologies
`Tableau Public` `Microsoft Excel` `Data Validation` `KPI Dashboard Design` `Data Storytelling`

---

## 📁 Repository Contents

| File | Description |
|---|---|
| KPI Dashboard | Tableau workbook with full-year KPI views |
| Trend Analysis Visuals | Monthly spend, volume, value, and customer trends |
| Storytelling Report | Executive summary with findings and the data-quality catch |

---

*Part of Shreyas Mupparapu's data analytics portfolio — [m-shreyas.github.io](https://m-shreyas.github.io)*
