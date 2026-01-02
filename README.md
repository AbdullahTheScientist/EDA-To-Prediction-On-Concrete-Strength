# 🏗️ Concrete Compressive Strength Prediction

## Overview
Concrete compressive strength is a critical indicator of structural performance in civil engineering.  
This project leverages **data-driven analysis** and **machine learning** to predict concrete strength based on mix design parameters and curing age.

The dataset includes features such as:

- Cementitious materials: `cement`, `slag`, `ash`
- Water content and superplasticizer: `water`, `superplastic`
- Aggregates: `coarseagg`, `fineagg`
- Curing age: `age`
- Engineered features: `water_cement_ratio`, `total_binder`, `aggregate_to_cement`, `cement_water_interaction`, `age_strength_proxy`

The goal is to build a **robust, interpretable, and accurate predictive model** aligned with civil engineering principles.

---
---

## 📊 Exploratory Data Analysis (EDA)
The EDA includes:

- **Univariate Analysis**: Histograms and box plots for numeric features to detect distributions and outliers
- **Bivariate Analysis**: Scatter plots of key features vs `strength`
- **Correlation & Multicollinearity**: Pearson correlation matrix and Variance Inflation Factor (VIF) analysis
- **Feature Engineering Validation**: Engineered features such as `water_cement_ratio` and `cement_water_interaction` validated with correlation and visual analysis
- **Age-Based Analysis**: Grouping strength by curing age bins
- **Water–Cement Ratio Bucketing**: Optimal ranges for strength determined from data

---

## 🤖 Machine Learning Models

The project compares multiple regression models:

   Model        
 Linear Regression\
 Random Forest    
 XGBoost Regressor

> Random Forest and XGBoost outperform Linear Regression due to non-linear interactions in concrete mix data.

**Feature Importance:**  
Random Forest highlights key predictors such as `total_binder`, `cement`, `water_cement_ratio`, and `age`.

---

## 🔧 Dependencies
- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
- statsmodels
- scipy

