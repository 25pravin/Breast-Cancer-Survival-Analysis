# Breast-Cancer-Survival-Analysis

## Overview
This project presents an end-to-end survival analysis study on breast cancer patient data using classical and parametric survival modeling techniques in Python. The objective is to identify significant prognostic factors affecting patient survival outcomes and compare multiple survival modeling approaches for clinical interpretation.

The project includes:

- Kaplan–Meier Survival Analysis
- Log-Rank Statistical Testing
- Cox Proportional Hazards (PH) Modeling
- Weibull Accelerated Failure Time (AFT) Modeling
- Proportional Hazards Assumption Diagnostics
- Survival Visualization and Interpretation

---

## Dataset Information

- Total Patients: *15,054*
- Clinical Variables: *34*
- Mortality Events Observed: *9,318*

The dataset contains demographic, tumor-related, treatment-related, and biomarker-based clinical variables associated with breast cancer survival outcomes.

---

## Objectives

- Analyze breast cancer survival outcomes using time-to-event analysis
- Identify statistically significant prognostic factors
- Evaluate proportional hazards assumptions
- Compare semi-parametric and parametric survival models
- Generate clinically interpretable survival visualizations

---

## Methodology

### 1. Data Preprocessing
- Missing value handling
- Data cleaning and feature transformation
- Survival time and event variable preparation
- Exploratory data analysis (EDA)

---

### 2. Kaplan–Meier Survival Analysis
- Estimated survival probabilities over time
- Generated Kaplan–Meier survival curves for subgroup analysis
- Conducted Log-Rank tests to compare survival distributions

---

### 3. Cox Proportional Hazards (PH) Model
Developed a multivariable Cox PH model to estimate hazard ratios and evaluate prognostic significance of clinical variables.

#### Key Findings

| Variable | Hazard Ratio (HR) | Interpretation |
|----------|-------------------|---------------|
| Tumor Size | 1.62 | Larger tumor size associated with increased mortality risk |
| HER2 Positive Status | 1.44 | HER2-positive patients exhibited higher hazard risk |

#### Model Performance
- Concordance Index (C-index): *0.66*

---

### 4. Proportional Hazards Assumption Testing
- Evaluated proportional hazards assumptions using Schoenfeld residual diagnostics
- Identified time-varying effects for selected covariates

---

### 5. Weibull Accelerated Failure Time (AFT) Model
Implemented a Weibull AFT model to improve interpretability where covariate effects changed over time.

#### Model Performance
- Akaike Information Criterion (AIC): *111166.68*

---

## Technologies Used

### Programming Language
- Python

### Libraries
- pandas
- numpy
- lifelines
- matplotlib
- seaborn
- scipy
- scikit-learn

---

## Project Structure

text
breast-cancer-survival-analysis/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── survival_analysis.ipynb
│
├── scripts/
│   ├── data_preprocessing.py
│   ├── kaplan_meier_analysis.py
│   ├── cox_ph_model.py
│   ├── weibull_aft_model.py
│   └── diagnostics.py
│
├── outputs/
│   ├── plots/
│   ├── reports/
│   └── model_results/
│
├── requirements.txt
├── README.md
└── LICENSE


---

## Key Insights

- Tumor size and HER2-positive status were identified as major prognostic indicators.
- The Cox PH model provided effective estimation of mortality risk.
- Weibull AFT modeling improved interpretation for variables violating proportional hazards assumptions.
- Kaplan–Meier analysis demonstrated clear survival differences across patient groups.

---

## Sample Outputs

### Kaplan–Meier Survival Curves
- Overall survival estimation
- Subgroup survival comparison

### Diagnostic Visualizations
- Schoenfeld residual plots
- Hazard ratio interpretation plots

### Model Outputs
- Hazard ratios
- Confidence intervals
- Statistical significance testing

---

## Installation and Setup

### Clone the Repository

bash
git clone https://github.com/25pravin/breast-cancer-survival-analysis.git


### Navigate to Project Directory

bash
cd breast-cancer-survival-analysis


### Install Required Dependencies

bash
pip install -r requirements.txt


---

## How to Run

### Run Jupyter Notebook

bash
jupyter notebook


Open:

text
notebooks/survival_analysis.ipynb


OR execute Python scripts individually from the scripts/ directory.

---

## Applications

This project demonstrates practical applications of:

- Survival Analysis
- Clinical Data Science
- Biostatistics
- Healthcare Analytics
- Oncology Research
- Predictive Modeling

---

## Future Improvements

- Implement Random Survival Forests
- Explore Deep Learning-based survival models (DeepSurv)
- Build interactive dashboards for survival prediction
- Perform external validation on independent
