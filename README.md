# CodeAlpha_DiseasePredictionModel
# Disease Prediction Model

Predicts the likelihood of heart disease from patient data, built for the 
CodeAlpha Machine Learning Internship (Task 4).

## Dataset
Combined UCI Heart Disease dataset (~920 patients, 4 hospital sites). 
Target built from disease severity (0 = no disease, 1 = disease present).

## Approach
- Data cleaning (handled missing values, dropped high-missing features)
- Logistic Regression, Random Forest, and SVM classifiers
- Evaluation using Precision, Recall, F1-Score, and ROC-AUC

## Results
- Random Forest performed best overall (F1 ~0.86, ROC-AUC ~0.83)
- Top predictors: cholesterol, max heart rate, age, ST depression

## Limitation
Data was missing in two clinically relevant features (`ca`, `thal`) in over 
half the rows, so they were dropped rather than imputed unreliably.

## Tech
Python, pandas, scikit-learn, matplotlib, seaborn
