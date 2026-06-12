# Turbofan Engine Remaining Useful Life (RUL) Prediction

## Organization

**Uniconvergence Technology (UCT)**

This project is being developed as part of the Machine Learning Internship Program at Uniconvergence Technology (UCT). UCT works in areas such as IoT, AI/ML, Smart Cities, Digital Transformation, Industrial Automation, and Predictive Analytics. The objective is to apply machine learning techniques to solve industrial predictive maintenance problems using real-world sensor data.

---

# Project Background

In modern industrial environments, equipment failures can result in significant operational losses, safety risks, and maintenance expenses. Traditional maintenance strategies often rely on fixed schedules or reactive repairs after failure occurs.

Predictive Maintenance aims to overcome these limitations by monitoring equipment health and estimating the remaining operational life of machines before failures occur.

Turbofan engines generate large volumes of sensor and operational data during their lifecycle. By analyzing these measurements, machine learning models can estimate the Remaining Useful Life (RUL) of an engine and help organizations schedule maintenance proactively.

---

# Problem Statement

The objective of this project is to predict the number of operational cycles remaining before a turbofan engine fails.

Using operational settings and sensor measurements collected from engines throughout their lifecycle, the model must estimate the Remaining Useful Life (RUL) for each engine.

The project uses the NASA C-MAPSS dataset, a widely used benchmark dataset for predictive maintenance research.

---

# Problem Relevance

Predictive Maintenance has become a critical application of Artificial Intelligence and Machine Learning across various industries.

### Applications

* Aerospace Industry
* Manufacturing Plants
* Industrial Automation
* Smart Factories
* Transportation Systems
* Energy Sector

### Benefits

* Reduced downtime
* Lower maintenance costs
* Increased equipment reliability
* Improved operational efficiency
* Better maintenance scheduling
* Enhanced safety

---

# Dataset Description

### Dataset

NASA C-MAPSS Turbofan Engine Dataset

### Dataset Used

FD001

### Dataset Characteristics

* 100 Training Engines
* 100 Testing Engines
* 1 Operating Condition
* 1 Fault Mode
* 3 Operational Settings
* 21 Sensor Measurements

### Target Variable

Remaining Useful Life (RUL)

```text
RUL = Maximum Engine Cycle - Current Cycle
```

---

# Project Objectives

* Understand engine degradation behavior.
* Analyze operational settings and sensor measurements.
* Generate Remaining Useful Life labels.
* Perform exploratory data analysis.
* Develop machine learning models for RUL prediction.
* Evaluate model performance using regression metrics.
* Compare different prediction approaches.

---

# Project Methodology

## Phase 1: Data Understanding

* Dataset exploration
* Data quality assessment
* Missing value analysis
* Statistical summary generation

## Phase 2: Data Preprocessing

* RUL label generation
* Data cleaning
* Dataset preparation

## Phase 3: Exploratory Data Analysis

* Engine lifecycle analysis
* Correlation analysis
* Sensor trend analysis
* Degradation pattern identification

## Phase 4: Model Development

Models evaluated:

* Linear Regression
* Random Forest Regressor

Models planned:

* XGBoost Regressor
* Gradient Boosting Regressor

Advanced models (optional):

* LSTM
* GRU

## Phase 5: Evaluation

Performance Metrics:

* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* R² Score

---

# Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook
* Git & GitHub

---

# Workflow

1. Load Dataset
2. Explore Dataset
3. Generate RUL Labels
4. Perform Exploratory Data Analysis
5. Train Baseline Models
6. Evaluate Performance
7. Analyze Feature Importance
8. Compare Models
9. Generate Insights

---

# Project Structure

```text
TURBOFAN-RUL-PREDICTION/

├── data/
│   ├── train_FD001.txt
│   ├── test_FD001.txt
│   └── RUL_FD001.txt
│
├── notebooks/
│   ├── 01_EDA_FD001.ipynb
│   └── 02_Model_Training.ipynb
│
├── images/
│   ├── engine_life_distribution.png
│   ├── rul_distribution.png
│   ├── correlation_heatmap.png
│   ├── feature_importance.png
│   └── actual_vs_predicted.png
│
├── reports/
│   ├── Week-01-Progress.md
│   ├── Week-02-Progress.md
│   ├── Week-03-Progress.md
│   └── Final_Report.pdf
│
├── README.md
└── requirements.txt
```

