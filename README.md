# 🛍️ Fashion Retail Sales Analysis

Analyze customer behavior, product trends, and payment patterns using a fashion retail sales dataset. This project combines exploratory data analysis, machine learning modeling, and an interactive dashboard to deliver actionable insights for retail strategy and decision-making.

---

## Overview
This project analyzes transactional data from a fashion retail store to understand customer purchasing behavior and product trends. By cleaning, exploring, and modeling the data, it identifies key patterns and builds a predictive model for purchase amounts. A dashboard is developed to visualize sales trends, payment preferences, and product popularity—offering insights that could guide inventory, marketing, and payment strategies in fashion retail.


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

## Objectives

To explore and model customer purchasing behavior in the fashion retail sector by analyzing transactional data. 
The project aims to:
- Extract actionable insights on sales trends, product popularity, customer segments, and payment preferences.
- Train machine learning models for predictive and behavioral analysis
- Deliver insights through an interactive dashboard to support inventory, marketing, and business strategy in fashion retail.

## Goals
- Explore customer purchasing behavior and product trends
- Clean and preprocess raw transactional data
- Train machine learning models to:
  - Predict purchase amount
  - Segment customers based on behaviour
  - Predict review rating _(optional)_
- Create a dashboard to visualize:
  - Popular products & purchase patterns over time
  - Preferred payment methods
  - Customer segments & Spend profiles

---

## Machine Learning

This project includes two core ML tasks:

- Purchase Amount Prediction:
Train regression models to predict transaction amounts based on item type, date, payment method, etc.

- Customer Segmentation:
Use unsupervised learning (e.g., K-Means) to cluster customers based on behavioral features such as purchase frequency, amount, and review patterns.

> Bonus: Explore predicting customer review ratings using classification/regression models


### Techniques Used

- Linear Regression, Decision Trees, Random Forests
- K-Means Clustering or Hierarchical Clustering

Feature engineering: time-based patterns, product popularity, review ratings
---

## Dashboard

An interactive dashboard built using:
- **Streamlit** (for web app)  
OR  
- **Tableau** (if dashboard is BI-focused)

Key features:
- Filter by item, date, and payment method
- View:
  - Sales trends and top-performing products
  - Customer segmentation results and spend profiles
  - Preferred payment methods
- Support business questions like:
  - _Which items drive the most revenue?_
  - _Which customer segments spend more?_
  - _What’s the seasonal purchase trend?_
---

## Installation

Clone the repo and install dependencies:
```bash
git clone https://github.com/mandele1999/fashion-retail-sales-analysis.git
cd fashion-retail-sales-analysis
pip install -r requirements.txt
```
Run the dashboard(Streamlit version):
```bash
streamlit run dashboard/app.py
```

## Reports & Visuals

All visuals used in the project and final summary reports can be found in:
- `reports/figures/`
- `reports/summary.pdf`

## Contributing
Feel free to fork the repo and open a PR. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines

## License
MIT License. See [LICENSE](LICENSE) for details.

## Acknowledgements
- Dataset from [Kaggle](https://www.kaggle.com/datasets/atharvasoundankar/fashion-retail-sales)
- Open-source community for the awesome tools.

