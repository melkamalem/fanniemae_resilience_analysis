# Fannie Mae Portfolio Resilience & Housing Market Analysis (2022–2024)

### Project Overview
This notebook analyzes Fannie Mae’s single-family loan performance trends from **2022 to 2024**, focusing on **portfolio resilience**, **credit stress**, and **delinquency trends** using publicly available datasets.  
By combining loan-level summary metrics with data-driven KPIs, the project highlights how Fannie Mae’s loan book maintained stability amid post-pandemic market tightening.

---

###  Objectives
- Measure **portfolio resilience** using active loan ratios adjusted for prepayments and repurchases.  
- Evaluate **credit stress levels** and loss containment using internal delinquency metrics.  
- Visualize quarterly portfolio health and operational efficiency trends.  
- Correlate borrower activity (prepayments) with portfolio stickiness and resilience.  
- Deliver clear **data storytelling** that translates complex housing data into business-ready insights.

---

### Data & Methodology
| Data Source | Description | Usage |
|--------------|-------------|--------|
| `HP % v2.xlsx` | Fannie Mae summary performance metrics (1999–2025) | Core dataset filtered for 2022–2024 |
| Plotly | Interactive visualization library | Used for line and scatter charts |
| pandas + SQLite | Data preparation and KPI computation | Managed ETL and resilience metrics |
| statsmodels (OLS) | Regression engine | Added correlation trendline for prepay vs. resilience |

---

### Key KPIs Calculated
| KPI | Formula | Business Meaning |
|------|----------|------------------|
| **Resilience** | (Active ÷ (100 − Prepay − Repurchase)) × 100 | Ability to sustain performing loans |
| **Delinquency** | NPL/RPL + REO + Ever180+ | Credit stress and potential losses |
| **Stress Index** | Delinquency ÷ Resilience | Resilience-adjusted credit risk ratio |
| **Net Loss Rate** | Direct from Fannie Mae | Loss containment efficiency |

---

### Visuals
1. **Portfolio Health (2022–2024):** Resilience, Loss, and Delinquency trends  
2. **Prepayment vs Resilience:** Scatter plot with regression line  
3. **KPI Summary Table:** Aggregated quarterly metrics and computed stress index  

---

### Key Insights
- **Resilience** averaged *~92%*, reflecting Fannie Mae’s strong active loan retention.  
- **Delinquency** stayed below *2%*, signaling post-pandemic credit normalization.  
- **Stress Index** remained stable, proving effective loss controls despite interest-rate volatility.  
- **Regression analysis** showed an inverse link between prepayments and resilience—borrowers refinanced less during tightening cycles.  
- Overall, Fannie Mae’s portfolio demonstrates **strong housing-market resilience** and **credit discipline** heading into 2025.

---

### Tech Stack
`Python` · `pandas` · `Plotly` · `statsmodels` · `SQLite` · `Jupyter Notebook`

---

### Files
| File | Description |
|------|--------------|
| `FannieMae_Resilience_Analysis.ipynb` | Complete ETL + KPI + Visualization notebook |
| `HP % v2.xlsx` | Core dataset (Fannie Mae portfolio metrics) |

---

### Author
Developed by **melkam.h** — Senior Data Analyst with finance, accounting, and data science expertise, focused on transforming public data into strategic business intelligence.
