# Parkinson Disease Detection using SVM

## Overview
This project aims to develop a machine learning model to detect Parkinson’s disease using voice measurements and biomedical features. The model utilizes a **Support Vector Machine (SVM)** algorithm to classify whether a patient has Parkinson’s disease based on the provided dataset.

## Features
- End-to-end implementation in Python using Jupyter Notebook  
- Data preprocessing and normalization  
- Feature extraction and visualization  
- Model training using **SVM Classifier**  
- Model evaluation using accuracy metrics  
- Prediction system to test new input samples  

## Dataset
The dataset used in this project contains biomedical voice measurements from individuals, both healthy and affected by Parkinson’s disease.  
Each row in the dataset represents one voice recording, with various features such as:
- Fundamental frequency measurements  
- Jitter and shimmer parameters  
- Harmonic-to-noise ratio  
- Nonlinear dynamical complexity measures  

**Target variable:** `status`  
- 1 → Parkinson’s disease  
- 0 → Healthy  

## Workflow
1. **Importing Dependencies**  
   Import essential Python libraries like `numpy`, `pandas`, `sklearn`, and `matplotlib` for data processing and visualization.

2. **Data Collection and Pre-processing**  
   Load the dataset, handle missing values, and normalize feature columns for consistent scaling.

3. **Splitting Dataset**  
   Divide the dataset into training and testing sets using `train_test_split`.

4. **Model Training**  
   Train a Support Vector Machine (SVM) classifier using a linear kernel to distinguish between Parkinson’s and healthy subjects.

5. **Model Evaluation**  
   Evaluate model performance using accuracy score and confusion matrix.

6. **Prediction System**  
   Implement a system that takes input features and predicts if the person has Parkinson’s disease.

## Technologies Used
- Python 3.x  
- Jupyter Notebook  
- scikit-learn  
- NumPy  
- Pandas  
- Matplotlib  

## Results
The SVM classifier demonstrated high accuracy in predicting Parkinson’s disease, showing strong generalization across the test data.  
This makes it a reliable baseline model for further optimization and deployment.

## Author
**Raghav Bhatia**  
