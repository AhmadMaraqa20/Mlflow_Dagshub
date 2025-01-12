# ML Model Development and Offline Evaluation


## Project Overview
   - This project demonstrates the usage of MLflow for tracking machine learning experiments and managing the end-to-end ML lifecycle. The implementation includes:
1. Model Training and Logging: Tracks experiments with parameters, metrics, and models.
2. Local MLflow Server Setup: Provides instructions to host MLflow locally for tracking runs.
3. Model Registry: Registers models for versioning and deployment.

## Prerequisites
1-MLflow: Install MLflow via pip:
```bash
pip install mlflow
```
2-Environment Setup: Install additional dependencies by running:
```bash
pip install -r requirements.txt
```


## Dataset
The dataset used in this project is sourced from Kaggle: [Mushroom Classification](https://www.kaggle.com/datasets/prishasawhney/mushroom-dataset). It is a cleaned version of the original UCI Mushroom Dataset and includes 9 columns describing physical attributes of mushrooms for classification.

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
   - For DagsHub tracking, visit the relevant repository and explore tracked experiments [(press here)](https://dagshub.com/AhmadMaraqa20/Mlflow_Dagshub).

## Tools and Technologies
   - Programming Language: Python.
   - Libraries: scikit-learn, pandas, numpy, matplotlib, seaborn, MLflow.
   - Experiment Tracking: MLflow ((local setup and DagsHub integration)).

