# rescue1122-ems-machine-learning

> Machine Learning Analysis of Emergency Medical Services Using Rescue 1122 Data from Punjab, Pakistan

## 📌 Brief One-Line Summary

A machine-learning project evaluating emergency response patterns, vehicle effectiveness, and patient outcomes within the Rescue 1122 emergency medical service system of Punjab, Pakistan.

---

## 📖 Overview

Emergency medical services (EMS) play a critical role in reducing mortality by providing rapid medical assistance to patients.

This project analyzes Rescue 1122 emergency response data from Punjab, Pakistan, with a particular focus on comparing **motorbike and ambulance responses**.

The study combines large-scale data preprocessing, exploratory data analysis, statistical analysis, feature engineering, and machine-learning models to investigate whether the speed advantage of motorbike responses is associated with improved patient outcomes.

---

## ❗ Problem Statement

Emergency medical services in low- and middle-income countries often operate under challenging urban and rural conditions.

Motorbike emergency responders may reach patients faster than conventional ambulances because they can navigate traffic congestion, narrow roads, and difficult urban environments more efficiently.

However, faster response does not necessarily guarantee better patient outcomes.

This project addresses the following research question:

**Does the response-time advantage of motorbike emergency units translate into improved patient outcomes, and for which emergency and geographic conditions is this advantage most important?**

---

## 📊 Dataset

The analysis uses Rescue 1122 emergency response records from Punjab, Pakistan.

### Dataset Statistics

| Description | Number |
|---|---:|
| Original Rescue 1122 records | 1,808,946 |
| Complete ambulance/motorbike cases | 1,063,122 |
| Class-balanced ML dataset | 26,271 |
| Training cases | 21,016 |
| Testing cases | 5,255 |

### Main Variables

The dataset contains variables related to:

- Vehicle type
- Emergency type
- Injury type
- Patient age
- Gender
- Urban/rural location
- Vehicle distance
- Response delay
- Call-to-arrival interval
- Trip duration
- Patient outcome

> **Note:** Raw Rescue 1122 data are not publicly included in this repository because of data-access, privacy, and institutional restrictions.

---

## 🛠️ Tools and Technologies

### Programming Language

- Python

### Data Analysis

- Pandas
- NumPy

### Data Visualization

- Matplotlib
- Seaborn

### Machine Learning

- Scikit-learn
- XGBoost
- TensorFlow
- Keras

### Statistical Analysis

- Logistic Regression
- Confidence Intervals
- Subgroup Analysis

### Development Environment

- Jupyter Notebook
- Google Colab / Local Python Environment

---

## 🔬 Methods

The complete analytical workflow consists of the following stages:

```text
Raw Rescue 1122 Data
        │
        ▼
Data Preprocessing
        │
        ▼
Column Selection
        │
        ▼
Data Cleaning
        │
        ▼
Vehicle Type Filtering
        │
        ▼
Category Remapping
        │
        ▼
Time-Based Feature Engineering
        │
        ▼
Numerical Validation
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Stratified Sampling
        │
        ▼
Class Balancing
        │
        ▼
Feature Finalization
        │
        ▼
Train / Test Split
        │
        ├──────────────┬──────────────┐
        ▼              ▼              ▼
 Random Forest      XGBoost      Neural Network
        │              │              │
        └──────────────┼──────────────┘
                       ▼
                Model Evaluation
                       │
             ┌─────────┼─────────┐
             ▼         ▼         ▼
         Accuracy   Confusion   Feature
                    Matrix     Importance
                       │
                       ▼
                  Final Results
