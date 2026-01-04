# Predicting Emergency Readmission of Discharged Heart Failure Patients

**1st SIT Coursework 02 - Autumn Semester 2025 - Milestone 1**

| Field | Details |
|-------|---------|
| **Student ID** | 23050386 |
| **Name** | Prashanna Sthapit |
| **Module** | CU6051NI - Artificial Intelligence |

## Project Overview

This project implements a comparative analysis of three machine learning models to predict emergency department readmission within 6 months for discharged heart failure patients:

1. **Logistic Regression** - Linear baseline model
2. **Random Forest** - Ensemble tree-based model (Bagging)
3. **XGBoost** - Gradient boosting algorithm

## Repository Structure

```
├── 23050386 Prashanna Sthapit.ipynb   # Main Jupyter notebook
├── README.md                           # Project documentation
└── dataset/
    ├── dat.csv                         # Main dataset
    ├── dat_md.csv                      # Metadata
    ├── dataDictionary.csv              # Data dictionary
    ├── LICENSE.txt                     # Dataset license
    └── SHA256SUMS.txt                  # Checksums
```

## Key Features

- **Meaningful Null Handling**: Null values are treated as informative (e.g., test not performed) rather than missing data
- **Class Imbalance Handling**: Uses balanced class weights and scale_pos_weight
- **Comprehensive Evaluation**: Accuracy, Precision, Recall, F1-Score, AUC-ROC, and 5-fold Cross-Validation
- **Visual Comparisons**: ROC curves, confusion matrices, and feature importance plots

## Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
```

## Usage

1. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn xgboost`
2. Open and run the Jupyter notebook: `23050386 Prashanna Sthapit.ipynb`

## Target Variable

`return.to.emergency.department.within.6.months` - Binary classification (0: No return, 1: Returned)