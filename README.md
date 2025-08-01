# Housing Price Predictor | Kaggle Competition

This project is a submission for the [Kaggle House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) competition. The goal is to predict the final price of homes in Ames, Iowa, using machine learning models trained on various house features such as square footage, neighborhood, condition, and more.

## 📌 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Tech Stack](#tech-stack)


## 🧠 Overview
The dataset includes 79 features describing almost every aspect of a residential home. The task is to predict the **SalePrice** of each home using regression-based models. My model was in the **top 4%** of submissions.

This project focuses on:
- Data preprocessing
- Careful Feature engineering
- Experimenting with different ML models
- Hyperparameter tuning for improved accuracy

## 📊 Dataset
- **Train set**: 1,460 entries
- **Test set**: 1,459 entries
- Source: [Kaggle competition page](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)

## 🔍 Exploratory Data Analysis
Conducted EDA to:
- Identify missing values and data imbalances
- Detect skewed or categorical features

## 🧰 Feature Engineering
- Imputed missing values with group-wise medians/modes
- Converted categorical features using one-hot encoding and ordinal encoding

## 🤖 Modeling

Tested the following models:
- Decision Tree Regressor
- Random Forest
- XGBoost

### 🔧 Tuning
Used `GridSearchCV` and cross-validation (RMSE as scoring metric) to tune hyperparameters.

---

## 📈 Results

| Model          | Public Score (MAE) |
|----------------|--------------------|
| Decision Tree  | 21,217.96          |
| Random Forest  | 16,619.08          |
| XGBoost        | 14,376.90          |


## 🛠 Tech Stack

- Python 3.10
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-Learn
- XGBoost, RandomForestRegressor, DecisionTreeRegressor
- Jupyter Notebook
