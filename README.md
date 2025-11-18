# Customer Churn Prediction 

Ecommerce Dataset :-
Source : Kaggle 
Size: 555.61 kB
Rows: 5630
Columns: 20
---
## Overview

Customer Churn Prediction is a critical machine learning use case that helps businesses identify customers who are likely to discontinue their services. By predicting churn proactively, companies can implement targeted retention strategies, reduce revenue loss, and improve customer lifetime value.

This project implements a comprehensive end-to-end machine learning pipeline for customer churn prediction, including data preprocessing, handling class imbalance, model training, evaluation, and comparison of multiple algorithms.

---

## Objective

The primary objective of this project is to:

1. **Build a robust Machine Learning prediction model** to accurately identify customers at risk of churning
2. **Implement techniques to handle imbalanced datasets** effectively
3. **Evaluate model performance** using appropriate metrics for imbalanced classification
4. **Provide performance insights** through confusion matrix and ROC curve analysis
5. **Enable data-driven business decisions** for customer retention strategies

---

## Problem Statement

**Goal**: Build a Machine Learning Prediction model to predict Customer Churn

**Key Challenges**:
- Handle **imbalanced dataset** (typical churn rate: ~30%)
- Select appropriate **evaluation metrics** for imbalanced classification
- Interpret results using **Confusion Matrix** and **ROC Curve**
- Optimize for **high recall** to minimize missed churners (false negatives)

**Success Criteria**:
- Accuracy: Target ~0.70+
- Recall: Prioritize capturing actual churners
- ROC-AUC: Aim for moderate to strong predictive power (0.70+)
- Precision & Recall: Balance based on business requirements

---

## Workflow 
1. Data Collection 
2. EDA : Exploratory Data Analysis
3. Data Preprocessing
4. Train-Test Split
5. Model Training
6. Model Evaluation
7. Deployment

---

##  Technologies Used

### Programming Language
- **Python**

### Data Manipulation & Analysis
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing

### Data Visualization
- **matplotlib** - Static visualizations
- **seaborn** - Statistical data visualization

### Machine Learning
- **scikit-learn** - ML algorithms and utilities
  - Classification algorithms
  - Preprocessing tools
  - Model evaluation metrics
  - Cross-validation
  
- **imbalanced-learn (imblearn)** - Handling imbalanced datasets
  - SMOTE (Synthetic Minority Over-sampling Technique)
  - RandomUnderSampler

- **XGBoost** - Gradient boosting framework

---


### Target Variable Distribution
- **No Churn**: 83.16 (Class Imbalance!)
- **Churn**: 16.84

---

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Analyze target variable distribution
- Visualize numerical features
- Examine categorical features
- Correlation analysis

### 2. Data Preprocessing
- Handle missing values
- Remove duplicates
- Convert data types
- Drop irrelevant features 

### 3. Feature Engineering
- **One-Hot Encoding**: Transform multi-category features
- **Feature Scaling**: StandardScaler for normalization

### 4. Train-Test Split
- **Split Ratio**: 80% training, 20% testing

### 5. Model Training
- Used xgboost

### 6. Evaluation
- **Accuracy** : 0.97
- **Decision** -0.915
- **Precision** : 0.9158
- **Recall** : 0.9158
- **F1-score** : 0.9158
- **ROC** : 0.9904
