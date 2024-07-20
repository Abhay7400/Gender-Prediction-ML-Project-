# Dentistry Gender Prediction Project
## **Project Overview**

This project aims to predict gender based on dental measurements using various machine learning models. The dataset consists of dental features such as canine distances and widths. The goal is to build a model that can accurately classify the gender of individuals based on these features.

## **Data Preprocessing**

Data preprocessing is a crucial step before training the models. It involves handling missing values, encoding categorical features, and scaling numerical features. Here’s an overview of the preprocessing steps performed:

1. *Handling Missing Values:* Missing values are imputed using the median of the respective columns.
2. *Encoding Categorical Features:* The gender column is encoded using one-hot encoding to convert categorical values into numerical values.
3. *Scaling Features:* Numerical features are scaled to standardize the data, which helps in improving the model performance.
   
## Exploratory Data Analysis (EDA)
EDA is performed to understand the distribution of the data, detect outliers, and identify correlations between features.

1. *Outliers Detection:* Outliers are detected using the IQR (Interquartile Range) method. Outliers are values that fall below Q1 - 1.5IQR or above Q3 + 1.5IQR.
2. *Correlation Analysis:* Features that are highly correlated with each other are identified and dropped to reduce multicollinearity, which can negatively affect the model performance.

## Model Building

Several machine learning models are trained and evaluated for gender prediction. The models include:

1. *Linear Regression:* Although primarily used for regression tasks, it’s included for comparison.
2. *Decision Tree Classifier:* A simple, interpretable model that splits the data based on feature values.
3. *Random Forest Classifier:* An ensemble method that builds multiple decision trees and combines their predictions.
4. *XGBoost Classifier:* A powerful gradient boosting algorithm known for its high performance.

## Evaluation Metrics

The models are evaluated using various metrics to determine their performance:

1. *Confusion Matrix:* Provides a summary of prediction results on the classification problem. It shows the number of true positives (TP), true negatives (TN), false positives (FP), and false negatives (FN).
2. *Accuracy:* Measures the proportion of correctly classified instances out of the total instances.
3. *ROC Curve (Receiver Operating Characteristic Curve):* Plots the True Positive Rate (TPR) against the False Positive Rate (FPR) at different threshold settings.
4. *AUC (Area Under the ROC Curve):* Provides an aggregate measure of the model’s performance across all classification thresholds.


## Key Findings and Outcomes
ROC Curve and AUC Score: The ROC curve for the best-performing model shows a high True Positive Rate and a low False Positive Rate, indicating excellent performance. The AUC score of 0.97 indicates that the model has a very high ability to distinguish between the classes.
Confusion Matrix: The confusion matrix helps in understanding the types of errors the model is making, providing insights into its precision, recall, and overall accuracy.

## Conclusion
The project successfully builds and evaluates several models for gender prediction based on dental features. The XGBoost classifier, with an AUC score of 0.97, demonstrates the best performance, making it a reliable model for this classification task. This project provides a comprehensive approach to data preprocessing, model building, and evaluation, serving as a valuable resource for students and practitioners in the field of machine learning.
