# Week 03 Progress Report

## Project

Predicting Remaining Useful Life (RUL) of Turbofan Engines

## Duration

Week 03

---

## Objectives

The objective of this week was to begin machine learning model development using the NASA C-MAPSS FD001 dataset and evaluate baseline models for Remaining Useful Life prediction.

---

## Activities Completed

### 1. Data Preparation

* Prepared features and target variables.
* Selected operational settings and sensor measurements as model inputs.
* Defined Remaining Useful Life (RUL) as the target variable.
* Performed train-test splitting for model evaluation.

### 2. Linear Regression Model

Implemented Linear Regression as the baseline model.

Performance:

* MAE: 34.05
* RMSE: 44.34
* R² Score: 0.57

### 3. Random Forest Regressor

Implemented Random Forest Regressor to capture non-linear degradation patterns.

Performance:

* MAE: 29.69
* RMSE: 41.52
* R² Score: 0.62

### 4. Feature Importance Analysis

Performed feature importance analysis using the Random Forest model.

Top predictive features identified:

1. Sensor 11
2. Sensor 9
3. Sensor 4
4. Sensor 12
5. Sensor 7

### 5. Model Evaluation

* Compared Linear Regression and Random Forest performance.
* Generated Actual vs Predicted RUL visualization.
* Analyzed model prediction behavior.
* Identified important degradation indicators.

---

## Key Findings

* Random Forest outperformed Linear Regression across all evaluation metrics.
* Sensor 11 emerged as the most influential feature.
* Sensor measurements provide valuable information for RUL prediction.
* Prediction accuracy improves as engines approach failure.

---

## Challenges Faced

* Understanding model behavior across different RUL ranges.
* Interpreting feature importance results.
* Evaluating model performance using multiple regression metrics.

---

## Learning Outcomes

During Week 03, I learned:

* Regression model development.
* Linear Regression implementation.
* Random Forest Regression implementation.
* Model evaluation using MAE, RMSE, and R².
* Feature importance analysis.
* Predictive maintenance modeling techniques.

---

## Planned Activities for Week 04

* Hyperparameter tuning.
* Feature selection.
* XGBoost implementation.
* Model optimization.
* Final model comparison.
* Project documentation and report preparation.

---

## Status

Week 03 successfully completed.

Baseline machine learning models have been developed and evaluated. The project is now ready for model optimization and performance improvement.
