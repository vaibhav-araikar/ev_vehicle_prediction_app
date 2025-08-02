# ⚡ Electric Vehicle (EV) Adoption Forecasting

This project aims to forecast future Electric Vehicle (EV) adoption using historical registration data provided by the Washington State Department of Licensing (DOL). The model predicts the number of EVs per county based on trends, vehicle types, and historical growth.

---

## 📊 Problem Statement

As electric vehicle (EV) adoption surges, urban planners must anticipate infrastructure needs—especially charging stations. Inadequate planning can cause bottlenecks and reduce user satisfaction.

### ✅ Objective:
Build a regression model to forecast future EV counts using historical EV registration data from 2017 to 2024.

---

## 🧾 Dataset

- 📅 Date Range: January 2017 – February 2024
- 🏙️ Geographic Scope: County-level registration data
- 🔌 Features: Battery Electric Vehicles (BEVs), Plug-in Hybrid EVs (PHEVs), Non-EVs, Total Vehicles, Percent EVs

Dataset Source: [Kaggle Dataset Link](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024)

---

## 🧠 Model

- **Algorithm Used**: Random Forest Regressor
- **Modeling Techniques**:
  - Lag features (1, 2, 3-month EV counts)
  - Rolling averages and percentage change
  - EV growth slope (trend over past 6 months)
  - RandomizedSearchCV for hyperparameter tuning

---

## 🔍 Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score (Coefficient of Determination)

Achieved:
