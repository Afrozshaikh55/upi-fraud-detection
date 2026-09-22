UPI Fraud Detection Using Machine Learning

Project Overview

This project uses machine learning to classify UPI transactions as legitimate or fraudulent based on transaction and customer-related features.

Dataset

The project uses the upi_fraud_dataset.csv dataset.

Target Variable

fraud_risk — 0 = Legitimate, 1 = Fraud

Features Used

Transaction hour

Transaction day

Transaction month

Age

Transaction amount

Transaction category

State

The dataset is used for training and evaluating classification models for UPI fraud detection.

Project Workflow

Import Libraries

Load Dataset

Data Understanding

Data Cleaning

Exploratory Data Analysis (EDA)

Feature and Target Separation

Train-Test Split

Data Preprocessing

Logistic Regression

Random Forest

Random Forest Cross-Validation

Random Forest Feature Importance

XGBoost

Model Comparison

XGBoost Hyperparameter Tuning

Final Model Comparison

Final Model Evaluation

Data Cleaning

The dataset was checked for:

Missing values

Duplicate rows

Potential outliers in transaction amount

Exploratory Data Analysis

The analysis includes:

Fraud vs. legitimate transaction distribution

Transaction amount analysis

Fraud rate by transaction hour

Fraud rate by transaction category

Preprocessing

Numerical features are standardized using StandardScaler.

Categorical features are encoded using OneHotEncoder.

A ColumnTransformer is used to apply the appropriate preprocessing to each feature type.

Machine Learning Models

The following classification models were trained and evaluated:

Logistic Regression

Random Forest Classifier

XGBoost Classifier

XGBoost was also tuned using RandomizedSearchCV.

Model Evaluation

The models are evaluated using:

Accuracy

Precision

Recall

F1 Score

ROC-AUC

Confusion Matrix

The notebook also compares the models using these evaluation metrics.

Technologies Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

XGBoost

Jupyter Notebook

How to Run

Clone or download this repository.

Install the required libraries:

pip install -r requirements.txt

Place upi_fraud_dataset.csv in the same directory as the notebook.

Open UPI_Fraud_Detection.ipynb in Jupyter Notebook or JupyterLab.

Run the cells in order.

Project Structure

upi-fraud-detection/
│
├── UPI_Fraud_Detection.ipynb
├── upi_fraud_dataset.csv
├── README.md
└── requirements.txt
