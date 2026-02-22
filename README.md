# Online Retail II — Funnel, Cohort & AARRR Analysis

## Key Findings

| Insight | Detail |
|---|---|
| **Revenue Concentration** | Top 23% of customers generate 80% of total revenue (£17.7M) |
| **One-Time Buyer Problem** | 27.6% of customers make only 1 purchase — first-month churn is the biggest leak |
| **Strong Repeat Base** | 72.4% of customers are repeat buyers (2+ orders) |
| **Geographic Over-Dependence** | UK accounts for 83.0% of total revenue across 5,878 customers |
| **Seasonal Revenue Spike** | Q4 (Sep–Nov) shows a sharp revenue peak driven by holiday shopping |

## Analysis Overview

### Monthly Revenue Trend
![Monthly Revenue](images/01_monthly_revenue.png)

### Customer Engagement Funnel
![Funnel](images/06_funnel.png)

### Cohort Retention Heatmap
![Cohort Heatmap](images/07_cohort_heatmap.png)

### Average Retention Curve
![Retention Curve](images/09_avg_retention.png)

### Revenue Pareto (Concentration)
![Pareto](images/05_pareto.png)

### AARRR: ARPU & AOV Trends
![ARPU AOV](images/11_arpu_aov.png)

### Summary Dashboard
![Summary](images/12_summary_dashboard.png)

## Business Recommendations

1. **Reduce First-Month Churn** — Implement a post-purchase email sequence (day 7, 14, 30) with personalized product recommendations
2. **Loyalty Program** — Create tiered rewards for top 23% revenue-generating customers to increase retention and LTV
3. **International Expansion** — Prioritize top non-UK markets (Netherlands, EIRE, Germany, France) with localized marketing
4. **Q1 Retention Campaign** — Launch targeted re-engagement campaigns in January to retain holiday-season acquired customers

## Dataset

- **Source**: [Online Retail II (UCI)](https://archive.ics.uci.edu/dataset/502/online+retail+ii)
- **Period**: December 2009 – December 2011
- **Records**: ~1,067,000 transactions (cleaned to ~723,000)
- **Customers**: 5,878 unique customers
- **Country**: Primarily UK-based online retailer

## Tech Stack

- Python 3.11
- pandas, NumPy — data manipulation
- Matplotlib, Seaborn — visualization
- Jupyter Notebook — interactive analysis
- openpyxl — Excel file reading

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/user-funnel-cohort-analysis.git
cd user-funnel-cohort-analysis

# 2. Create virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Download dataset
# Download "Online Retail II" from UCI/Kaggle and place the .xlsx file in data/

# 5. Run the notebook
jupyter notebook notebooks/analysis.ipynb
```

## Project Structure

```
user-funnel-cohort-analysis/
├── .gitignore
├── README.md
├── requirements.txt
├── data/                    # Dataset (not tracked in git)
│   └── online_retail_II.xlsx
├── notebooks/
│   └── analysis.ipynb       # Full analysis notebook
└── images/                  # Chart PNGs for README
    ├── 01_monthly_revenue.png
    ├── 02_monthly_customers.png
    ├── 03_top10_countries.png
    ├── 04_order_frequency.png
    ├── 05_pareto.png
    ├── 06_funnel.png
    ├── 07_cohort_heatmap.png
    ├── 08_cohort_size.png
    ├── 09_avg_retention.png
    ├── 10_acquisition.png
    ├── 11_arpu_aov.png
    └── 12_summary_dashboard.png
```
