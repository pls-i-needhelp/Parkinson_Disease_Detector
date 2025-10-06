# Parkinson's Disease Detector using SVM

This project uses **Machine Learning (ML)** techniques — specifically a **Support Vector Machine (SVM)** model — to detect **Parkinson’s Disease** from biomedical voice measurements.  
The goal is to assist in the early diagnosis of Parkinson’s Disease based on voice-related features.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Model Used](#model-used)
- [Workflow](#workflow)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Future Improvements](#future-improvements)
- [Contributors](#contributors)
- [License](#license)

---

## Overview
Parkinson’s Disease (PD) is a progressive neurological disorder that affects movement and speech.  
This project leverages **Machine Learning** to build a model capable of identifying Parkinson’s patients using voice features such as jitter, shimmer, and fundamental frequency.

The **Support Vector Machine (SVM)** algorithm was chosen due to its effectiveness in classification problems with small-to-medium datasets and its robustness in handling non-linear decision boundaries.

---

## Dataset
The dataset used in this project is the **UCI Machine Learning Repository – Parkinson’s Dataset**.

- **Dataset Link:** [https://archive.ics.uci.edu/ml/datasets/parkinsons](https://archive.ics.uci.edu/ml/datasets/parkinsons)
- **Number of Instances:** 195  
- **Number of Attributes:** 24 (including the target variable)  
- **Target Variable:** `status`  
  - `1` → Parkinson’s Disease  
  - `0` → Healthy  

---

## Features
Some key features used in the dataset:
- `MDVP:Fo(Hz)` — Average vocal fundamental frequency  
- `MDVP:Fhi(Hz)` — Maximum vocal fundamental frequency  
- `MDVP:Flo(Hz)` — Minimum vocal fundamental frequency  
- `MDVP:Jitter(%)`, `MDVP:Jitter(Abs)` — Measures of variation in frequency  
- `MDVP:Shimmer`, `MDVP:Shimmer(dB)` — Measures of variation in amplitude  
- `NHR`, `HNR` — Ratio measures of noise to tonal components in the voice  
- `RPDE`, `DFA` — Signal fractal scaling features  
- `spread1`, `spread2`, `PPE` — Nonlinear dynamic complexity measures  

---

## Model Used
The model used is a **Support Vector Machine (SVM)** with:
- **Kernel:** RBF (Radial Basis Function)  
- **C Parameter:** Tuned using Grid Search or manual optimization  
- **Scaler:** StandardScaler applied to normalize data  

The model separates the data points into two classes (Healthy vs Parkinson’s) using an optimal hyperplane.

---

## Workflow
1. **Import Libraries**  
2. **Load Dataset**  
3. **Data Preprocessing**  
   - Handle missing values (if any)  
   - Feature scaling using `StandardScaler`  
4. **Split Dataset**  
   - 80% training  
   - 20% testing  
5. **Model Training** using `SVM`  
6. **Prediction & Evaluation**   
   - Accuracy Score    

---


