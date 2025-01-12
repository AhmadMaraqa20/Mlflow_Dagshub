# ML Model Development and Offline Evaluation


## Overview
This project involves building a machine learning model to classify mushrooms as edible or poisonous based on their features. The project utilizes the Mushroom Classification dataset and leverages MLflow for experiment tracking, model comparison, and offline evaluation.

## Dataset
The dataset used in this project is sourced from Kaggle: Mushroom Classification. It is a cleaned version of the original UCI Mushroom Dataset and includes 9 columns describing physical attributes of mushrooms for classification.

## Project Workflow

1. Data Loading
   - The cleaned dataset was loaded directly without requiring additional preprocessing.
   - The data was split into training and testing sets to ensure reliable evaluation.

2. Model Development
   - Several machine learning algorithms were tested, including:
      1-Random Forest.
      2-Logistic Regression.
      3-K-Nearest Neighbors (KNN).
      4-Decision Tree.

3. Experiment Tracking with MLflow:
   - MLflow was used to track experiments, including:
     - Parameters.
     - Metrics (e.g., accuracy, precision, recall, F1 score).
     - Artifacts (e.g., model files).
   - Both local MLflow and DagsHub were employed for tracking and managing experiments.

5. Offline Evaluation
   - The final model was evaluated using offline evaluation techniques.
   - Metrics from the test set were compared across models to identify the best-performing one.

6. Model Selection
   - After comparing all models, the Random Forest model was chosen as the final model based on its superior performance in accuracy and balanced metrics.
   - The selected model was registered using MLflow for future reference and deployment.

## Results
   - The model with the highest accuracy and balanced performance across other metrics was the Random Forest model.
   - Detailed comparison and results of all models can be found in the experiment logs tracked via MLflow.

## View results
   - To view MLflow tracking results locally, start the MLflow UI: mlflow ui
   - For DagsHub tracking, visit the relevant repository and explore tracked experiments.

## Tools and Technologies
   - Programming Language: Python.
   - Libraries: scikit-learn, pandas, numpy, matplotlib, seaborn, MLflow.
   - Experiment Tracking: MLflow (local and DagsHub).

