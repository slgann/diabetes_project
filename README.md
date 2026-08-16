# Diabetes Prediction with Machine Learning

A machine learning classification project for predicting diabetes outcomes based on clinical features.

## Project Overview

This project compares three classification models:

- Decision Tree
- Random Forest
- MLP

The workflow includes:

- Exploratory Data Analysis (EDA)
- Missing value handling using KNNImputer
- Feature scaling using StandardScaler
- Stratified 5-Fold Cross-Validation
- Hyperparameter tuning with GridSearchCV
- Model comparison and evaluation
- Saving the best model with Joblib

## Machine Learning Pipeline

```text
Data
 ↓
Data Cleaning
 ↓
Train/Test Split
 ↓
StandardScaler
 ↓
KNNImputer
 ↓
Classifier
 ↓
Cross-Validation
 ↓
GridSearchCV
 ↓
Best Model
 ↓
Test Set Evaluation
```
## Result

The best-performing model is selected based on cross-validation ROC-AUC and then evaluated on the unseen test set.

The final trained pipeline is saved as:

`best_model.joblib`