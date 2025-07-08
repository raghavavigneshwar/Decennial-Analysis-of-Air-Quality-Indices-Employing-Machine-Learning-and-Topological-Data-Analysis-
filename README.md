# Air Quality Index (AQI) Forecasting and COVID-19 Impact Analysis Using Time Series Models and Topological Data Analysis

This repository contains two distinct projects focusing on Air Quality Index (AQI) analysis and prediction:

1. **AQI Time Series Forecasting and Clustering with TDA**
2. **AQI Analysis Using Azure Machine Learning**


# Project 1: AQI Forecasting and Clustering Using Time Series Models and Topological Data Analysis (TDA)

This project focuses on forecasting and analyzing **Air Quality Index (AQI)** data using advanced **time series models** along with clustering techniques enhanced by **Topological Data Analysis (TDA)**. The goal is to accurately predict AQI trends, identify pollution patterns, and uncover hidden structures within the data to support **environmental decision-making**.

---

## 📌 Project Overview

The primary objective of this project is to forecast AQI levels across major Indian cities using **ARIMA, SARIMA, Facebook Prophet, and NeuralProphet**, while applying **TDA-based clustering** to reveal deeper insights and patterns in the air quality data.

---

## 🚀 Key Features

- 📊 **Time Series Forecasting**: Implementation of multiple time series models to predict future AQI trends.
- 🔍 **Topological Data Analysis (TDA) for Clustering**: Applied TDA to cluster AQI data and identify complex patterns beyond traditional methods.
- 📈 **Model Evaluation**: Comprehensive evaluation of forecast accuracy and clustering effectiveness.

---

## 🔗 Technologies Used

- **Python**
- **ARIMA, SARIMA (Statsmodels)**
- **Facebook Prophet, NeuralProphet**
- **Scikit-learn**
- **Topological Data Analysis (TDA)**
- **Pandas, Matplotlib, Seaborn**

---

## 🛠 Project Workflow

1. **Data Preparation**  
   AQI data from multiple Indian cities is collected, cleaned, and transformed for analysis.

2. **Time Series Forecasting**  
   Forecasting AQI using **ARIMA, SARIMA, Facebook Prophet, and NeuralProphet** to capture trends, seasonality, and anomalies.

3. **Clustering with TDA**  
   Applying **Topological Data Analysis (TDA)** techniques for clustering and pattern recognition in AQI data.

---

## 📊 Model Performance (Best Model: Facebook Prophet)

| Metric | Train  | Test  |
|--------|--------|-------|
| MAE    | 12.10  | 9.72  |
| MSE    | 244.85 | 189.48 |
| RMSE   | 15.65  | 13.77 |

---

## 🌍 COVID-19 Lockdown Impact Analysis

Analyzed the impact of the **COVID-19 lockdown (March–May 2020)** on air quality across cities:

| City       | Lockdown AQI (2020) | Avg AQI (Other Years) | AQI Reduction (%) |
|-----------|---------------------|-----------------------|-------------------|
| Delhi     | 127.41              | 198.16                | 35.7%             |
| Mumbai    | 75.08               | 108.35                | 30.7%             |
| Hyderabad | 72.17               | 94.49                 | 23.6%             |
| Chennai   | 56.25               | 69.14                 | 18.6%             |
| Kolkata   | 78.99               | 95.40                 | 17.2%             |
| Ahmedabad | 125.13              | 139.41                | 10.2%             |

---

## 📌 Conclusion

- The **Facebook Prophet** model delivered the most accurate AQI forecasts with lower error metrics.
- The use of **Topological Data Analysis (TDA)** enhanced the clustering process by uncovering hidden patterns and structures in the data.
- The project demonstrates the effectiveness of combining **time series forecasting** and **unsupervised clustering** for meaningful **environmental analysis and risk assessment**.
  
# Project 2: AQI Analysis Using Azure Machine Learning

This project focuses on analyzing Air Quality Index (AQI) data using Azure Machine Learning (Azure ML) to build an end-to-end machine learning pipeline. It includes data preprocessing, model training, evaluation, and deployment using the capabilities of Azure ML. The project leverages custom Python scripts, components, and pipelines to automate the entire machine learning workflow.

## Project Overview

The primary goal of this project is to analyze AQI data and predict air quality levels using various machine learning models. The project utilizes Azure Machine Learning services to streamline and automate the workflow, from data ingestion to model deployment.

Key Features:
- Modular and reusable components for data processing and model training.
- Custom Python scripts for each step of the pipeline.
- Automation of the entire ML lifecycle using Azure ML pipelines.
- Flexibility to handle large datasets and scalable execution on cloud resources.

## Project Structure

The project consists of the following key components:

### 1. **Python Scripts**
The core of the project is built around several Python scripts that perform specific tasks, such as data loading, feature engineering, model training, and evaluation. Each script is parameterized, allowing flexibility and reusability across different datasets and configurations.

### 2. **JSON Files**
A `config.json` file stores essential configuration details, such as the Azure subscription ID, resource group, and workspace name. This ensures seamless integration with the Azure ML workspace and avoids hardcoding sensitive information into scripts.

### 3. **Components in Azure ML**
In Azure ML, components are modular, reusable building blocks that represent specific steps in the machine learning workflow. Each component (implemented as Python scripts or executables) performs a self-contained task, such as data preprocessing or model training. These components have defined input/output interfaces, which makes them versatile and easily combinable in various pipelines.

### 4. **Azure ML Pipeline**
The pipeline orchestrates the sequence of tasks necessary to complete the AQI analysis. It automates the ML workflow by linking components such as data transformation, model training, and evaluation. Azure ML pipelines ensure scalability, parallelism, and efficient resource usage by executing different tasks on appropriate compute resources.

## Prerequisites

Before running the project, make sure you have the following:
- An Azure subscription and Azure Machine Learning workspace set up.
- Python 3.8+ and the required dependencies (listed in `environment.yml`).
- Access to the AQI dataset.

## Project Workflow

1. **Data Preprocessing**: AQI data is preprocessed to clean missing values, engineer features, and normalize the data.
2. **Model Training**: Multiple machine learning models, such as XGBoost, Random Forest, and Logistic Regression, are trained using a custom component.
3. **Model Evaluation**: Each model is evaluated based on metrics such as accuracy, precision, recall, and F1-score.

## Results

The XG Boost model achieved the best performance with an f1 score of 88% on the test dataset. The model was selected for deployment based on its business suitability and predictive power.

## Conclusion

This project demonstrates the power of Azure Machine Learning in building scalable and reusable machine learning workflows. By leveraging the modularity of components and pipelines, this project automates the AQI analysis and prediction workflow, providing accurate insights into air quality levels.


---
