# 🔬 Lung Cancer Survival Prediction: A Comprehensive Study


## Project Overview 🚀
This project is a deep dive into lung cancer survival prediction, comparing a range of statistical and machine learning models. Using the National Lung Screening Trial (NLST) dataset, we explore how various factors—from patient demographics to tumor characteristics—influence survival outcomes.

Our goal is to create robust, predictive models that can provide valuable insights for clinical decision-making. 🩺

## Key Features & Objectives 🎯

1. Survival Dynamics: Uncover the key factors driving survival rates in lung cancer patients.
2. Model Comparison: Evaluate and benchmark classic statistical models like CoxPH against modern Machine Learning (ML) and Deep Learning (DL) techniques.
3. Advanced Architectures: Implement advanced models, including Transformer-augmented DeepSurv, to capture complex, non-linear relationships in the data.
4. Ensemble Power: Develop a powerful ensemble model to combine the strengths of multiple DL models for superior predictive accuracy. 💪
5. Actionable Insights: Translate complex survival analysis into clear, practical visualizations and conclusions.

## Data at a Glance 📊
The analysis is based on a curated subset of the NLST dataset, which includes data from 2,150 lung cancer patients. This dataset is rich with features that provide a holistic view of each patient:
A. Patient Demographics: Age, gender, and smoking history.
B. Tumor Characteristics: Lesion size, clinical staging, and pathology.
C. Time-to-Event Data: Detailed information on days to diagnosis and cancer-free days.
The data was meticulously preprocessed, with techniques like median imputation for missing values and feature selection to ensure optimal model performance. ✨

## Models Implemented 🤖
This project isn't just about one model—it's a comprehensive comparison. Here’s a quick rundown of the models we built and evaluated:

## Model	Type	Key Features
1. Cox Proportional Hazards (CoxPH)	Traditional Statistics	A classic model for survival analysis.
2. Random Survival Forests (RSF)	ML (Ensemble)	Handles censored data with a tree-based approach.
3. XGBoost	ML (Gradient Boosting)	A powerful gradient boosting framework adapted for survival prediction.
4. DeepSurv	Deep Learning	A neural network extension of CoxPH that can capture non-linear relationships.
5. DeepHit	Deep Learning	Directly estimates survival distributions without proportional hazards assumptions.
6. DeepSurv Transformer	Deep Learning (Advanced)	A transformer-based architecture designed to model complex feature interactions.
7. Ensemble Model	Hybrid	Combines predictions from multiple DL models for enhanced robustness. 🤝

## Evaluation & Results ✅
To ensure a fair and thorough comparison, we used a range of industry-standard metrics to evaluate each model's performance:
1. Concordance Index (C-Index): Measures the model's ability to rank survival times correctly.
2. Integrated Brier Score (IBS): Assesses prediction accuracy over time.
3. ROC-AUC: Evaluates classification performance at specific time points.

Install the required libraries:
pip install -r requirements.txt
The requirements.txt file contains a full list of dependencies, including lifelines, scikit-survival, pytorch, numpy, pandas, matplotlib, seaborn, and scikit-learn. 🐍
