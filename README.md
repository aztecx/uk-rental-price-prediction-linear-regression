# uk-rental-price-prediction-linear-regression
Predicting UK rental prices using linear regression with regularisation (Ridge/Lasso)

---

## 1. Project Overview

**Goal:**
Build a model that estimates the rental price of a property from its features (e.g. location, number of bedrooms, size).

**Type of problem:**
- Supervised learning 
- **Regression** (target is a numeric price)

---

## 2. Dataset

For this project I use the **UK Rental Properties Dataset** from Kaggle:

- Title: **UK Apartments Dataset (UK Rental Properties Dataset)**
- Source: [Kaggle – UK Rental Properties Dataset](https://www.kaggle.com/datasets/georgejnr/uk-rental-properties-dataset)
- Type: tabular data (CSV)

---


Planned structure:

```text
uk-rental-price-prediction-linear-regression/
  ├─ data/         # raw and processed data (or download scripts)
  ├─ notebooks/    # Jupyter notebooks for EDA and experiments
  ├─ src/          # Python modules (data loading, training, evaluation)
  ├─ reports/      # figures, markdown/PDF reports
  ├─ requirements.txt
  ├─ LICENSE
  └─ README.md
