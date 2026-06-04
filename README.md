# spamemailml
A comparative study of classical ML classifiers for spam vs. ham email classification using structured features.

Overview: 

This project trains and evaluates five machine learning models on a structured spam email dataset. Rather than raw text, it uses engineered features like word count, link count, and sender reputation to classify emails as spam or ham.

Models Trained: 

-Logistic Regression

-Decision Tree

-K-Nearest Neighbors (KNN)

-Random Forest

-Naive Bayes (Multinomial)

Evaluation Metrics: 

1. Classification Metrics:
   
Accuracy, Precision, Recall, F1-Score,
ROC-AUC, Log Loss,
Matthews Correlation Coefficient (MCC),
Balanced Accuracy, Specificity, FPR, FNR

2. Calibration / Regression Metrics (on predicted probabilities):
   
MSE, RMSE, MAE, Brier Score

3. Visualizations:
   
ROC Curves (all models overlaid),
Confusion Matrices (heatmaps),
Feature Importance (Random Forest),
Model Metric Comparison Bar Chart

Key Insights:

-Random Forest typically yields the highest accuracy and ROC-AUC due to ensemble averaging.

-sender_reputation_score and contains_money_terms are the most important features per RF feature importance.

-Naive Bayes is fastest to train but may underperform on numeric features compared to text-native use cases.

