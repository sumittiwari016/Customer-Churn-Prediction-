Customer Churn Prediction

About The Project

This project aims to predict customer churn for a telecommunications company. By analyzing customer data, we build and evaluate several classification models to identify customers who are likely to discontinue their service. The goal is to provide insights that can help the company develop strategies to retain customers.

The project notebook (Customer_Churn_Prediction.ipynb) walks through the complete machine learning pipeline, from data preparation to model evaluation.


Project Pipeline The analysis follows these key steps:


Data Loading & Inspection: The dataset is loaded, and its structure and initial values are examined.

Data Cleaning & Preprocessing: This involves handling missing values (like in TotalCharges), removing irrelevant columns (customerID), and converting categorical features into a numerical format suitable for machine learning models using LabelEncoder.

Exploratory Data Analysis (EDA): Visualizations like count plots and a correlation heatmap are used to understand the distribution of features and their relationships with customer churn.

Model Preparation: The data is split into features (X) and a target (y). The features are then scaled using StandardScaler to ensure all variables contribute equally to model performance. Finally, the data is divided into training (70%) and testing (30%) sets.

Model Training & Evaluation: Several classification algorithms are trained on the data, and their performance is evaluated using metrics like Accuracy, ROC AUC Score, and a detailed Classification Report.

About the Dataset The dataset used is churn_data.csv, which contains information about the company's customers. Each row represents a unique customer.

Key Columns in the Dataset: customerID: A unique identifier for each customer.

gender: The customer's gender (Male/Female).

SeniorCitizen: Whether the customer is a senior citizen (1, 0).

Partner, Dependents: Whether the customer has a partner or dependents (Yes, No).

tenure: The number of months the customer has been with the company.

PhoneService, MultipleLines: Information about the customer's phone service.

InternetService, OnlineSecurity, OnlineBackup, etc.: Details about internet and related services.

Contract: The customer's contract term (Month-to-month, One year, Two year).

PaymentMethod: The customer's payment method.

MonthlyCharges, TotalCharges: The amount charged to the customer monthly and in total.

Churn: The target variable, indicating whether the customer churned (Yes, No).



Models Used The following classification models were trained and evaluated to predict customer churn:

Logistic Regression

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Decision Tree

Random Forest

AdaBoost

Gradient Boosting

XGBoost
