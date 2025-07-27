# ☀️ Solar Panel Efficiency Prediction using ML

This project focuses on predicting solar panel efficiency using environmental and sensor data. Built as part of a machine learning hackathon, the goal was to achieve high accuracy using a robust ensemble pipeline.

## 📌 Problem Statement

Solar panels' efficiency is influenced by various environmental factors like temperature, irradiance, humidity, etc. Accurately predicting efficiency helps optimize energy production and maintenance scheduling. This project leverages supervised learning models to make those predictions.

## 🧩 Dataset

The dataset contains sensor readings related to:
- Ambient temperature
- Panel temperature
- Irradiance
- Wind speed
- Humidity
- Time-based features

Target: **Efficiency** of the solar panel.

## ⚙️ Pipeline Overview

1. **Data Preprocessing**
   - Handling missing values
   - Outlier treatment
   - Feature scaling

2. **Feature Engineering**
   - Creating time-based and polynomial features
   - Encoding categorical data (if any)

3. **Modeling**
   - Trained multiple models:
     - LightGBM
     - XGBoost
     - CatBoost
   - Used **Optuna** for hyperparameter tuning
   - Final predictions via **stacked ensembling**

4. **Evaluation**
   - RMSE, MAE, and R² Score used
   - Final accuracy: **89.8%**, aiming for 90%+

## 📦 Libraries Used

- `pandas`, `numpy`
- `scikit-learn`
- `xgboost`, `lightgbm`, `catboost`
- `optuna` for tuning
- `matplotlib`, `seaborn` for visualization

