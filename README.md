# Healthcare-Predictive-Analytics
Predictive analytics platform for diabetes risk classification using Scikit-learn Pipelines and XGBoost. Features automated data preprocessing for large-scale datasets (236k+ records), handling imbalanced classes, and model evaluation.

# Project Overview
This project aims to classify the risk of diabetes based on health indicators from a large-scale survey dataset. It explores the entire machine learning lifecycle, from data engineering and preprocessing of an imbalanced dataset to model evaluation and hyperparameter tuning.

The core of this project is a robust data pipeline designed to handle real-world, noisy, and skewed data, providing a reliable classification for three groups: non-diabetic, pre-diabetic, and diabetic patients.

# Dataset
Source: Kaggle - Diabetes Health Indicators Dataset
Scale: 236,378 records (responses).
Target Variable (diabetes_012):
0: No diabetes / Only during pregnancy
1: Pre-diabetes
2: Diabetes
Features: 21 health-related indicators (High Blood Pressure, High Cholesterol, BMI, Physical Activity, etc.).

# Engineering & Methodology
To ensure professional-grade code and reproducibility, the project implements:
Data Cleaning: Handling missing values and ensuring correct data types for categorical variables.
Handling Imbalanced Data: Addressing the significant class imbalance inherent in healthcare surveys.
Feature Engineering: Scaling numerical features and encoding categorical data within a unified pipeline.
Scikit-learn Pipelines: Using Pipeline objects to prevent data leakage during cross-validation and to ensure that preprocessing steps are strictly applied to training folds.

# Modeling & Results
The project evaluated several architectures, focusing on ensemble methods for their robustness:
Primary Model: Random Forest Classifier / XGBoost.
Validation Strategy: 5-Fold Cross-Validation.
Performance: Achieved an Accuracy of ~84% on the test set.
Key Insight: Feature importance analysis revealed that High Blood Pressure, BMI, and Age are the most significant predictors of diabetic status in this population.

# Tech Stack
Language: Python 3.x
Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn.
Environment: Jupyter Notebook / Google Colab.

# How to Run
1. Clone the repository: git clone https://github.com/YOUR_USERNAME/Healthcare-Predictive-Analytics.git
2. Install dependencies: pip install -r requirements.txt
3. Open the notebook: jupyter notebook Klasyfikacja wskaźników zdrowotnych - Diabetes Indicators.ipynb
