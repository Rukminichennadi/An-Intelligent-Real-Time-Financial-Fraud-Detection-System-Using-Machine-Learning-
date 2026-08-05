Overview

This repository contains the implementation of an Intelligent Real-Time Financial Fraud Detection System developed as part of an MSc dissertation at the University of Roehampton. The project focuses on detecting fraudulent financial transactions by combining Machine Learning, Deep Learning, and Explainable Artificial Intelligence (XAI) techniques. The proposed framework is designed to improve fraud detection accuracy, reduce false positives, and provide transparent predictions that can support decision-making in digital financial services.

The project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology, covering the complete machine learning pipeline from data preprocessing to model evaluation and explainability.

Project Objectives

The primary objectives of this project are to:

Develop an intelligent fraud detection framework using supervised and unsupervised learning.
Compare the performance of traditional machine learning, ensemble learning, and deep learning models.
Improve fraud detection in highly imbalanced datasets.
Reduce false-positive predictions while maintaining high recall.
Provide interpretable predictions using Explainable AI (SHAP).
Dataset

The project uses the PaySim Financial Transaction Dataset, a synthetic dataset that simulates mobile money transactions based on real-world financial behaviour. It contains millions of financial transactions, including both legitimate and fraudulent activities, making it suitable for fraud detection research.

The dataset includes features such as:

Transaction type
Transaction amount
Transaction timestamp
Sender and receiver balances
Fraud labels
Rule-based fraud flags

Additional behavioural and account-consistency features were engineered to improve model performance.

Technologies Used
Python
Jupyter Notebook
Pandas
NumPy
Scikit-learn
XGBoost
TensorFlow / Keras
SHAP
Matplotlib
Seaborn
Machine Learning Models

Multiple models were implemented and evaluated, including:

Logistic Regression
Decision Tree
Random Forest
XGBoost
Deep Neural Network (DNN)
Long Short-Term Memory (LSTM)
Autoencoder

A hybrid framework combines the strengths of ensemble learning and deep learning to enhance fraud detection performance.

Project Workflow

The implementation follows these major stages:

Data Loading
Data Cleaning and Preprocessing
Exploratory Data Analysis (EDA)
Feature Engineering
Handling Class Imbalance
Model Development
Model Training
Model Evaluation
Explainable AI Analysis using SHAP
Performance Comparison
Feature Engineering

Several new features were created to improve predictive performance, including:

Transaction time features
Balance consistency features
Transaction amount ratio
Behavioural transaction indicators
One-hot encoded transaction types

These engineered features help the models capture abnormal transaction behaviour more effectively.

Model Evaluation

The models were evaluated using industry-standard classification metrics suitable for imbalanced datasets:

Accuracy
Precision
Recall
F1-Score
ROC-AUC
Precision-Recall Curve
Confusion Matrix
Cross-Validation

Performance comparison enables identification of the most effective fraud detection approach.

Explainable AI

The project incorporates SHAP (SHapley Additive exPlanations) to improve model transparency. SHAP identifies the contribution of each feature to individual fraud predictions, allowing users to understand why a transaction is classified as fraudulent or legitimate. This enhances trust, interpretability, and supports responsible AI deployment.

Repository Structure
Financial-Fraud-Detection/
│
├── Code_Software.ipynb          # Complete project implementation
├── README.md                    # Project documentation
├── requirements.txt             # Python dependencies
├── Dataset/                     # Dataset (if included)
├── Images/                      # Figures and visualisations
├── Results/                     # Model outputs and evaluation results
└── LICENSE                      # License information
Installation

Clone the repository:

git clone https://github.com/your-username/Financial-Fraud-Detection.git

Navigate to the project folder:

cd Financial-Fraud-Detection

Install the required packages:

pip install -r requirements.txt

Launch Jupyter Notebook:

jupyter notebook

Open Code_Software.ipynb and run the notebook sequentially.

Key Features
End-to-end fraud detection pipeline
Advanced feature engineering
Multiple machine learning and deep learning models
Hybrid fraud detection framework
Class imbalance handling
Explainable AI using SHAP
Comparative performance analysis
Publication-style visualisations
Future Enhancements

Future work may include:

Real-time transaction streaming
REST API deployment using Flask or FastAPI
Cloud deployment on AWS or Azure
Continuous model retraining for concept drift
Integration with fraud monitoring dashboards
Transformer-based deep learning models
Acknowledgements

This project was developed as part of the MSc programme at the University of Roehampton. The implementation is based on the PaySim Financial Transaction Dataset and demonstrates the application of machine learning, deep learning, and explainable AI for intelligent financial fraud detection.

License

This project is intended for academic and research purposes. Please ensure appropriate citation and acknowledgement if the work is used in research or educational projects.