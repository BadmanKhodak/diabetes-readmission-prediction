# Diabetes 30-Day Hospital Readmission Prediction

## Project Overview

This project develops and evaluates machine learning models for predicting 30-day hospital readmission among diabetic patients.

The study uses the Diabetes 130-US Hospitals dataset and applies data preprocessing, feature extraction, feature selection, classification, and model optimization to develop a predictive model for hospital readmission.

## Objectives

The main objectives of the project are to:

- Preprocess and prepare the diabetes hospital dataset for machine learning.
- Extract and select relevant features for predicting hospital readmission.
- Develop and compare multiple machine learning classification models.
- Evaluate the models using appropriate classification performance metrics.
- Optimize the best-performing model to improve prediction of 30-day readmission.

## Machine Learning Models

The following models were developed and evaluated:

1. Balanced Logistic Regression
2. Decision Tree
3. Random Forest
4. Linear Support Vector Machine (SVM)
5. XGBoost
6. Optimized XGBoost

## Selected Features

The final model was developed using 20 selected features:

- num_lab_procedures
- num_medications
- time_in_hospital
- diag_3
- diag_2
- age
- diag_1
- number_inpatient
- num_procedures
- discharge_disposition_id
- number_diagnoses
- admission_type_id
- insulin
- admission_source_id
- race
- number_outpatient
- gender
- number_emergency
- glipizide
- metformin

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Particular attention was given to recall because the dataset contains an imbalanced target variable and the identification of patients at risk of readmission is an important objective of the study.

## Final Model

The Optimized XGBoost model achieved the highest ROC-AUC and recall among the evaluated models.

Performance of the Optimized XGBoost model:

- Accuracy: 63.97%
- Precision: 17.86%
- Recall: 61.96%
- F1-score: 27.73%
- ROC-AUC: 68.19%

The Optimized XGBoost model was therefore selected as the final prediction model.

## Repository Contents

- `Readmission_Prediction.ipynb` – Jupyter Notebook containing the complete data preprocessing, feature extraction, model development, evaluation, and optimization workflow.

## Dataset

The project uses the Diabetes 130-US Hospitals dataset. The dataset is not included in this repository.

The notebook expects the dataset file to be available locally before execution.

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

## Project Purpose

This repository accompanies an academic research project investigating the application of machine learning to the prediction of 30-day hospital readmission among diabetic patients.
