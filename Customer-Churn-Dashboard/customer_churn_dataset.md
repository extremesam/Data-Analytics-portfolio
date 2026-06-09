# 📊 300-Row Customer Churn Dataset

A logic-driven synthetic dataset built for churn analysis dashboards, segmentation, and predictive modeling.

---

## 📁 Workbook Structure

| Sheet | Description |
|-------|-------------|
| **Churn Data** | Full dataset — 300 rows × 18 columns, auto-filter enabled, frozen headers |
| **Summary** | Key KPI snapshot for quick reference |

---

## 🗂️ Column Reference (18 Columns)

| Column | Purpose |
|--------|---------|
| Customer ID | Unique identifier |
| Age Group | Customer segmentation |
| Gender | Customer segmentation |
| Location | Customer segmentation |
| Contract Type | Churn by contract type visualization |
| Payment Method | Churn by payment method visualization |
| Tenure (Months) | Tenure distribution chart |
| Monthly Charges | Financial metrics |
| Total Charges | Financial metrics |
| CLV (Customer Lifetime Value) | Financial metrics |
| Internet Service | Service usage vs churn |
| Phone Service | Service usage vs churn |
| Online Security | Service usage vs churn |
| Tech Support | Service usage vs churn |
| # of Services | Service usage vs churn |
| Satisfaction Score | Retention driver |
| Risk Segment | Risk segmentation analysis |
| Churn (Yes/No) | Primary target variable |

---

## 📈 Dataset Stats

- **300 customers** · **~52% churn rate**
- Churn is **logic-driven**, not random:

| High-Churn Signal | Detail |
|-------------------|--------|
| Contract Type | Month-to-Month contracts |
| Payment Method | Electronic Check payments |
| Tenure | Low tenure (< 12 months) |
| Satisfaction | Low satisfaction scores |

> All churn signals are aligned with key business insights for realistic dashboard behavior.

---

## 🎨 Color Coding

| Indicator | Meaning |
|-----------|---------|
| 🔴 Red rows | Churned customers |
| 🟢 Green rows | Active customers |
| 🟡 Risk highlights | Risk segment color bands |

---

## 🚀 Use Cases

- Customer churn dashboard (Power BI / Tableau / Looker)
- Cohort and segmentation analysis
- Predictive churn modeling (ML training data)
- KPI reporting and retention strategy design
