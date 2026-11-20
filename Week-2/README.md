# Week 2: Advanced Data Visualization & Restaurant Sales Analytics

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Seaborn%20%7C%20Matplotlib%20%7C%20Plotly-teal.svg)]()
[![Internship](https://img.shields.io/badge/Internship-Yuvaintern%20Data%20Science-navy.svg)]()

## Overview
This repository contains the **Week 2 Project Submission** for the **Yuvaintern Data Science with Python** internship program. The project implements an end-to-end exploratory visual analytics pipeline on a reproducible dataset of **300 simulated restaurant transactions**, demonstrating statistical storytelling across static and interactive visualization libraries.

> **Synthetic Data Disclosure:** The dataset used in this notebook is synthetically generated (`np.random.seed(42)`). Observed statistical relationships—including the $r = 0.865$ correlation between `total_bill` and `tip`—are mathematical artifacts of the simulation equations. All business recommendations are framed strictly as illustrative analytical hypotheses requiring validation on historical POS data.

---

## Project Objectives
1. **Univariate Distribution Analysis:** Profile check totals using a 20-bin histogram, Kernel Density Estimation (KDE), and median threshold line.
2. **Bivariate Regression Modeling:** Quantify linear scaling and heteroscedastic variance between bill totals and dollar tips (`r = 0.865`).
3. **Multi-Factor Categorical Comparison:** Evaluate average bill performance across service days (`Thursday`–`Sunday`) and meal periods (`Lunch` vs. `Dinner`) with 95% confidence intervals.
4. **Party-Size & Multivariate Correlation Analysis:** Inspect spending dispersion across party sizes (`1`–`6` guests) and map pairwise Pearson correlations across five numerical metrics.
5. **Interactive Visual Exploration:** Build an interactive Plotly box-and-points chart to inspect daily `tip_percentage` distributions.

---

## Dataset Schema (`n = 300`)
| Column | Type | Description |
| :--- | :--- | :--- |
| `total_bill` | `float64` | Simulated total check amount ($10.00 – $100.00, uniform distribution) |
| `size` | `int64` | Number of guests per party (`1` to `6`) |
| `day` | `object` | Day of service (`Thursday`, `Friday`, `Saturday`, `Sunday`) |
| `time` | `object` | Meal shift (`Lunch`, `Dinner`) |
| `smoker` | `object` | Seating category (`Yes`, `No`) |
| `tip` | `float64` | Dollar tip calculated as `total_bill * Uniform(0.10, 0.25)` |
| `tip_percentage` | `float64` | Engineered KPI: `(tip / total_bill) * 100` |
| `bill_per_person` | `float64` | Engineered KPI: `total_bill / size` |

**Data Quality Verification:** `0` missing values, `0` duplicate records across all 300 rows.

---

## Repository Structure
```text
Week-2-Advanced-Data-Visualization/
│
├── README.md                                  # Project documentation & summary findings
├── Week_2_Advanced_Data_Visualization.ipynb   # Google Colab / Jupyter Notebook with full code & outputs
├── Week_2_Project_Report.docx                 # Formal internship project report with embedded visuals
├── submission_description.txt                 # Ready-to-submit portal summary
│
└── visualizations/
    ├── visualization_1.png                    # Histogram + KDE of Total Bill Distribution
    ├── visualization_2.png                    # OLS Regression Plot: Total Bill vs. Tip
    ├── visualization_3.png                    # Grouped Bar Chart: Average Bill by Day & Meal Period
    ├── visualization_4.png                    # Boxplot + Stripplot: Total Bill by Party Size
    ├── visualization_5.png                    # Annotated Pearson Correlation Heatmap
    └── visualization_6.html                   # Interactive Plotly Boxplot: Tip Percentage by Day
```

---

## Key Numerical Findings

### Overall Benchmarks
* **Total Transactions:** 300
* **Average Bill:** $54.57 (Median: $56.05)
* **Average Tip:** $9.73 (Mean Tip Percentage: 17.94%)
* **Average Party Size:** 3.49 guests
* **Bill-to-Tip Correlation (`r`):** 0.865

### Performance by Day of Week
| Day | Transactions | Average Bill | Total Sales | Average Tip | Mean Tip % |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Thursday** | 86 | $53.39 | $4,591.36 | $9.35 | 17.64% |
| **Saturday** | 77 | $57.70 | $4,442.99 | $10.20 | 17.91% |
| **Friday** | 81 | $53.10 | $4,300.83 | $9.69 | 18.35% |
| **Sunday** | 56 | $54.20 | $3,035.34 | $9.71 | 17.84% |

### Performance by Meal Period
| Meal Period | Transactions | Average Bill | Total Sales | Average Tip |
| :--- | :---: | :---: | :---: | :---: |
| **Lunch** | 150 | $56.22 | $8,432.54 | $10.16 |
| **Dinner** | 150 | $52.92 | $7,937.99 | $9.29 |

---

## How to Run Locally or in Google Colab
1. Clone this repository or upload `Week_2_Advanced_Data_Visualization.ipynb` to Google Colab.
2. Install required packages if running locally:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly
   ```
3. Run all cells sequentially (`Runtime > Run all`) to reproduce the dataset (`seed=42`), summary statistics, and all six visualizations.
