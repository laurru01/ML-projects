# Customer Churn Analysis

## Project Description
This project focuses on analyzing customer churn to predict which customers are likely to leave a service or product. It uses machine learning algorithms to identify patterns in customer behavior and factors leading to churn. The project involves data preprocessing, exploratory data analysis, feature engineering, model selection, improvement, and deployment. Key Python libraries used include Pandas, NumPy, Scikit-Learn, XGBoost, Optuna, and Flair.

## Table of Contents
- [1. Project Initiation](#1-project-initiation)
  - [1.1 Restart the Session](#11-restart-the-session)
  - [1.2 Import Libraries](#12-import-libraries)
- [2. Data Preprocessing](#2-data-preprocessing)
  - [2.1 Import Data](#21-import-data)
  - [2.2 Exploratory Data Analysis](#22-exploratory-data-analysis)
  - [2.3 Missing Data](#23-missing-data)
  - [2.4 Outlier Detection](#24-outlier-detection)
  - [2.5 Categorical Features](#25-categorical-features)
    - [2.5.1 Identify Unique Values](#251-identify-unique-values)
    - [2.5.2 One-Hot Encoding](#252-one-hot-encoding)
  - [2.6 Feature Engineering](#26-feature-engineering)
    - [2.6.1 Sentiment Analysis on 'Feedback'](#261-sentiment-analysis-on-feedback)
  - [2.7 Feature Selection](#27-feature-selection)
    - [2.7.1 Multicollinearity](#271-multicollinearity)
    - [2.7.2 Sklearn SelectKBest](#272-sklearn-selectkbest)
    - [2.7.3 Random Forest Importance](#273-random-forest-importance)
  - [2.8 Feature Scaling](#28-feature-scaling)
- [3. Model Selection](#3-model-selection)
  - [3.1 Initial Considerations](#31-initial-considerations)
  - [3.2 Metric Selection](#32-metric-selection)
  - [3.3 Baseline Classification Algorithms Comparison](#33-baseline-classification-algorithms-comparison)
- [4. Model Improvement](#4-model-improvement)
  - [4.1 Optuna Hyperparameter Optimization](#41-optuna-hyperparameter-optimization)
- [5. Model Deployment](#5-model-deployment)

## 1. Project Initiation

### 1.1 Restart the Session
Code snippet to clear all temporary variables before starting coding.

### 1.2 Import Libraries
Import of necessary Python libraries for data analysis and machine learning.

## 2. Data Preprocessing
The data preprocessing phase involves cleaning the data, handling missing values, encoding categorical features, and feature scaling.

### 2.1 Import Data
Data is imported for analysis using Pandas.

### 2.2 Exploratory Data Analysis
Exploratory analysis to understand the data and its features.

### 2.3 Missing Data
Missing data is handled through imputation or removal.

### 2.4 Outlier Detection
Outliers are detected and handled to improve model accuracy.

### 2.5 Categorical Features
Categorical features are encoded using one-hot encoding.

### 2.6 Feature Engineering
Feature engineering includes sentiment analysis on the 'Feedback' column using the Flair library.

### 2.7 Feature Selection
Feature selection methods like multicollinearity analysis, SelectKBest, and random forest importance are used to select relevant features.

### 2.8 Feature Scaling
Feature scaling is performed to standardize the range of independent variables.

## 3. Model Selection

### 3.1 Initial Considerations
The problem is approached as a classification task.

### 3.2 Metric Selection
Metrics such as ROC AUC, accuracy, precision, recall, and F1 score are used for model evaluation.

### 3.3 Baseline Classification Algorithms Comparison
Various classification algorithms like Logistic Regression, SVC, KNN, Decision Tree, Random Forest, and XGBoost are compared based on their performance metrics.

## 4. Model Improvement

### 4.1 Optuna Hyperparameter Optimization
Optuna is used for hyperparameter optimization of the selected model (XGBoost) to improve its performance.

## 5. Model Deployment
The final model is deployed using the joblib library for future predictions on new customer data.

```python
filename = 'final_model.model'
joblib.dump(final_model, filename)
