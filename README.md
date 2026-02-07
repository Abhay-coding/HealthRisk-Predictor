# 🏥 Health Risk Classification System (NovaGen)
### End-to-End Supervised Machine Learning Pipeline (Binary Classification)

---

## 📌 Project Overview

The **Health Risk Classification System** is a supervised machine learning project
developed to classify individuals as **Healthy** or **Unhealthy** based on
physiological measurements, lifestyle habits, and medical history data.

The project is designed in the context of **NovaGen Research Labs**, a biomedical
research institute conducting large-scale population health studies. The goal is
to support data-driven decision-making by accurately identifying individuals who
may be at higher health risk.

**Target Prediction:**  
✅ **Healthy (1)**  
❌ **Unhealthy (0)**  

---

## 🧩 Problem Statement

NovaGen Research Labs conducts large-scale population health studies to better
understand how underlying health conditions influence disease risk and long-term
health outcomes. Every year, the institute recruits thousands of volunteers who
undergo medical examinations, lifestyle assessments, and clinical tests.

Despite the availability of extensive health data, researchers currently lack a
reliable and consistent method to distinguish individuals with generally healthy
profiles from those who may be at higher health risk. This limitation reduces the
effectiveness of participant selection and stratified analysis in research studies.

To address this challenge, NovaGen has compiled a dataset containing health records
from **9,800 individuals**, collected across multiple observational studies. Each
record represents a unique participant to ensure independent observations and
avoid sampling bias. The dataset includes a combination of **numerical and
categorical health indicators**, such as physiological measurements, lifestyle
factors, and medical history attributes.

As a **Data Scientist**, the objective is to develop a supervised machine learning
model that accurately classifies individuals as **healthy** or **unhealthy** based
on the available health data. This classification supports key research decisions,
including:

- Selecting eligible participants for clinical trials and longitudinal studies  
- Stratifying populations for risk-based analysis and outcome comparison  

---

## 🧠 Machine Learning Task

- **Learning Type:** Supervised Learning  
- **Problem Type:** Binary Classification  
- **Target Variable:** `Target`  
  - `1` → Healthy  
  - `0` → Unhealthy  

---

## 📂 Dataset Description

Each record represents a single individual and contains a mix of numerical and
categorical health-related features.

### 🧾 Key Features

**Physiological Measurements**
- Age  
- BMI  
- Blood Pressure  
- Cholesterol  
- Glucose Level  
- Heart Rate  

**Lifestyle Factors**
- Sleep Hours  
- Exercise Hours  
- Water Intake  
- Stress Level  
- Smoking  
- Alcohol Consumption  

**Health & Medical Information**
- Mental Health Score  
- Physical Activity Level  
- Medical History  
- Allergies  
- Diet Type  
- Blood Group  

---

## 🔍 Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to gain insights into the dataset and
understand relationships between features and health outcomes. This included:

- Distribution analysis of physiological and lifestyle features  
- Examination of health risk patterns across different lifestyle behaviors  
- Impact of medical history and stress levels on health classification  
- Identification of correlations and potential feature importance  

---

## 🛠️ Feature Engineering & Preprocessing

- Numerical features were cleaned and used directly.
- Categorical features were initially one-hot encoded.
- One-hot encoded columns related to **diet type** and **blood group** were merged
  into single mapped categorical features to reduce dimensionality.

### Why Mapping Instead of One-Hot Encoding?

The final models used in this project are **tree-based classifiers**, which do not
depend on distance-based or linear assumptions between feature values. As a result,
numeric mapping of categorical variables is:

- Technically appropriate  
- Computationally efficient  
- Easier to interpret  
- Suitable for tree-based algorithms  

---

## 🤖 Models Implemented

The following supervised machine learning models were trained and evaluated:

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Random Forest  
- Gradient Boosting  
- Voting Classifier  

---

## 📊 Results & Model Comparison

### 🔍 Evaluation Metric
**Recall** was chosen as the primary evaluation metric, as correctly identifying
individuals at higher health risk is more critical in a healthcare context than
minimizing false positives.

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

Based on recall performance, **Random Forest** was selected as the final model for
the Health Risk Classification System.

- **Recall:** 95.8%  
- **Accuracy:** 93.7%  

The high recall indicates that the model is highly effective at identifying
individuals who may be at higher health risk, aligning well with the objectives
of population health research and early risk detection.

---

## 🎯 Project Outcomes

This project demonstrates:

- End-to-end supervised ML pipeline development  
- Thoughtful feature engineering and encoding decisions  
- Comparative evaluation of multiple classification models  
- Appropriate metric selection for healthcare applications  
- Practical application of machine learning to real-world health data  

---

## 📌 Note

This repository represents an **academic machine learning project** developed
for learning, evaluation, and demonstration purposes.
