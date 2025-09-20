# Flight Price Prediction Project

## Overview

This project demonstrates a complete **machine learning workflow** to predict **flight prices** based on various features such as **airline**, **class**, **duration**, **departure time**, **source city**, and **destination city**. The goal is to predict the price of flights using a **Random Forest Regressor** model.

The notebook covers:
- Exploratory Data Analysis (EDA)
- Data preprocessing and feature engineering
- Model training using **Random Forest Regressor**
- Hyperparameter tuning using **RandomizedSearchCV**
- Model evaluation (R², MAE, MSE, RMSE)
- Feature importance analysis
- Visualization of prediction results

---

## Dataset

The dataset used in this project is sourced from **Kaggle**: [Flight Price Prediction Dataset](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction). It contains:
- **Flights data** with multiple features such as:
  - Airline
  - Source city
  - Destination city
  - Class (Business/Economy)
  - Duration
  - Stops (number of stops)
  - Departure time
  - Arrival time
  - Price (target variable)

The dataset is used to predict the **flight price** based on these features.

---

## Project Structure

- `flight_price_prediction.ipynb` — Jupyter notebook containing the full workflow of data exploration, model training, and evaluation.
- `README.md` — Project overview and instructions.

---

## Requirements

- Python 3.x
- Jupyter Notebook
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - scipy

---

## Notes

- The notebook demonstrates data preprocessing steps, including **One-Hot Encoding**, **Factorization**, and **Binary Transformation** of features.
- The **Random Forest Regressor** is used to train the model, and **RandomizedSearchCV** is applied for **hyperparameter tuning**.
- The model's performance is evaluated using various metrics: **R²**, **MAE**, **MSE**, and **RMSE**.
- Feature importance is analyzed to understand which factors (like **class** and **duration**) most affect the flight price.
- **Scatter plots** are used to visualize the model's predictions vs. actual prices.

---

## Results

- The **Random Forest Regressor** achieves a very high **R² score** (~98.5%), indicating the model explains the vast majority of the variance in flight prices.
- The **MAE** (Mean Absolute Error) is **$1070.86**, suggesting that, on average, the model's predictions are off by **$1070.86**.
- The **MSE** and **RMSE** are also relatively high, indicating that some larger errors exist in predictions.
- The model demonstrates **high accuracy**, with feature importance analysis showing that **class** (Business vs. Economy) plays the most significant role in predicting flight prices.

---
