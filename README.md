Diabetes Benchmarking: Uncertainty, Calibration, and Predictive Safety in Machine Learning

This repository contains the full experimental pipeline, evaluation framework, and analysis code for the paper:

"Benchmarking Predictive Performance, Calibration, and Uncertainty for Reliable Diabetes Risk Prediction from Tabular Data"

The project provides a comprehensive benchmarking study across 12 machine learning models, evaluated on two heterogeneous diabetes datasets, with a strong focus on predictive reliability, uncertainty, and safety — beyond conventional accuracy metrics.

Overview

Traditional ML studies in healthcare focus primarily on predictive accuracy. However, high accuracy does not guarantee reliable or safe predictions, especially in clinical decision-support settings.

This project systematically evaluates:

Predictive discrimination (PR-AUC, ROC-AUC)

Probability calibration and reliability

Epistemic uncertainty quality

Selective prediction safety

Conformal prediction with statistical guarantees

Comparative safety analysis across models and datasets

The goal is to understand which models are not only accurate, but trustworthy.

Key Features

Benchmarking of 12 ML models across classical, ensemble, and deep learning families

Leakage-free nested cross-validation with calibration split

Post-hoc probability calibration (Temperature Scaling, Isotonic Regression)

Epistemic uncertainty estimation for all models

Risk–coverage and selective prediction analysis

Conformal prediction with validity guarantees

High-quality scientific figures and tables for publication

Fully reproducible pipeline

Models Included
Linear & Probabilistic

Logistic Regression (ElasticNet)

Ridge Classifier

Gaussian Naïve Bayes

Ensemble Tree Models

Random Forest

Extra Trees

XGBoost

LightGBM

CatBoost

Classical Nonlinear

Support Vector Machine (RBF)

Deep Tabular Models

Multilayer Perceptron (MLP)

TabNet

FT-Transformer

Datasets
1. BRFSS 2015 Diabetes Health Indicators

Population-scale diabetes risk dataset derived from CDC BRFSS survey.

~10,000 samples (balanced subset)

21 tabular features

Demographic, lifestyle, and health indicators

Population-level risk prediction

Dataset link:
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset

Original BRFSS source:
https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system

2. Early-Stage Diabetes Risk Prediction

Small clinical dataset for symptom-based diabetes detection.

520 samples

16 features (symptoms + demographic)

Mixed categorical and binary variables

Clinical risk prediction scenario

Dataset link:
https://www.kaggle.com/datasets/ishandutta/early-stage-diabetes-risk-prediction-dataset

Evaluation Dimensions
Predictive Performance

PR-AUC (primary metric)

ROC-AUC

Accuracy, Balanced Accuracy

MCC, F1, Sensitivity, Specificity

Calibration & Reliability

Expected Calibration Error (ECE)

Brier Score

Negative Log-Likelihood (NLL)

Reliability diagrams

Epistemic Uncertainty

Epistemic AURC (EpAURC)

Risk–coverage curves

High-confidence wrong rate

Spearman correlation (uncertainty vs error)

Selective Prediction

Accuracy at fixed coverage (80%, 90%, 95%)

Safety improvement under rejection

Conformal Prediction

Coverage validity (90%, 95%)

Prediction set size

Reliability guarantees
