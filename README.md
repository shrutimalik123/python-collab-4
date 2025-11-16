# python-collab-4

Day 4

https://colab.research.google.com/drive/1Cbk1kYrK_IB7XrXl3Sv9ZTEyBF5bMmeY?usp=sharing

Day 4 Project: MLOps Experiment Tracking SimulationProject 

File: mlops_logger.py

Skill Focus: MLOps, Experiment Tracking, Artifact Logging, Production Readiness (Simulated)

Description: Implemented a custom MLOps_Logger Python class to simulate an MLOps experiment tracker (like MLflow). This class logs all crucial parameters, metrics, and saves essential model components as artifacts for deployment. This directly addresses the job requirement for "Strong experience with MLOps" and "deployment of machine learning... models in production.

"Key MLOps Steps Demonstrated:

Unique Run ID: Every experiment run gets a unique, timestamped ID to ensure full traceability.

Parameter Logging: Documented model hyper-parameters (model_type, solver, features_used).

Metrics Logging: Recorded model performance metrics (accuracy, precision, recall).

Artifact Saving: Crucially, saved both the trained model (model.pkl) and the StandardScaler (scaler.pkl). 
Saving the scaler is vital, as it ensures production inputs are transformed identically to the training data.

Day 4 Net Results

This exercise successfully created a local directory structure mirroring an MLOps platform, demonstrating the ability to manage and reproduce model runs—a necessity for compliance and model governance in healthcare.

MLOps 

OutputFile

Name

Purpose in Production

Parameters

params.json

Ensures reproducibility by documenting exactly how the model was configured and what features it used.

Model Artifact

model.pkl

The trained Logistic Regression object, ready for serving.

Data Artifact

scaler.pkl

Critical for serving. Ensures any new patient data is scaled (normalized) exactly as the training data was before making a prediction.
