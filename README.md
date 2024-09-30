# AQI Analysis Using Azure Machine Learning

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
