# 👥 HR Analytics Dataset — Power BI & DAX Ready

A 460-employee workforce dataset covering attrition risk, compensation, engagement, and performance — structured as a complete HR fact table with pre-calculated risk scores, satisfaction labels, and department summaries ready for Power BI data modeling.

---

## 📁 Workbook Structure (5 Sheets)

| Sheet | Purpose |
|-------|---------|
| **Employee Data** | 460 employee-level records — complete HR fact table |
| **Department Summary** | Aggregated KPIs per department including attrition, salary & risk |
| **Age & Attrition** | Age group × department cross-analysis for attrition patterns |
| **Salary by Role** | Min / Max / Avg / Median salary per job role with attrition overlay |
| **KPI Summary** | Executive HR snapshot with 16 headline metrics |

---

## 🗂️ Column Reference (30 Columns)

| Group | Fields |
|-------|--------|
| **Identity** | Employee ID, Full Name, Gender, Age, Age Group |
| **Structure** | Department, Job Role, Location, Hire Date |
| **Tenure** | Years at Company, Years in Role, Years Since Promotion, Num Companies Worked |
| **Profile** | Education Level, Education Field, Business Travel, Overtime |
| **Compensation** | Annual Salary ($) |
| **Engagement** | Job Satisfaction (1–5 + label), Work-Life Balance (1–4 + label), Environment Satisfaction (1–5 + label), Manager Rating, Training Hours |
| **Performance** | Performance Rating |
| **Attrition** | Attrition (Yes/No), Attrition Risk Score, Risk Band |

---

## 📊 Dataset Highlights

| Metric | Value |
|--------|-------|
| 👥 Total Employees | 460 across 10 Departments |
| ⚠️ Attrition Rate | 48.5% — intentionally elevated to surface meaningful patterns in Power BI |
| 💰 Avg Annual Salary | $135,622 |
| 🎂 Avg Age | 35 years |
| 📅 Avg Tenure | 3.9 years |
| 🔴 Critical Risk | 78 employees flagged |
| 🟡 High Risk | 140 employees flagged |
| 🏆 Highest Attrition Dept | Customer Support |
| 💵 Highest Paid Dept | Data & Analytics |

---

## 📺 Power BI Visualization Mapping

| Visual | Source Sheet | Fields / Notes |
|--------|-------------|----------------|
| Attrition by Department | Department Summary | Attrition Rate % — bar chart |
| Attrition by Age Group | Age & Attrition | Clustered bar by Age Group |
| Gender Distribution | Employee Data | Gender — donut chart (🔵🟣 color-coded) |
| Salary Distribution | Salary by Role | Box plot or bar chart by role / department |
| Job Role Breakdown | Employee Data | Treemap — Department → Job Role drill-through |
| Tenure vs Attrition | Employee Data | Scatter: Years at Company vs Attrition Risk Score |

---

## 🎨 Color Coding

| Column | Coding |
|--------|--------|
| Risk Band | 🔴 Critical · 🟡 High · 🟢 Low |
| Attrition | 🔴 Yes · 🟢 No |
| Job Satisfaction | Color-scaled 1–5 from low to high |
| Work-Life Balance | Color-scaled 1–4 from low to high |
| Environment Satisfaction | Color-scaled 1–5 from low to high |
| Gender | 🔵 Male · 🟣 Female |

> All satisfaction, WLB, and performance label columns carry their own color logic — visual storytelling is ready in Excel before Power BI even opens.

---

## 🛠️ Data Model Notes

- **Employee Data** is the fact table — connect Department Summary, Age & Attrition, and Salary by Role as aggregation layers via `Department`, `Age Group`, and `Job Role`
- `Attrition Risk Score` is a continuous numeric field — use in scatter plots, histograms, or as a slicer threshold
- `Risk Band` is the categorical version of the score — ideal for segmentation visuals and color-coded KPI cards
- Satisfaction and engagement fields include both **numeric scores** and **text labels** — use numeric for DAX measures, labels for tooltip/callout visuals
- `Years Since Promotion` and `Num Companies Worked` are strong attrition signal features for DAX-driven predictive visuals

---

## 🚀 Use Cases

- HR attrition and retention dashboards (Power BI / Tableau)
- Workforce segmentation and demographic analysis
- Compensation benchmarking by role and department
- Engagement and satisfaction trend reporting
- Risk band monitoring for HR intervention planning