---

# Current Progress

## Week 01

### Project Familiarization

* Studied project objectives and internship deliverables.
* Understood Predictive Maintenance concepts.
* Learned about Remaining Useful Life (RUL) estimation.
* Explored industrial applications of predictive maintenance.

### Dataset Understanding

* Downloaded and explored the NASA C-MAPSS FD001 dataset.
* Studied dataset structure and feature descriptions.
* Examined operational settings and sensor measurements.
* Reviewed training and testing dataset formats.

### Environment Setup

* Configured development environment.
* Installed required libraries.
* Created project repository structure.

---

## Week 02

### Exploratory Data Analysis (EDA)

* Performed dataset inspection and statistical analysis.
* Conducted missing value analysis.
* Investigated engine lifecycle characteristics.
* Generated engine lifetime distribution plots.
* Generated Remaining Useful Life labels.
* Analyzed RUL distribution.
* Performed correlation analysis using heatmaps.
* Investigated sensor degradation patterns.
* Studied feature relationships.

### Key Visualizations

* Engine Lifetime Distribution
* RUL Distribution
* Correlation Heatmap
* Sensor Trend Analysis

---

## Week 03

### Baseline Model Development

#### Linear Regression

Performance:

* MAE: 34.05
* RMSE: 44.34
* R² Score: 0.57

#### Random Forest Regressor

Performance:

* MAE: 29.69
* RMSE: 41.52
* R² Score: 0.62

### Feature Importance Analysis

Top Predictive Features:

1. Sensor 11
2. Sensor 9
3. Sensor 4
4. Sensor 12
5. Sensor 7

### Model Evaluation

* Compared Linear Regression and Random Forest models.
* Generated Actual vs Predicted RUL visualization.
* Performed feature importance analysis.
* Identified critical sensors related to engine degradation.

---

## Upcoming Work (Week 04)

* Hyperparameter tuning
* Feature selection
* XGBoost implementation
* Model optimization
* Error reduction
* Final model comparison
* Project documentation
* Final report preparation

---

# Results

## Exploratory Data Analysis

Completed analyses include:

* Dataset structure analysis
* Statistical summary analysis
* Missing value assessment
* Engine lifecycle distribution analysis
* RUL generation and distribution analysis
* Correlation heatmap analysis
* Sensor trend analysis
* Feature variability assessment

## Model Results

| Model                   | RMSE    | MAE     | R² Score |
| ----------------------- | ------- | ------- | -------- |
| Linear Regression       | 44.34   | 34.05   | 0.57     |
| Random Forest Regressor | 41.52   | 29.69   | 0.62     |
| XGBoost Regressor       | Planned | Planned | Planned  |

---

## Key Findings

* Random Forest outperformed Linear Regression across all evaluation metrics.
* Sensor 11 emerged as the most influential predictor.
* Sensor measurements contain significant information related to engine degradation.
* The model predicts low-RUL engines more accurately than high-RUL engines.
* The baseline model successfully captures overall degradation trends.

---

## Best Model

### Random Forest Regressor

Performance:

* MAE: 29.69 cycles
* RMSE: 41.52 cycles
* R² Score: 0.62

---

# Key Learnings

Through this project, I learned:

* Predictive Maintenance concepts
* Remaining Useful Life (RUL) estimation
* Industrial sensor data analysis
* Exploratory Data Analysis (EDA)
* Correlation analysis and visualization
* Linear Regression modeling
* Random Forest Regression
* Model evaluation using MAE, RMSE, and R²
* Feature importance analysis
* Machine Learning workflow for industrial applications

---

# Future Improvements

* Perform hyperparameter tuning.
* Apply feature selection using importance scores.
* Train on FD002, FD003, and FD004 datasets.
* Implement XGBoost Regressor.
* Explore deep learning approaches (LSTM/GRU).
* Deploy the model using Streamlit or Flask.
* Build an interactive predictive maintenance dashboard.

---

# Author

**Kushagra Pandey**

Machine Learning Intern

**Uniconvergence Technology (UCT)**
