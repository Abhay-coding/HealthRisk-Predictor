# 🏥 Health Risk Classification System (NovaGen)
### End-to-End Supervised Machine Learning Pipeline (Binary Classification)

---

## 📌 Project Overview

The **Health Risk Classification System** is a supervised machine learning project
developed to classify individuals as **Healthy** or **Unhealthy** based on their
physiological measurements, lifestyle habits, and medical history.

Biomedical research organizations such as **NovaGen Research Labs** conduct
large-scale population health studies to identify individuals who may be at
higher health risk. Manual analysis of such data is often slow, inconsistent,
and difficult to scale.

This project addresses these challenges by building a **data-driven machine
learning pipeline** that enables fast, consistent, and accurate health risk
classification.

**Target Prediction:**  
✅ **Healthy (1)**  
❌ **Unhealthy (0)**  

---

## 🎯 Problem Statement

Healthcare research institutes face two major challenges:

### ⚠️ Key Challenges
1. **Failing to identify high-risk individuals** → delayed intervention and poor outcomes  
2. **Incorrectly classifying healthy individuals as high-risk** → inefficient use of resources  

### ✅ Solution
A supervised machine learning system that:
- Learns from historical health records
- Accurately classifies individuals based on risk
- Supports population-level health analysis and decision-making

---

## 🧠 Machine Learning Task

- **Learning Type:** Supervised Learning  
- **Problem Type:** Binary Classification  
- **Target Variable:** `Target`  
  - `1` → Healthy  
  - `0` → Unhealthy  

---

## 📂 Dataset Description

Each record represents a unique individual and contains a combination of
numerical and categorical health indicators.

### 🧾 Key Features

- **Physiological Measurements**
  - Age
  - BMI
  - Blood Pressure
  - Cholesterol
  - Glucose Level
  - Heart Rate

- **Lifestyle Factors**
  - Sleep Hours
  - Exercise Hours
  - Water Intake
  - Stress Level
  - Smoking
  - Alcohol Consumption

- **Health & Medical Information**
  - Mental Health Score
  - Physical Activity Level
  - Medical History
  - Allergies
  - Diet Type
  - Blood Group

---

## 🔍 Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand the dataset and uncover
important patterns, including:
- Distribution of physiological and lifestyle features
- Relationship between health habits and risk classification
- Impact of medical history and stress levels on health outcomes
- Identification of feature correlations and data balance

---

## 🛠️ Feature Engineering & Preprocessing

- Numerical features were cleaned and used directly.
- Categorical features were initially one-hot encoded.
- One-hot encoded columns related to **diet type** and **blood group** were
  merged back into single mapped categorical features to reduce dimensionality.

### Why Mapping Instead of One-Hot Encoding?

The final models used are **tree-based classifiers**, which do not rely on
distance-based or linear assumptions between feature values.  
Therefore, numeric mapping:
- Reduces feature dimensionality
- Improves interpretability
- Is computationally efficient
- Remains technically correct for tree-based models

---

## 🤖 Models Implemented

Multiple supervised machine learning models were trained and evaluated:

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Random Forest  
- Gradient Boosting  
- Voting Classifier  

---

## 📊 Results & Model Comparison

### 🔍 Evaluation Metric
**Recall** was selected as the primary evaluation metric, as correctly identifying
individuals at higher health risk is more important than minimizing false positives
in a healthcare context.

### 📈 Model Performance (Recall)

| Model               | Recall |
|--------------------|--------|
| Logistic Regression | 82.8%  |
| K-Nearest Neighbors | 88.3%  |
| Random Forest       | 95.8%  |
| Gradient Boosting   | 94.9%  |
| Voting Classifier   | 93.07% |

---

## 🏆 Best Model Selection

Based on recall performance, **Random Forest** was selected as the final model
for the NovaGen Health Risk Classification System.

- **Recall:** 95.8%  
- **Accuracy:** 93.7%  

The high recall demonstrates the model’s effectiveness in identifying
individuals who are at higher health risk, aligning well with real-world
healthcare and research objectives.

---

## 🎯 Project Outcomes

This project demonstrates:
- End-to-end supervised ML pipeline development
- Thoughtful feature engineering and encoding decisions
- Comparison of multiple classification algorithms
- Appropriate metric selection for healthcare applications
- Practical application of machine learning to real-world health data

---

## 📌 Note

This repository represents an **academic machine learning project**
developed for learning, evaluation, and demonstration purposes.

- **Accuracy:** 93.7%  

The high recall indicates that the model is highly effective at identifying
individuals who are at higher health risk, which aligns with the objectives
of population health analysis and early risk detection.

