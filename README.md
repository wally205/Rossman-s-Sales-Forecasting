# Rossmann Sales Forecasting

## Overview
This project focuses on **forecasting daily sales** for Rossmann retail stores using Machine Learning models. The goal is to build an accurate regression pipeline that captures the effects of time, promotions, store characteristics, and competition.

## Dataset
The Rossmann Store Sales dataset contains historical sales data from **1,115 stores**, including:
- Sales (target variable)
- Store type and assortment
- Promotions and holidays
- Competition distance
- Time-related features

## Methodology
An end-to-end **Machine Learning pipeline** was implemented:
- Data preprocessing and missing value handling  
- Feature engineering (time features, lag features, rolling statistics)  
- Encoding categorical variables  
- Training and comparing multiple regression models  

## Models Evaluated
- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- XGBoost  
- CatBoost  
- LightGBM  

## Model Performance

| Model              | MAE    | RMSPE  | Training Time (s) |
|--------------------|--------|--------|------------------|
| Linear Regression  | 0.1549 | 0.0254 | 1.99             |
| Ridge Regression   | 0.1549 | 0.0253 | 0.92             |
| Lasso Regression   | 0.1553 | 0.0253 | **0.16**         |
| XGBoost            | 0.1137 | 0.0185 | 85.50            |
| CatBoost           | 0.1143 | 0.0183 | 62.57            |
| **LightGBM**       | **0.1114** | **0.0180** | 58.58 |

**Best model:** **LightGBM**, achieving the lowest MAE and RMSPE with competitive training time.

## Tools
- Python, Pandas, NumPy  
- Scikit-learn  
- LightGBM, XGBoost, CatBoost  

## Reference
- [Rossmann Store Sales – Kaggle](https://www.kaggle.com/c/rossmann-store-sales)
