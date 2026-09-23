# Customer Churn Analysis and Prediction

## 📌 Project Overview

Customer churn is an important business problem where organizations aim to understand why customers leave their services and identify customers who may be likely to churn.

This project, **Customer Churn Analysis and Prediction Using Data Analytics and Machine Learning**, combines Exploratory Data Analysis (EDA), statistical analysis, data visualization, data preprocessing, machine learning, model evaluation, cross-validation, hyperparameter tuning, and customer churn prediction.

The project analyzes customer demographics, services, contracts, billing information, usage behavior, support interactions, satisfaction levels, and churn status to identify patterns associated with customer churn.

---

## 🎯 Main Objective

The main objective of this project is to:

- Analyze customer churn patterns using data analytics.
- Explore demographic, service, contract, billing, and customer-experience variables.
- Identify important factors associated with customer churn.
- Prepare customer data for machine learning.
- Develop multiple classification models.
- Compare machine learning model performance.
- Perform cross-validation.
- Tune the Random Forest model using GridSearchCV.
- Identify important features influencing churn prediction.
- Generate customer churn predictions and churn probabilities.

---

## 📊 Dataset

The project uses an Excel-based customer dataset containing:

- **20,000 customer records**
- **31 columns**
- **Target variable:** `Churn`
- **Numerical features:** 9
- **Categorical features:** 20

The dataset contains information related to:

- Customer demographics
- Age
- Income
- Tenure
- Contract type
- Internet service
- Online security
- Online backup
- Device protection
- Technical support
- Streaming services
- Monthly charges
- Total charges
- Monthly usage
- Support tickets
- Late payments
- Satisfaction score
- City tier
- Referral
- Customer churn status

The dataset is loaded from the Excel sheet:

`raw_data`

---

## 🔍 Project Workflow

The project follows an end-to-end Data Analytics and Machine Learning workflow.

### 1. Data Loading

The Excel dataset is loaded into a Pandas DataFrame for further analysis.

### 2. Initial Dataset Overview

The dataset structure, dimensions, column names, data types, and sample records are examined.

### 3. Statistical Analysis

Descriptive statistics are generated to understand the numerical variables and their distributions.

### 4. Data Quality Analysis

The project checks:

- Missing values
- Duplicate records
- Duplicate customer IDs
- Numerical data quality
- Potential data anomalies

No missing values or duplicate records were identified. A potential anomaly was observed in `TotalCharges`, where a negative value appears in the dataset.

### 5. Categorical Variable Analysis

Categorical variables are analyzed to understand customer distribution and their relationship with churn.

Important variables include:

- Gender
- Marital Status
- Dependents
- Education
- Employment Status
- Internet Service
- Contract
- Payment Method
- City Tier
- Referral

### 6. Numerical Variable Analysis

Numerical variables are analyzed using statistical summaries and visualizations.

Important numerical variables include:

- Age
- Income
- TenureMonths
- MonthlyCharges
- TotalCharges
- AvgMonthlyUsageGB
- NumSupportTickets
- LatePayments
- SatisfactionScore

### 7. Exploratory Data Analysis

EDA is performed to investigate customer churn patterns using:

- Churn distribution
- Age analysis
- Gender analysis
- Contract analysis
- Monthly charges analysis
- Tenure analysis
- Satisfaction score analysis
- Support ticket analysis
- Internet service analysis
- Payment method analysis
- Tenure vs Monthly Charges
- Correlation analysis

---

## 🤖 Machine Learning Preparation

The target variable `Churn` is converted into binary form:

```text
No  → 0
Yes → 1
