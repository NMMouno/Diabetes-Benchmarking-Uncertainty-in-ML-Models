# Diabetes Benchmarking: Predictive Performance, Calibration, and Uncertainty in Machine Learning

This repository contains the complete experimental pipeline, evaluation framework, and analysis code for benchmarking machine learning models for **reliable diabetes risk prediction from tabular data**.

Unlike conventional studies focused only on predictive accuracy, this work evaluates **predictive reliability, calibration, epistemic uncertainty, and safety** across diverse model families and heterogeneous clinical datasets.

---

## Overview

High predictive accuracy does not guarantee reliable or safe predictions, especially in clinical decision-support systems. This project systematically evaluates whether machine learning models produce **trustworthy probability estimates, meaningful uncertainty signals, and statistically valid predictions**.

The framework benchmarks **12 machine learning models** across two diabetes datasets under a strict leakage-free evaluation protocol.

---

## Key Contributions

- Comprehensive benchmarking of **12 ML models**
- Evaluation beyond accuracy: **calibration, uncertainty, and predictive safety**
- Leakage-free cross-validation with independent calibration split
- Post-hoc calibration (Temperature Scaling and Isotonic Regression)
- Epistemic uncertainty estimation across all model families
- Risk–coverage and selective prediction safety analysis
- Conformal prediction with statistical reliability guarantees
- Publication-quality figures and reproducible pipeline

---

## Models Included

### Linear & Probabilistic
- Logistic Regression (ElasticNet)
- Ridge Classifier
- Gaussian Naïve Bayes

### Ensemble Tree Models
- Random Forest  
- Extra Trees  
- XGBoost  
- LightGBM  
- CatBoost  

### Classical Nonlinear
- Support Vector Machine (RBF Kernel)

### Deep Tabular Models
- Multilayer Perceptron (MLP)  
- TabNet  
- FT-Transformer  

---

## Datasets

### 1. BRFSS 2015 Diabetes Health Indicators
Population-scale diabetes risk prediction dataset derived from CDC BRFSS survey.

- ~10,000 samples (balanced subset)
- 21 tabular features
- Demographic, lifestyle, and health indicators

Dataset:
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset  

Original BRFSS:
https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system  

---

### 2. Early-Stage Diabetes Risk Prediction
Small clinical dataset for symptom-based diabetes prediction.

- 520 samples
- 16 features
- Mixed categorical and binary variables

Dataset:
https://www.kaggle.com/datasets/ishandutta/early-stage-diabetes-risk-prediction-dataset  

---

## Evaluation Dimensions

### Predictive Performance
- PR-AUC (primary)
- ROC-AUC
- Balanced Accuracy
- MCC, F1-score, Sensitivity, Specificity

### Calibration & Probability Reliability
- Expected Calibration Error (ECE)
- Brier Score
- Negative Log-Likelihood (NLL)
- Reliability diagrams

### Epistemic Uncertainty
- Epistemic AURC (EpAURC)
- Risk–coverage curves
- High-confidence incorrect rate
- Spearman correlation (uncertainty vs error)

### Selective Prediction
- Accuracy at fixed coverage (80%, 90%, 95%)
- Safety improvement via uncertainty-based rejection

### Conformal Prediction
- Coverage validity (90%, 95%)
- Prediction set size
- Formal reliability guarantees

---

## Repository Structure

# Diabetes Benchmarking: Predictive Performance, Calibration, and Uncertainty in Machine Learning

This repository contains the complete experimental pipeline, evaluation framework, and analysis code for benchmarking machine learning models for **reliable diabetes risk prediction from tabular data**.

Unlike conventional studies focused only on predictive accuracy, this work evaluates **predictive reliability, calibration, epistemic uncertainty, and safety** across diverse model families and heterogeneous clinical datasets.

---

## Overview

High predictive accuracy does not guarantee reliable or safe predictions, especially in clinical decision-support systems. This project systematically evaluates whether machine learning models produce **trustworthy probability estimates, meaningful uncertainty signals, and statistically valid predictions**.

The framework benchmarks **12 machine learning models** across two diabetes datasets under a strict leakage-free evaluation protocol.

---

## Key Contributions

- Comprehensive benchmarking of **12 ML models**
- Evaluation beyond accuracy: **calibration, uncertainty, and predictive safety**
- Leakage-free cross-validation with independent calibration split
- Post-hoc calibration (Temperature Scaling and Isotonic Regression)
- Epistemic uncertainty estimation across all model families
- Risk–coverage and selective prediction safety analysis
- Conformal prediction with statistical reliability guarantees
- Publication-quality figures and reproducible pipeline

---

## Models Included

### Linear & Probabilistic
- Logistic Regression (ElasticNet)
- Ridge Classifier
- Gaussian Naïve Bayes

### Ensemble Tree Models
- Random Forest  
- Extra Trees  
- XGBoost  
- LightGBM  
- CatBoost  

### Classical Nonlinear
- Support Vector Machine (RBF Kernel)

### Deep Tabular Models
- Multilayer Perceptron (MLP)  
- TabNet  
- FT-Transformer  

---

## Datasets

### 1. BRFSS 2015 Diabetes Health Indicators
Population-scale diabetes risk prediction dataset derived from CDC BRFSS survey.

- ~10,000 samples (balanced subset)
- 21 tabular features
- Demographic, lifestyle, and health indicators

Dataset:
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset  

Original BRFSS:
https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system  

---

### 2. Early-Stage Diabetes Risk Prediction
Small clinical dataset for symptom-based diabetes prediction.

- 520 samples
- 16 features
- Mixed categorical and binary variables

Dataset:
https://www.kaggle.com/datasets/ishandutta/early-stage-diabetes-risk-prediction-dataset  

---

## Evaluation Dimensions

### Predictive Performance
- PR-AUC (primary)
- ROC-AUC
- Balanced Accuracy
- MCC, F1-score, Sensitivity, Specificity

### Calibration & Probability Reliability
- Expected Calibration Error (ECE)
- Brier Score
- Negative Log-Likelihood (NLL)
- Reliability diagrams

### Epistemic Uncertainty
- Epistemic AURC (EpAURC)
- Risk–coverage curves
- High-confidence incorrect rate
- Spearman correlation (uncertainty vs error)

### Selective Prediction
- Accuracy at fixed coverage (80%, 90%, 95%)
- Safety improvement via uncertainty-based rejection

### Conformal Prediction
- Coverage validity (90%, 95%)
- Prediction set size
- Formal reliability guarantees

## Repository Structure

├── gpip-diabetes-uncertainty-1.ipynb
├── outputs/
│ ├── figures/
│ ├── tables/
│ ├── predictions/
│ └── metrics/
├── README.md
└── requirements.txt
