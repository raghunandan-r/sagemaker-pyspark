# Time Series Forecasting with DeepAR and PySpark

## Project Overview
These notebooks showcases the application of AWS SageMaker's DeepAR algorithm for time series forecasting, integrated with data processing using PySpark. The Jupyter notebook (`forecasting_with_deepAR_AWS Summit22.ipynb`) covers the entire workflow from data ingestion and preprocessing, through model training, to inference and evaluation.

The second notebook (`sparkmagic-sentiment-analysis.ipynb`) covers the implementation of a simple sentiment analysis project using AWS Blazingtext model. The model was deployed on an endpoint and a real time inference of a text review was evaluated.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Usage](#usage)
- [Data Description](#data-description)
- [Methodology](#methodology)
- [Results and Discussion](#results-and-discussion)
- [Issues and Future Work](#limitations-and-future-work)
- [References](#references)

## Features
- **PySpark for Data Processing**: Utilizes Apache Spark for efficient handling of large datasets.
- **DeepAR Forecasting**: Implements DeepAR for robust time series forecasting.
- **Model Training and Evaluation**: Detailed steps for model training and performance evaluation.
- **Batch and Real-Time Inference**: Techniques for both batch processing and real-time model inference.
- **Visualization**: Includes visualization tools for comparing forecasts with actual data.

## Getting Started

### Prerequisites
- Understanding of Python, time series analysis, and machine learning.
- An AWS account with SageMaker and S3 access.
- A Spark environment for running PySpark.

### Installation
- Clone or download the Jupyter notebook from the repository. 
- Tested using `Studio SparkMagic - PySpark Kernel` running on a `ml.t3.medium` instance and connected to an EMR clsuter with an `m5.xlarge` Master node and 2 `m5.xlarge` Core nodes. Please ensure that you see PySpark (SparkMagic) in the top right on your notebook.

## Data Description
This project uses a time series dataset (e.g., electricity demand from the UCI Machine Learning Repostiory) compatible with PySpark and AWS DeepAR. We also use the `movie_reviews` sample data.


## Methodology
- **Data Wrangling**: Using PySpark for data loading, cleaning, transformation, and feature engineering.
- **Model Training**: Training the DeepAR model using AWS SageMaker.
- **Inference**: Implementing both batch and real-time inference.
- **Evaluation**: Assessing model performance with various metrics and visualizations.

## Results and Discussion
- Successful training of a model using Sagemaker Studio and PySpark.

## Limitations and Future Work
- Resource constraints to perform batch transformation in a personal account
- Future work involves, deploying an endpoint for real-time infrerence and changes for incremental processing.

## References
- [Scalable data preparation using Amazon SageMaker Studio notebooks - AWS Virtual Workshop
] (https://www.youtube.com/watch?v=UcRNNHuYsxE)
- Workshop Link: https://catalog.workshops.aws/sagemaker-studio-emr/
