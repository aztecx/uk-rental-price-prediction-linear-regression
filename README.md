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

'''
---

##  Results so far

This project currently includes two simple linear regression models:

| Model ID | Features used                       | RMSE (test) | R² (test) |
|---------|--------------------------------------|-------------|-----------|
| M1      | Rooms only                           | ≈ £2198.52  | 0.013     |
| M2      | Rooms + Location (one-hot encoded)   | ≈ £2121.31  | 0.081     |

### Interpretation

- **Adding Location helps**:  
  - RMSE decreased from ~£2199 =>  ~£2121 (about £77 less error on average).  
  - R² increased from ~0.013 =>  ~0.081 (from 1.3% to 8.1% of variance explained).

- **But the model is still limited**:
  - Even with Location, R² is low, so the model explains only a small part of the variation in rental prices.
  - This suggests other factors are important (more fine-grained location, property type, description text, etc.).

- **What this shows about my skills**:
  - I can clean and prepare real-world tabular data (prices, rooms, locations).
  - I can build baseline and improved regression models.
  - I can compare models using RMSE and R² and reason about feature importance.

