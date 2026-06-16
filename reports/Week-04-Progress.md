# Week 04 Progress Report

## Project

Predicting Remaining Useful Life (RUL) of Turbofan Engines

## Duration

Week 04

---

## Objectives

The objective of Week 04 was to improve model performance, experiment with advanced machine learning algorithms, compare model results, and select the final model for Remaining Useful Life prediction.

---

## Activities Completed

### 1. Random Forest Optimization

The Random Forest model developed during Week 03 was further optimized by experimenting with different hyperparameters and feature subsets.

Parameters Tested:

```python
RandomForestRegressor(
    n_estimators=500,
    max_depth=20,
    min_samples_split=5,
    min_samples_leaf=2,
    random_state=42
)
```

---

### 2. Feature Selection

Based on feature importance analysis from Week 03, the most influential sensors were selected:

* Sensor 11
* Sensor 9
* Sensor 4
* Sensor 12
* Sensor 7
* Sensor 14
* Sensor 21
* Sensor 15
* Sensor 3
* Sensor 2

The model was retrained using only these high-importance features.

#### Results

| Metric   | Value |
| -------- | ----- |
| MAE      | 29.58 |
| RMSE     | 41.42 |
| R² Score | 0.625 |

#### Observations

* Slight improvement was achieved.
* Important sensors retained most predictive information.
* Feature reduction simplified the model without degrading performance.

---

### 3. XGBoost Regressor Implementation

An XGBoost Regressor was implemented and evaluated.

```python
from xgboost import XGBRegressor
```

#### Results

| Metric   | Value |
| -------- | ----- |
| MAE      | 53.90 |
| RMSE     | 65.61 |
| R² Score | 0.058 |

#### Observations

* Performance was significantly lower than Random Forest.
* The model struggled to capture degradation behavior effectively.
* Random Forest remained the superior approach for this dataset.

---

### 4. Model Comparison

| Model                   | MAE   | RMSE  | R² Score |
| ----------------------- | ----- | ----- | -------- |
| Linear Regression       | 34.05 | 44.34 | 0.57     |
| Random Forest           | 29.69 | 41.52 | 0.62     |
| Optimized Random Forest | 29.58 | 41.42 | 0.625    |
| XGBoost Regressor       | 53.90 | 65.61 | 0.058    |

---

## Final Model Selection

### Selected Model

**Random Forest Regressor**

#### Performance

| Metric   | Value |
| -------- | ----- |
| MAE      | 29.69 |
| RMSE     | 41.52 |
| R² Score | 0.62  |

#### Reasons for Selection

* Best overall performance.
* Lowest prediction error.
* Highest R² Score among evaluated models.
* Stable and interpretable predictions.
* Effective feature importance analysis.

---

## Key Findings

* Sensor measurements contain useful degradation information.
* Sensor 11 remained the strongest predictor of Remaining Useful Life.
* Feature selection produced minor performance improvements.
* Random Forest consistently outperformed alternative models.
* XGBoost did not improve performance on the FD001 dataset.

---

## Challenges Faced

* Improving prediction accuracy beyond the baseline model.
* Selecting the most informative sensors.
* Evaluating advanced machine learning models.
* Balancing model complexity and performance.

---

## Learning Outcomes

During Week 04, I learned:

* Hyperparameter tuning techniques.
* Feature selection strategies.
* Advanced ensemble learning methods.
* XGBoost implementation.
* Model comparison and selection.
* Performance optimization techniques.

---

## Project Status

Week 04 successfully completed.

The final predictive maintenance model has been selected and evaluated. Random Forest Regressor achieved the best performance and was chosen as the final model for Remaining Useful Life prediction.

The project is now ready for final documentation and report preparation.
