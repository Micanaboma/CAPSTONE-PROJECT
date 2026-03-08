# CAPSTONE-PROJECT


Customer Churn Prediction (Telco Dataset)

Project Overview

Customer churn prediction is a critical task for companies that rely on subscription-based services. Retaining existing customers is often more cost-effective than acquiring new ones, making churn analysis an important area of business analytics.

This project applies "supervised machine learning techniques" to predict whether a telecom customer is likely to churn based on demographic information, service usage, and account-related features.

The objective is to identify patterns associated with customer churn and build a predictive model capable of identifying customers at risk of leaving the service.


Dataset

The dataset used in this project is the "Telco Customer Churn dataset", which contains information about customers of a telecommunications company.

Features in the Dataset

The dataset includes several types of variables:

Customer Demographics

Gender
Senior Citizen status
Partner
Dependents
Service Information

Phone service
Internet service
Online security
Online backup
Device protection
Streaming TV
Streaming movies
Account Information

Contract type
Payment method
Monthly charges
Total charges
Tenure
Target Variable

Churn

Yes → Customer left the company

No → Customer stayed

Project Workflow

The project follows a structured "machine learning workflow".

Data Preparation and Cleaning

Initial preprocessing steps included:

Loading the dataset using Pandas
Inspecting data structure and data types
Handling missing or inconsistent values
Preparing features for modeling
Exploratory Data Analysis (EDA)

Exploratory data analysis was performed to understand patterns within the dataset.

Univariate Analysis (Numeric Variables)

Numeric variables such as:

Tenure
Monthly Charges
Total Charges
were analyzed to understand their distributions.

Visualization techniques included:

Histograms
Distribution plots
Univariate Analysis (Categorical Variables)

Categorical variables such as:

Gender
Contract Type
Payment Method
Internet Service
were analyzed using "count plots" to observe the frequency distribution of each category.

These analyses helped identify potential relationships between customer characteristics and churn behavior.

Feature Engineering and Preprocessing

To prepare the dataset for machine learning, preprocessing techniques were applied:

Column Transformer

A "ColumnTransformer" was used to apply different transformations to numeric and categorical features.

Scaling

Numeric features were scaled using "StandardScaler" to normalize feature ranges.

Encoding

Categorical variables were converted into numerical form using "One-Hot Encoding".

Model Development

A "Logistic Regression classifier" was used as the baseline model.

The model was implemented using a Scikit-learn Pipeline, which combines preprocessing and model training into a single workflow.

Pipeline Components

Data preprocessing
Feature scaling and encoding
Logistic Regression model
Using pipelines improves reproducibility and ensures consistent preprocessing during training and evaluation.

Model Evaluation

The dataset was split into "training and testing sets" using train_test_split.

The model's performance was evaluated using standard classification metrics:

Accuracy – Overall correctness of the model
Precision – Correct positive predictions
Recall – Ability to detect churn cases
F1 Score – Balance between precision and recall
Confusion Matrix – Detailed classification results
These metrics provide insight into the model's ability to correctly identify customers likely to churn.

Key Insights

Exploratory analysis and modeling revealed that several factors influence churn behavior, including:

Customer tenure
Monthly charges
Contract type
Payment method
Internet service features
Understanding these relationships allows businesses to design targeted customer retention strategies.

Technologies Used

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook / Google Colab


Customer-Churn-Prediction
│
├── DATASET
├── PROJECT
├── README.md
