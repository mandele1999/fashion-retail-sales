# 🛍️ Fashion Retail Sales Analysis

Analyze customer behavior, product trends, and payment patterns using a fashion retail sales dataset. This project combines exploratory data analysis, machine learning modeling, and an interactive dashboard to deliver actionable insights for retail strategy and decision-making.

---

## 📦 Project Structure

```graphql
fashion-retail-sales-analysis/
├── data/
│   ├── raw/                         # Original dataset (untouched)
│   └── processed/                   # Cleaned and transformed data
├── notebooks/
│   ├── 01_data_exploration.ipynb    # EDA and insight generation
│   ├── 02_data_cleaning.ipynb       # Handling missing values & formatting
│   ├── 03_feature_engineering.ipynb # Preparing features for ML
│   ├── 04_modeling.ipynb            # ML model training & evaluation
│   └── 05_dashboard_dev.ipynb       # Prepping visuals or data for dashboard
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py        # Data wrangling and cleaning functions
│   ├── modeling.py                  # ML-related utilities
│   └── visualization.py             # Helper functions for EDA plots
├── dashboard/
│   ├── app.py                       # Streamlit or Dash app
│   └── assets/                      # Images, logos, CSS (if any)
├── reports/
│   ├── figures/                     # Saved plots or visuals
│   └── summary.pdf                  # Final report or slide deck
├── docs/
│   └── data_description.md  # Data catalog/overview
├── tests/
│   └── test_utils.py                # (Optional) Unit tests for core functions
├── README.md
├── requirements.txt
└── .gitignore
```
---
## Dataset Overview

The dataset contains 3,400 records of fashion retail sales, including:
- Item purchased
- Purchase amount
- Review rating
- Purchase date
- Payment method  
🟡 Missing values are present in `Purchase Amount` and `Review Rating`.

> For detailed information, see [`docs/data_description.md`](docs/data_description.md)

---

## 🔍 Objectives

- Explore customer purchasing behavior and product trends
- Clean and preprocess raw transactional data
- Train machine learning models to predict:
  - Purchase amount
  - Review rating (optional)
- Create a dashboard to visualize:
  - Popular products
  - Preferred payment methods
  - Purchase patterns over time

---

## 🧠 Machine Learning

ML models will be applied to:
- Predict missing or future purchase amounts
- Segment customers based on purchase behavior (optional clustering)

Techniques explored:
- Linear Regression, Decision Trees, Random Forests
- Feature engineering for time/date, product popularity, etc.

---

## 🖥️ Dashboard

An interactive dashboard built using:
- **Streamlit** (for web app)  
OR  
- **Tableau** (if dashboard is BI-focused)

Key features:
- Filter by item, date, payment method
- View sales trends and top products
- Compare purchase behavior across time

---

## ⚙️ Installation

Clone the repo and install dependencies:
```bash
git clone https://github.com/mandele1999/fashion-retail-sales-analysis.git
cd fashion-retail-sales-analysis
pip install -r requirements.txt
