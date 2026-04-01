# CAC & Retention Cohort Analysis

**Georgetown MSBA — MARK 6601: Strategic Marketing Analytics**  
Case Study 2

---

## Overview

This case study analyzes customer acquisition cost (CAC), user engagement, and retention for a consumer social platform using publicly reported Q2 FY2019 metrics and a proprietary cohort dataset. The analysis covers three interconnected questions central to growth-stage marketing strategy:

1. **Revenue per user and acquisition cost efficiency** — Is the platform generating more revenue than it spends to acquire users?
2. **User engagement trends** — Are users becoming more engaged over time?
3. **Cohort retention and revenue analysis** — How well does the platform retain users, and what is the revenue impact across cohorts?

---

## Questions & Key Findings

### Q1: ARPU and Customer Acquisition Cost

Using Q2 FY2019 financials broken out by geographic segment, average revenue per user (ARPU) and cost per acquired user (CPA) were calculated.

| Metric | Value |
|---|---|
| ARPU — US & Canada | $32.60 |
| ARPU — Europe | $10.52 |
| ARPU — Asia Pacific | $3.01 |
| Cost Per Acquired User (CPA) | $22.81 |
| ARPU / CPA Ratio | 1.43x |

The 1.43x ARPU/CPA ratio indicates the platform generates $1.43 in revenue for every dollar spent acquiring a user — a positive return at the aggregate level, though the ratio varies substantially by region.

---

### Q2: User Engagement — L28 Power User Curve & DAU/MAU

Engagement was assessed by comparing 2017 vs. 2018 user activity using the L28 power user curve (days active in the last 28 days) and the DAU/MAU ratio.

| Metric | 2017 | 2018 |
|---|---|---|
| DAU/MAU Ratio | 29% | 44% |
| Avg. Days Active (L28) | 8 days | 12 days |

The DAU/MAU ratio increased 15 percentage points year-over-year, and average days active grew by 50%. The L28 power user curve shifted markedly toward higher-frequency usage, reflecting a more engaged and retained user base.

---

### Q3: Cohort Retention & Revenue Projection

Retention was analyzed by acquisition cohort (January–August 2017). Each cohort was tracked monthly post-acquisition to identify retention patterns and project forward revenue.

**Key observations:**
- Cohorts acquired in **February–April** showed weaker retention
- Cohorts acquired in **May–July** showed meaningfully stronger retention curves
- At $10/month per active subscriber, total revenue across all 2017 cohorts would be **$346,510** (34,510 total active customers × $10)

The variation across cohorts suggests differences in marketing campaign, acquisition channel, product launches, or user demographics. The report recommends further investigation to identify the key drivers.

---

## Repository Structure

```
.
├── data/
│   └── data.xlsx              # Raw input data (Q2 engagement and Q3 cohort datasets)
├── analysis/
│   └── case_2_analysis.xlsx   # Working analysis workbook (6 sheets: Q1 metrics,
│                              #   power user curve, DAU/MAU, cohort retention)
├── reports/
│   ├── case_2_report.pdf      # Final case study report (PDF)
│   └── case_2_report.docx     # Final case study report (Word)
└── README.md
```

### Analysis Workbook Sheets

| Sheet | Contents |
|---|---|
| `q1` | ARPU, MAU, NUA%, CPA, and ARPU/CPA ratio calculations |
| `q2` | Raw Q2 engagement data |
| `q2_clean` | Processed daily activity records (655 rows) |
| `q2_dau_mau` | Aggregated DAU/MAU statistics by month and year |
| `q2_viz` | 2017 vs. 2018 power user curve visualization data |
| `q3` | Cohort retention tracking with monthly retention status per cohort |

---

## Methods

All analysis was performed in Excel. Techniques used:

- **ARPU/CPA calculation** from segmented financial disclosures
- **DAU/MAU ratio** aggregation from daily activity logs
- **L28 power user curve** constructed from individual-level activity flags
- **Cohort retention curves** using month-over-month retention rates by acquisition cohort
- **Revenue projection** using retained user counts and a fixed subscription price assumption

---

## Course Context

This case study was completed as part of MARK 6601: Strategic Marketing Analytics in the Georgetown McDonough School of Business MSBA program. The dataset is based on publicly reported Facebook Q2 FY2019 earnings data combined with a provided customer-level engagement and cohort dataset.
