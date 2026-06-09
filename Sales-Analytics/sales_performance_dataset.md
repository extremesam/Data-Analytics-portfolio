# 🏆 Sales Performance Dataset — Power BI & DAX Ready

A 24-month order-level sales dataset covering 6 Nigerian regions, 40 products, and 10 salespersons — structured as a clean fact table ready for Power BI data modeling and DAX measures.

---

## 📁 Workbook Structure (5 Sheets)

| Sheet | Purpose |
|-------|---------|
| **Sales Data** | 602 order-level transactions — the full fact table for your data model |
| **Monthly Sales Summary** | 24-month revenue, profit, targets & variances for trend visuals |
| **Product Performance** | All 40 products ranked by revenue with margin analysis |
| **Region Performance** | Revenue, profit & target variance across 6 Nigerian regions |
| **KPI Summary** | Executive headline metrics at a glance |

---

## 🗂️ Column Reference (23 Columns)

| Group | Fields |
|-------|--------|
| **Time** | Order ID, Order Date, Month, Quarter, Year |
| **Geography** | Region, City |
| **Customer** | Customer Name, Customer Segment (Enterprise / SMB / Gov / Startup) |
| **Product** | Salesperson, Category, Product |
| **Financials** | Unit Price, Quantity, Discount %, Discount Amount |
| **Performance** | Revenue, Cost, Profit, Profit Margin %, Sales Target, Target Variance $, Target Variance % |

---

## 📊 Dataset Highlights

| Metric | Value |
|--------|-------|
| 🧾 Total Orders | 602 across 24 months (Jan 2023 – Dec 2024) |
| 💰 Total Revenue | $969K |
| 📈 Total Profit | $371K |
| 🎯 Avg Profit Margin | 38.4% |
| 📦 Categories | 5 |
| 🛒 Products | 40 |
| 🌍 Regions | 6 |
| 👥 Customers | 30 |
| 🧑‍💼 Salespersons | 10 |
| 🏆 Top Region | Lagos |
| 🥇 Top Product | Laptop Pro 15" |
| 📱 Top Category | Electronics |

---

## 📺 Power BI Visualization Mapping

| Visual | Source Sheet | Fields / Notes |
|--------|-------------|----------------|
| Monthly Sales Trend | Monthly Sales Summary | Revenue + Profit by Month — line chart |
| Revenue by Region | Region Performance | Bar chart, color by region |
| Top 10 Products | Product Performance | Filter Revenue Rank ≤ 10 — top 10 highlighted in 🟡 gold |
| Customer Contribution | Sales Data | Customer Name + Revenue — treemap or bar chart |
| Profit vs Target | Monthly Sales Summary | Target Variance $ — conditional 🟢 green / 🔴 red |
| Sales by Category | Sales Data | Category field — color-coded donut / pie chart |

---

## 🎨 Color Coding

| Column | Coding |
|--------|--------|
| Category | Unique color per product category |
| Customer Segment | Enterprise · SMB · Gov · Startup — color-coded for visual hierarchy |
| Target Variance | 🟢 Positive (above target) · 🔴 Negative (below target) |
| Top 10 Products | 🟡 Gold highlight on Revenue Rank ≤ 10 rows |

> Category and Customer Segment columns are pre-color-coded in Excel — your visual hierarchy is clear before you even open Power BI.

---

## 🛠️ Data Model Notes

- **Sales Data** is the fact table — connect all other sheets as dimension/summary tables via `Month`, `Region`, `Product`, or `Category` fields
- `Quarter` and `Year` columns enable DAX time intelligence functions out of the box
- `Discount %` and `Discount Amount` are separated for flexible margin analysis
- `Target Variance $` and `Target Variance %` are pre-calculated — use directly in KPI cards or conditional formatting visuals

---

## 🚀 Use Cases

- Sales performance dashboards (Power BI / Tableau)
- DAX measure development and data modeling practice
- Regional and product-level revenue analysis
- Salesperson performance tracking and leaderboard visuals
- Budget vs actual variance reporting
