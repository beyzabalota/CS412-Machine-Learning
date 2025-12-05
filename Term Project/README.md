# Bug Severity Prediction using Machine Learning - CS412 Term Project

This repository contains the source code and report for our **CS412 - Machine Learning** Term Project at **Sabancı University** (Spring 2023-2024).

## Project Overview

Our goal was to develop a machine learning model that accurately assigns severity scores to bug descriptions. We explored multiple models and feature extraction methods, ultimately choosing **XGBoost** due to its strong macro-average precision performance.

### Severity Levels:
- Enhancement
- Minor
- Normal
- Major
- Blocker
- Critical

## Methodology

- **Data Processing**: Used NLTK for lemmatization and TF-IDF for vectorization.
- **Model Selection**: Tried various algorithms, including Neural Networks, Logistic Regression, and Random Forest.
- **Final Model**: XGBoost with hyperparameter tuning via Grid Search.
- **Evaluation**: Highest macro-average precision score achieved by our final model.
- **Output**: Trained model predictions saved and submitted to Kaggle for testing.

## Key Results

- Traditional models showed competitive performance.
- XGBoost provided the best overall macro precision.
- TF-IDF proved effective in capturing essential textual features.
- Interpretability and efficiency were prioritized over deep learning.

## Team Members and Contributions

- **Berke Ayyıldızlı** – Model Application
- **Beyza Balota** – Feature Extraction
- **Kerem Tuğrul Enünlü** – Data Processing
- **Ali Eren Şahin** – Evaluation and Adjustment
- **Nur Deren Sakin** – Report Writing

## Note

This repository is for **demonstration purposes** only. The actual codebase and training artifacts are part of our private repository.

## Report

The full project report is included as [`CS412-TermProject.pdf`](./CS412-TermProject.pdf).

