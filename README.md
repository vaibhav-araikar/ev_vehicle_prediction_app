# ⚡ Electric Vehicle (EV) Growth Forecasting

This project focuses on projecting future trends in Electric Vehicle (EV) registrations by analyzing historical data from the Washington State Department of Licensing (DOL). It leverages machine learning techniques to estimate upcoming EV adoption patterns at the county level.

---

## 📊 Problem Overview

With the rapid rise in EV ownership, city planners and policymakers face the challenge of scaling infrastructure, especially public charging stations. Without accurate forecasting, infrastructure development may lag behind demand, leading to congestion and reduced efficiency.

### ✅ Goal
Develop a regression-based predictive model to estimate county-wise EV registrations using data spanning from early 2017 through early 2024.

---

## 🧾 Data Summary

- 📅 **Time Frame**: January 2017 to February 2024  
- 📍 **Coverage**: County-level EV registration data  
- ⚙️ **Variables**: Includes BEVs, PHEVs, non-EV counts, total vehicle population, and EV percentage share

**Dataset Source**: [Kaggle Dataset Link](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024)

---

## 🧠 Modeling Approach

- **Algorithm**: Random Forest Regressor
- **Feature Engineering**:
  - Lag features (EV totals from the last 1, 2, and 3 months)
  - 3-month rolling average of EV counts
  - Short-term percentage growth metrics
  - Linear growth slope based on the last 6 months
- **Optimization**: Applied `RandomizedSearchCV` to fine-tune hyperparameters

---

## 🔍 Evaluation Metrics

- ✅ **Mean Absolute Error (MAE)**
- ✅ **Root Mean Squared Error (RMSE)**
- ✅ **R² Score (Explained Variance)**

The model captures both historical and short-term growth patterns effectively and provides county-level EV forecasts for the next 3 years.
