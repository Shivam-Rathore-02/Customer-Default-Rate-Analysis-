# Customer Default Rate Analysis

## Overview

This repository contains the code, data, and documentation for conducting a comprehensive Customer Default Rate Analysis. The goal of this project is to assess the likelihood of customers defaulting on their financial obligations, using historical data, financial indicators, and predictive modeling techniques.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Data Description](#data-description)
- [Analysis Workflow](#analysis-workflow)
- [Predictive Modeling](#predictive-modeling)
- [Visualization](#visualization)


## Project Structure

The repository is organized as follows:


## Data Description

### 1. Raw Data
The raw data is stored in the `data/raw/` directory. It includes historical customer records, financial indicators, and external economic data. The key columns in the dataset include:
- `CustomerID`: Unique identifier for each customer
- `LoanAmount`: Amount of loan taken by the customer
- `InterestRate`: Interest rate applied to the loan
- `LoanTerm`: Duration of the loan
- `PaymentHistory`: Record of past payments
- `DefaultFlag`: Indicator of whether the customer has defaulted (1) or not (0)

### 2. Processed Data
The processed data, located in the `data/processed/` directory, includes additional features generated through the feature engineering process, such as:
- `DebtToIncomeRatio`
- `CreditScore`
- `EmploymentStatus`
- `EconomicIndicators` (e.g., unemployment rate, inflation)

## Analysis Workflow

The analysis is conducted in the following steps:

1. **Data Cleaning & Processing**: 
   - Handle missing values, outliers, and erroneous entries.
   - Normalize or scale the data as needed.
   - Merge external data sources, such as economic indicators.

2. **Exploratory Data Analysis (EDA)**:
   - Analyze the distribution of key variables.
   - Identify correlations between features.
   - Visualize trends in customer defaults over time.

3. **Feature Engineering**:
   - Create new features that capture additional information.
   - Perform dimensionality reduction if necessary.

4. **Predictive Modeling**:
   - Develop and train models to predict customer default probability.
   - Compare different models such as Logistic Regression, Random Forest, and Gradient Boosting.

5. **Model Evaluation**:
   - Evaluate models using metrics like accuracy, precision, recall, F1-score, and AUC-ROC.
   - Perform cross-validation to ensure model robustness.

6. **Results Interpretation & Visualization**:
   - Interpret the model results to provide actionable insights.
   - Visualize the key findings using plots and charts.

## Predictive Modeling

The predictive models used in this analysis include:
- **Logistic Regression**: A baseline model to predict default probability based on linear relationships.
- **Random Forest**: An ensemble method that improves predictive accuracy by combining multiple decision trees.
- **Gradient Boosting Machines (GBM)**: A powerful ensemble method that builds models sequentially to correct errors of previous models.

## Visualization

The `src/visualization.py` script is used to generate various visualizations, including:
- **Default Rate Trends**: Visualizing trends in default rates over time.
- **Feature Importance**: Showing the importance of different features in predicting default.
- **ROC Curve**: Plotting the Receiver Operating Characteristic curve to assess model performance.


