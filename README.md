# Insurance-Claim-Prediction-Project
This project builds a predictive model to estimate the probability that a building will have at least one insurance claim during its insured period, using building characteristics. It includes data cleaning, exploratory analysis, multiple machine learning models, and performance evaluation to support insurance risk assessment.

# Project Objective

The primary aim of this project is to predict the probability that a building will have at least one insurance claim during the insured period. The target variable is Claim, where Claim = 1 indicates at least one claim occurred, and Claim = 0 indicates no claim occurred.

# Dataset Description

The project uses the Train_data.csv dataset, which contains 7,160 rows and 14 columns. Additional feature definitions are provided in Variable Description.csv.

# Key Insights

Class Imbalance: The dataset is imbalanced, with approximately 77% no claims and 23% claims, highlighting the need for metrics beyond accuracy (e.g., ROC-AUC, Precision, Recall).
Feature Observations: Initial EDA suggested relationships between claims and features like Building_Painted (fewer claims), Building_Fenced (less risky), Residential status, and Building Dimension (higher claim variability).

# Evaluation Summary

Models were evaluated using ROC-AUC, Precision, Recall, and F1-score on the test set:

##1. Logistic Regression: ROC-AUC: 0.687, Precision (Class 1): 0.59, Recall (Class 1): 0.15

##2. Random Forest: ROC-AUC: 0.688, Precision (Class 1): 0.60, Recall (Class 1): 0.21

##3. Gradient Boosting: ROC-AUC: 0.694, Precision (Class 1): 0.60, Recall (Class 1): 0.21

Conclusion: The Gradient Boosting model achieved the highest ROC-AUC, making it the most suitable model for identifying risky buildings.

# How to Run the Notebook

Open in Google Colab: Upload the notebook to Google Colab.

Ensure Data is Available: Make sure Train_data.csv is accessible, preferably in the /content/ directory as used in the notebook.

Run Cells Sequentially: Execute all cells in the notebook from top to bottom. This will import necessary libraries, load and preprocess data, perform EDA, train models, and evaluate their performance.
