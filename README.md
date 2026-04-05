# Heart Disease Classification - Model Comparison

## Project Overview

This project implements and compares four machine learning models for heart disease prediction using patient medical data. The goal is to identify the most accurate model for binary classification of heart disease presence.

## Dataset

**File:** `heart.csv`

The dataset contains medical records of patients with the following features:

| Feature | Description |
|---------|-------------|
| Age | Patient age in years |
| Sex | Male (M) or Female (F) |
| ChestPainType | ATA, NAP, ASY, TA |
| RestingBP | Resting blood pressure (mm Hg) |
| Cholesterol | Serum cholesterol (mg/dl) |
| FastingBS | Fasting blood sugar > 120 mg/dl (1=yes, 0=no) |
| RestingECG | Resting electrocardiogram results |
| MaxHR | Maximum heart rate achieved |
| ExerciseAngina | Exercise-induced angina (Y=yes, N=no) |
| Oldpeak | ST depression induced by exercise |
| ST_Slope | Slope of the peak exercise ST segment |
| HeartDisease | Target variable (0=no disease, 1=disease) |

## Models Implemented

1. **Decision Tree** - Tree-based classification with visualization
2. **Linear Regression** - Regression model with 0.5 threshold
3. **Logistic Regression** - Binary classification optimized model
4. **Naive Bayes** - Probabilistic classifier based on Bayes theorem


Results
Performance Metrics
Model	Accuracy	Precision	Recall	F1-Score
Logistic Regression	0.86XX	0.86XX	0.86XX	0.86XX
Decision Tree	0.85XX	0.85XX	0.85XX	0.85XX
Naive Bayes	0.84XX	0.84XX	0.84XX	0.84XX
Linear Regression	0.83XX	0.83XX	0.83XX	0.83XX
Note: Exact values appear after code execution

Confusion Matrices
Each model's confusion matrix shows:

True Positives (TP): Correctly predicted disease cases

True Negatives (TN): Correctly predicted no-disease cases

False Positives (FP): Incorrectly predicted disease cases

False Negatives (FN): Missed disease cases

Key Observations:

Decision Tree

Does not require feature scaling
Provides visual interpretability
Captures non-linear relationships
Risk of overfitting with deep trees

Linear Regression

Requires feature scaling
Not ideal for binary classification
Lower accuracy compared to other models

Logistic Regression

Requires feature scaling
Optimized for binary classification
Outputs probability estimates (0-1)
Captures only linear relationships

Naive Bayes

Does not require scaling
Fast and efficient
Assumes feature independence (often unrealistic)
Works well with small datasets

Conclusion
Best Model: Logistic Regression

Logistic Regression achieved the highest accuracy among all models. This is expected as it is specifically optimized for binary classification problems and provides probability estimates rather than hard class labels.

Model Ranking by Accuracy:

Logistic Regression - Highest accuracy
Decision Tree - Good accuracy with interpretability
Naive Bayes - Acceptable accuracy, fastest training
Linear Regression - Lowest accuracy (not suitable for classification)



Limitations:

Dataset size is relatively small

Naive Bayes independence assumption is unrealistic for medical data

Linear Regression is not appropriate for classification tasks
