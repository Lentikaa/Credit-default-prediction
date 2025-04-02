# Credit-default-prediction
# Introduction
This project develops a robust credit card default prediction system for Bank A to assess and manage credit risk within their existing customer portfolio. The system implements a sophisticated behavior scoring model that predicts the probability of customer defaults
# Project Overview
Uses supervised learning techniques to classify customers as likely to default or not.

Includes data preprocessing, exploratory data analysis (EDA), and model building.

Implements models like Logistic Regression, Random Forest, and XGBoost.

Evaluates model performance using accuracy, precision, recall, and F1-score.
# Dataset
The dataset contains features such as income, age, credit balance, and previous payment history.

Missing values are handled, and categorical variables are encoded.
# Explanatory Data Analysis
Distribution of target classes (default vs. non-default).

Correlation analysis to identify important features.

Feature scaling and selection.
# Technologies Used
Python

Pandas, NumPy (Data Handling)

Matplotlib, Seaborn (Data Visualization)

Scikit-learn (Machine Learning Models)

XGBoost (Advanced Model)
# Model Performance
Evaluates classification reports and confusion matrices.

Uses AUC-ROC to compare models.

Applies SMOTE to handle class imbalance.
# Conclusion
Based on the model evaluation results:

Best Performing Model: Random Forest achieved the highest AUC (0.801), followed by XGBoost (0.780) and Logistic Regression (0.760).

Model Performance Analysis:

Random Forest has best overall performance but struggles with defaulter prediction (recall=0.00 for class 1)
Logistic Regression shows balanced performance for defaulter detection (precision=0.04, recall=0.61)
XGBoost provides a good compromise with moderate defaulter detection (precision=0.05, recall=0.36)


Final Recommendation: Despite having slightly lower overall AUC, XGBoost would be the recommended model for deployment because:

Provides balanced performance across both classes
Shows reasonable defaulter detection capability
Maintains high accuracy for non-defaulters



The system successfully identifies credit risk patterns while balancing between false positives and false negatives in default prediction.
