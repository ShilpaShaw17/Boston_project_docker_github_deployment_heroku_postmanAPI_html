# Boston_project_docker_github_deployment_heroku_postmanAPI_html


Overview

The Boston House Pricing Prediction project aims to predict the prices of houses in Boston using various machine learning techniques. This end-to-end project encompasses data collection, preprocessing, model training, evaluation, and deployment using Docker and GitHub Actions.

Introduction

House price prediction is a critical application of machine learning, providing valuable insights for real estate businesses and individual buyers. This project utilizes the Boston Housing dataset to build predictive models and deploy them for real-time predictions.

Project Structure

The project is organized into the following directories:

data: Contains the dataset and any data preprocessing scripts.
notebooks: Jupyter notebooks for exploratory data analysis (EDA) and model training.
src: Source code for data processing, model training, and prediction.
models: Saved machine learning models.
docker: Dockerfiles and related configurations for containerization.
.github: GitHub Actions workflows for CI/CD.

Model Training

The model training process involves:

Data preprocessing (handling missing values, feature engineering, etc.).
Splitting the data into training and testing sets.
Training various regression models (e.g., Linear Regression, Random Forest, Gradient Boosting).
Selecting the best model based on evaluation metrics.
Model Evaluation
Evaluate the performance of the trained models using metrics such as:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R-squared (R²) Score
Comparison of models and their evaluation results will be documented in the notebooks and model selection process.

Deployment

Deploy the trained model using Docker and GitHub Actions:

Build the Docker image:

bash
docker build -t boston-house-pricing 


Run the Docker container:

bash
docker run -p 5000:5000 boston-house-pricing
Access the web application at http://localhost:5000.
