# Healthcare Readmissions Prediction Project

## Business Objective

The goal of this project is to develop a predictive model for hospital readmissions. Healthcare readmissions occur when a patient is readmitted to a hospital within a specified period (typically 30 days) after discharge. This metric is a key indicator of hospital quality and continuity of patient care. High readmission rates may signal problems with initial treatment, discharge planning, or post-discharge follow-up. Reducing readmissions is crucial, as frequent readmissions are costly and can result in financial penalties for hospitals, especially under regulations like the US Affordable Care Act.

## Exploratory Data Analysis Report

- The EDA report provides a comprehensive overview of the dataset, including:
  - Data distributions and summary statistics
  - Correlation analysis
  - Feature engineering insights
  - Identification of missing values and outliers

  *Resources: [eda_report.ipynb](eda_report/eda_report.ipynb), [eda_report.pdf](eda_report/eda_report.pdf)*

## Data Preparation Plan

- The data preparation plan outlines the steps for cleaning and transforming the raw data, including:
  - Imputation of missing values
  - Feature engineering (e.g., BMI categories, age groups)
  - One-hot encoding of categorical variables
  - Removal of redundant or non-predictive features

  *Resources: [data_preparation_plan.pdf](data_prep_pipeline/data_preparation_plan.pdf)*

## Model Pipelines

- Deployed training and testing pipelines on Google Cloud:
  - [Training Pipeline](data_prep_pipeline/training_pipeline.ipynb): Loads and preprocesses data, splits into train/validation sets, normalizes features, applies SMOTE for class balancing, trains a logistic regression model, and evaluates performance.
  - [Testing Pipeline](data_prep_pipeline/testing_pipeline.ipynb): Preprocesses and normalizes test data, applies the trained model, and generates predictions.
  
  *Resources: [gcp_data_pipeline.pdf](data_prep_pipeline/gcp_data_pipeline.pdf)*

## Summary Discussion

- The project demonstrates an end-to-end approach for predicting hospital readmissions using structured patient data.
- The EDA and data preparation steps ensure high-quality inputs for modeling.
- The pipeline design supports reproducibility and scalability, leveraging cloud infrastructure for deployment.
- Predictive modeling of readmissions can help hospitals identify at-risk patients, improve care continuity, and reduce costs associated with frequent.