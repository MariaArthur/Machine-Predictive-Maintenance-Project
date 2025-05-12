# Machine Predictive Maintenance Classification

## Overview
This project aims to predict machine failures in industrial environments using sensor data. The process includes data preprocessing, statistical analysis, model building, and evaluation. The goal is to explore the relationships between sensor readings and failure types and to optimize maintenance scheduling to reduce downtime.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Data Preprocessing & Cleaning](#data-preprocessing--cleaning)
4. [Analysis & Insights](#analysis--insights)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Findings](#findings)
8. [Limitations & Assumptions](#limitations--assumptions)
9. [Recommendations](#recommendations)
10. [Conclusion](#conclusion)
11. [References](#references)

## Introduction
In this project, we use machine learning and data science techniques to predict potential machine failures. By analyzing historical sensor data, we aim to uncover patterns that will help optimize maintenance schedules and reduce operational downtime in industrial settings.

### Problem Statement
Inaccurate or unexpected machinery breakdowns can cause costly downtime and reduce productivity. Traditional time-based maintenance methods are inefficient and costly. This project aims to use a data-driven approach to predict failures and improve maintenance decision-making.

### Objectives
- Apply the data science process to explore machine sensor data.
- Investigate how machine features like temperature and tool wear relate to failure events.
- Build a model for failure prediction and optimize maintenance strategies.

## Dataset
The dataset used in this project is the **Machine Predictive Maintenance Classification** dataset from Kaggle. It contains 10,000+ instances and includes attributes related to machine conditions and failure types. Key features include:
- **Product ID**: Identifies the machine
- **UDI**: Unique Device Identifier (UDI) for each machine
- **Type**: Machine type (L, M, H)
- **Air temperature [K]**
- **Process temperature [K]**
- **Rotational speed [rpm]**
- **Torque [Nm]**
- **Tool wear [min]**
- **Target**: Binary classification (1 = failure, 0 = no failure)
- **Failure Type**: Type of failure (e.g., Heat Dissipation, Overstrain)

## Data Preprocessing & Cleaning
The dataset was cleaned and preprocessed to handle missing values, outliers, and categorical variables. Key preprocessing steps include:
- Handling missing values and duplicates
- Identifying and handling outliers
- Encoding categorical variables (e.g., `Product ID`, `Type`, `Failure Type`)
- Feature scaling and normalization

## Analysis & Insights
Exploratory Data Analysis (EDA) was conducted to uncover relationships between features and failure occurrences. Key insights include:
- The frequency of failure types and their distribution
- The impact of tool wear on failure likelihood
- The relationship between temperature, torque, and failures

## Modeling
We built several machine learning models to predict machine failures, including:
- **Logistic Regression** for failure prediction based on tool wear.
- **Random Forest**, **Support Vector Machine (SVM)**, and **XGBoost** to assess predictive accuracy.

## Evaluation
Model evaluation was performed using accuracy, confusion matrix, and other performance metrics. The effectiveness of each model in predicting failures was compared to determine the most reliable approach.

## Findings
- Tool wear increases the likelihood of machine failure, with a specific threshold indicating elevated risk.
- Certain failure types are more prevalent, providing insights into critical failure modes.
- Machine learning models can effectively predict failures based on real-time sensor data.

## Limitations & Assumptions
- The dataset may not cover all potential failure modes, limiting generalizability.
- Sensor data quality and external factors like machine environment were not considered.

## Recommendations
- **Optimal Maintenance Thresholds**: Intervene when tool wear exceeds 90% to balance cost and downtime.
- Use predictive maintenance models to schedule maintenance more efficiently and avoid unexpected breakdowns.

## Conclusion
This project successfully demonstrates the potential of predictive maintenance using data science techniques. The insights and models developed can help optimize maintenance schedules and reduce operational downtime in industrial settings.

## References
- Alsheibani, A., et al. (2020). "Machine Learning for Predictive Maintenance in Manufacturing." Journal of Industrial Engineering.

- Kaggle Dataset: [Machine Predictive Maintenance Classification](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification)
