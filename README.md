# Seasonal Agriculture Performance Analysis
**VOIS AICTE Batch1 2026-2027 — Major Project**

---

## Overview

This project analyzes agricultural performance across three Indian cropping seasons —
**Kharif**, **Rabi**, and **Zaid** — using a dataset of 4,000 farm records spanning
8 states and 8 crop types.

The goal is to identify meaningful patterns, trends, relationships and differences in
agricultural performance across seasons through data analytics and visualization.

---

## Repository Contents

| File / Folder | Description |
|---|---|
| `Seasonal_Agriculture_Performance_Analysis.ipynb` | Main Jupyter Notebook — full analysis |
| `seasonal_agriculture_performance_dataset.csv` | Dataset (4,000 rows × 28 features) |
| `VOIS_Major_Project_PPT_FILLED.pptx` | Filled PowerPoint presentation |
| `ppt_charts/` | 6 chart images generated from the analysis |

---

## Dataset

| Attribute | Value |
|---|---|
| Records | 4,000 farms |
| Features | 28 columns |
| Seasons | Kharif · Rabi · Zaid |
| Crops | Rice · Wheat · Maize · Cotton · Pulses · Groundnut · Chilli · Sugarcane |
| States | Andhra Pradesh · Gujarat · Karnataka · Madhya Pradesh · Maharashtra · Punjab · Tamil Nadu · Telangana |

---

## Analysis Sections

1. **Setup & Imports** — Libraries, colour palette, display settings
2. **Data Loading & Overview** — Shape, dtypes, summary statistics, distributions
3. **Data Cleaning & Preparation** — Missing value imputation (season-wise median), duplicate check, IQR outlier detection, derived features
4. **Exploratory Data Analysis** — Histograms, KDE yield-by-season overlay
5. **Seasonal Performance Analysis** — KPI table, bar charts, box plots, profitability breakdown
6. **Environmental Conditions** — Heatmap, rainfall vs temperature, violin plots
7. **Resource Usage Analysis** — Fertilizer, pesticide, irrigation methods, water efficiency
8. **Economic Performance** — Revenue vs cost vs profit, market price, revenue per hectare
9. **Crop-wise Seasonal Analysis** — Pivot heatmaps, top crops per season, state-wise yield
9b. **Unusual & Unexpected Patterns** — Z-score outlier detection, Zaid resilience analysis
10. **Correlation & Relationships** — 16-feature correlation matrix, yield drivers, scatter plots
11. **Statistical Testing** — Kruskal-Wallis, Mann-Whitney U, Chi-square, Pearson r
12. **Key Insights & Recommendations** — Summary dashboard, 10 findings, 7 recommendations

---

## Key Findings

| # | Finding | Evidence |
|---|---------|----------|
| 1 | Kharif is the most profitable season | Highest avg yield & profit |
| 2 | Zaid has negative median profit | Weakest season by all metrics |
| 3 | Yield differs significantly across seasons | Kruskal-Wallis H=70.2, p<0.001 |
| 4 | Profit differs significantly across seasons | Kruskal-Wallis H=97.1, p<0.001 |
| 5 | Fertilizer usage is uniform across seasons | H=1.06, p=0.589 — not significant |
| 6 | Sugarcane beats Zaid season yield average | Only crop to outperform Zaid mean |
| 7 | 35.5% of Zaid farms remain profitable | Unexpected resilience |
| 8 | Seed quality is the strongest yield predictor | Highest Pearson correlation |
| 9 | Drip irrigation delivers best water efficiency | Water efficiency box plot |
| 10 | 177 farms have extreme outlier yields (\|Z\|>3) | Z-score anomaly detection |

---

## Technologies Used

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core programming language |
| pandas | Data manipulation and aggregation |
| numpy | Numerical operations, Z-score |
| matplotlib | Charts, histograms, bar plots |
| seaborn | Box plots, heatmaps, violin plots |
| scipy.stats | Kruskal-Wallis, Mann-Whitney U, Chi-square |
| Jupyter Notebook | Interactive analysis environment |

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/Guru1817/Seasonal-Agriculture-Performance-Analysis.git
cd Seasonal-Agriculture-Performance-Analysis

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scipy jupyter

# 3. Launch the notebook
jupyter notebook Seasonal_Agriculture_Performance_Analysis.ipynb
```

---

## Author

**Gurupada Nayak**  
VOIS AICTE Batch1 2026-2027  
gurupadpnayak@gmail.com
