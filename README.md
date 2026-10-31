# AAL Australian Apparel Sales — Exploratory Data Analysis (Q4 2020)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/saihaanmohammed120-cell/aal-sales-eda/blob/main/AAL_Sales_EDA_Final_Colab.ipynb)

Course-end project for **Applied Data Science with Python** — part of the *Professional Certificate Course in Generative AI and Machine Learning* (E&ICT Academy, IIT Kanpur / Simplilearn).

A complete, structured exploratory data analysis of **7,560 Australian apparel sales records from Q4 2020**: from the business question through data-quality profiling, cleaning, visualization, and evidence-based recommendations.

## What's inside

| File | Description |
|---|---|
| `AAL_Sales_EDA_Final_Colab.ipynb` | The full analysis — 60 cells (35 markdown + 25 code) with explanations, tables, and chart outputs |
| `AusApparalSales4thQrt2020.csv` | The dataset (7,560 rows × 6 columns) required to re-run the notebook |

## Analysis workflow

1. **Business question** — define what the analysis must answer
2. **Load & describe** — dataset overview and column profiling
3. **Data-quality checks** — missing values, duplicates, invalid categories, date coverage
4. **Cleaning & validation** — category cleanup, numeric validation, whitespace trimming
5. **Normalization** — min-max scaling without overwriting original values
6. **Descriptive statistics** — Sales and Unit distributions
7. **Comparisons** — by state, customer group, state-by-group, and time of day
8. **Trends** — daily, weekly, monthly, and quarterly summaries with charts
9. **Distributions** — Seaborn distribution plots and box plots
10. **Conclusion** — business recommendations, limitations, and CSV exports of summary tables

## Verified data findings

- 7,560 rows × 6 columns — **zero missing cells, zero duplicate rows**
- 340,302,500 total recorded sales · 136,121 total units
- Every row follows `Sales = Unit × 2,500`; no negative values
- Two Q4 dates have no records (2020-10-31, 2020-12-31) — treated as *missing*, not zero
- Every observed date has 84 records (3 time periods × 7 states/territories × 4 groups)

> Note: the file covers only Q4 2020 and does not label the currency — conclusions are limited to the data available.

## Tech

Python · pandas · NumPy · Matplotlib · Seaborn · Google Colab

## Run it

**Option A — Google Colab (easiest):** click the *Open in Colab* badge above, then *Runtime → Run all*. If prompted, upload `AusApparalSales4thQrt2020.csv`.

**Option B — Locally:**
```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook AAL_Sales_EDA_Final_Colab.ipynb
```
Make sure `AusApparalSales4thQrt2020.csv` sits next to the notebook.
