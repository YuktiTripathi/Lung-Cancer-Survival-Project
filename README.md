# Lung-Cancer-Survival-Project

Lung Cancer Survival Prediction

Project Overview

This repository contains a comprehensive project focused on survival prediction for lung cancer patients using statistical, machine learning (ML), and deep learning (DL) approaches. The study utilizes the National Lung Screening Trial (NLST) dataset to compare the performance of various models, including Cox Proportional Hazards (CoxPH), Random Survival Forests (RSF), XGBoost, DeepSurv, DeepHit, and a Transformer-augmented DeepSurv architecture. An ensemble model combining DL outputs is also explored to enhance predictive accuracy.

The project aims to:

Investigate survival dynamics in lung cancer patients.

Identify significant clinical, demographic, and tumor-related factors influencing survival outcomes.

Compare traditional statistical models with ML and DL techniques for predictive performance.

Provide actionable insights for clinical decision-making through robust survival analysis and visualizations.

Dataset

The analysis is based on a curated subset of the NLST dataset, comprising clinical and survival data for 2,150 lung cancer patients. Key features include:


Patient demographics (age, gender, smoking history)
Tumor characteristics (lesion size, clinical staging, pathology)
Time-to-event variables (days to diagnosis, cancer-free days)
Screening and outcome data

The dataset was preprocessed to handle missing values, normalize features, and perform feature selection to optimize model performance.

Models Implemented

The following models were developed and evaluated

Cox Proportional Hazards (CoxPH): A traditional statistical model for survival analysis.

Random Survival Forests (RSF): A tree-based ensemble method for handling censored data.

XGBoost: A gradient boosting framework adapted for survival prediction.

DeepSurv: A neural network extension of CoxPH for modeling non-linear relationships.

DeepHit: A DL model that directly estimates survival distributions without proportional hazards assumptions.

DeepSurv Transformer: A transformer-based architecture for capturing complex feature interactions.

Ensemble Model: Combines predictions from DeepSurv, DeepHit, DeepSurv Transformer, and SurvNet for improved robustness.

Methodology

Data Preprocessing: Handled missing values using median imputation, normalized features, and conducted correlation analysis for feature selection.

Exploratory Data Analysis (EDA): Generated Kaplan-Meier survival curves, correlation heatmaps, and pairwise scatterplots to explore data distributions and relationships.

Model Training: Models were trained on 80% of the data, with 20% reserved for testing. Hyperparameters were tuned for optimal performance.

Evaluation Metrics:
Concordance Index (C-Index): Measures discriminatory power (ability to rank survival times).
Brier Score and Integrated Brier Score (IBS): Assesses calibration and prediction accuracy over time.
ROC-AUC: Evaluates classification performance at specific time points.

Requirements

Python 3.8+
Libraries: lifelines, scikit-survival, pytorch, numpy, pandas, matplotlib, seaborn, scikit-learn


