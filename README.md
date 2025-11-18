# Customer Churn Prediction - Machine Learning Use Case

---
## Live Demo : (streamlit) 

## Overview

Customer Churn Prediction is a critical machine learning use case that helps businesses identify customers who are likely to discontinue their services. By predicting churn proactively, companies can implement targeted retention strategies, reduce revenue loss, and improve customer lifetime value.

This project implements a comprehensive end-to-end machine learning pipeline for customer churn prediction, including data preprocessing, handling class imbalance, model training, evaluation, and comparison of multiple algorithms.

---

## Objective

The primary objective of this project is to:

1. **Build a robust Machine Learning prediction model** to accurately identify customers at risk of churning
2. **Implement techniques to handle imbalanced datasets** effectively
3. **Evaluate model performance** using appropriate metrics for imbalanced classification
4. **Provide actionable insights** through confusion matrix and ROC curve analysis
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
Gather raw data from available sources.
2. Handle Missing Values
Identify and impute/remove missing data.
3. Remove Duplicates
Detect and eliminate duplicate records.
4. Data Type Conversion
Convert incorrect data types to appropriate formats.
5. Distribution Analysis
Study distribution of each feature (histograms, KDE plots, etc.).
6. Correlation Analysis
Check relationships between features and target.
7. Data Visualization
Create plots for better understanding (bar charts, heatmaps, etc.).
8. Encode Categorical Variables
Convert non-numeric features using label encoding or one-hot encoding.
9. Feature Scaling
Normalize or standardize numerical columns.
10. Feature Selection
Identify and retain only the most important features.
11. Handle Imbalanced Data Using SMOTE
Oversample the minority class using SMOTE.
12. Random Under-sampling
Reduce majority class instances if needed.
13. Apply Class Weights
Give higher weight to minority class during model training.
14. Train Logistic Regression Model,Decision Tree Model, Random Forest Model, Gradient Boosting Model, XGBoost Model
15. Confusion Matrix Evaluation
Analyze TP, TN, FP, FN.
16. ROC Curve Evaluation + Precision, Recall, F1 + ROC-AUC Score
17. Model Deployment

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

## Dataset Description

### Source
- **File**: `customer_churn_data_imbalanced.csv`



### Target Variable Distribution
- **No Churn**: ~70% (Class Imbalance!)
- **Churn**: ~30%

---

## Methodology

### 1. Data Preprocessing
- Handle missing values
- Remove duplicates
- Convert data types (especially `TotalCharges`)
- Drop irrelevant features (`customerID`)

### 2. Exploratory Data Analysis (EDA)
- Analyze target variable distribution
- Visualize numerical features
- Examine categorical features
- Correlation analysis

### 3. Feature Engineering
- **Binary Encoding**: Convert Yes/No to 1/0
- **One-Hot Encoding**: Transform multi-category features
- **Feature Scaling**: StandardScaler for normalization

### 4. Train-Test Split
- **Split Ratio**: 80% training, 20% testing

### 5. Model Training
We will Train and compare multiple algorithms:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost
- Support Vector Machine (SVM)
- Naive Bayes

---

### Feature Engineering
- [ ] Interaction features (e.g., tenure × contract type)
- [ ] Temporal features (seasonality, trends)
- [ ] Customer behavior patterns
- [ ] Text mining from customer feedback


### 5. Advanced Analytics
- [ ] Customer segmentation
- [ ] Survival analysis
- [ ] Cohort analysis
- [ ] Churn reason classification
- [ ] Customer lifetime value prediction

---

