# Polycystic Ovary Syndrome (PCOS) Diagnosis: A Machine Learning Benchmark Analysis

This repository contains an end-to-end machine learning pipeline built to automate the early detection and risk assessment of Polycystic Ovary Syndrome (PCOS). By benchmarking eight distinct classification algorithms, this project identifies the most accurate and computationally efficient predictive frameworks to aid clinical decision-making.

## 📂 Project Artifacts & Structure
*   `pcos_dataset.csv`: The structured clinical dataset containing 1,000 patient records.
*   `REPORT BASED ON PCOS DIAGNOSIS.docx`: The comprehensive technical report evaluating algorithm effectiveness.
*   `README.md`: The repository summary and high-level benchmark overview.
   
## 📊 Dataset Overview
The analysis leverages a synthetic dataset of **1,000 patient entries** containing key clinical features highly correlated with PCOS risk factors:
*   **Age (years):** Patient age ranging from 18 to 45.
*   **BMI (kg/m²):** Body Mass Index ranging from 18 to 35.
*   **Menstrual Irregularity:** Binary indicator (0 = Regular, 1 = Irregular).
*   **Testosterone Level (ng/dL):** Blood hormonal indicator ranging from 20 to 100 ng/dL.
*   **Antral Follicle Count:** Ovarian reserve evaluation via ultrasound ranging from 5 to 30.
*   **Target Variable (PCOS Diagnosis):** Binary outcome (0 = Negative, 1 = Positive).

---

## 🛠️ Tech Stack & Dependencies
*   **Language:** Python 3.11+
*   **Machine & Deep Learning:** `scikit-learn`, `tensorflow` 
*   **Data Analysis & Engineering:** `pandas`, `numpy`
*   **Data Visualization:** `matplotlib`, `seaborn`

---

## 📈 Benchmark & Evaluation Results
Eight distinct algorithms were evaluated across standard performance metrics to identify the absolute best diagnostic model:

| Algorithm | Accuracy | Precision | Recall | F1-Score | Computation Time |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Artificial Neural Networks (ANN)** | **92%** | **90%** | **88%** | **89%** | Very High |
| **Gradient Boosting (GB)** | 91% | 89% | 86% | 87% | High |
| **Random Forest (RF)** | 90% | 88% | 85% | 86% | Moderate |
| **Support Vector Machine (SVM)** | 87% | 85% | 84% | 84.5% | High |
| **Decision Tree (DT)** | 85% | 82% | 80% | 81% | Low |
| **Logistic Regression (LR)** | 83% | 81% | 79% | 80% | Low |
| **K-Nearest Neighbors (KNN)** | 82% | 80% | 78% | 79% | Very High |
| **Naive Bayes (NB)** | 78% | 76% | 74% | 75% | Very Low |

---

## 🔍 Key Engineering Insights
*   **Top Diagnostic Predictor:** The **Artificial Neural Network (ANN)** yielded the highest generalization metrics with a **92% global accuracy** and a balanced **89% F1-Score**, making it highly reliable for clinical deployment.
*   **Optimal Deployment Alternative:** **Random Forest** serves as the strongest ensemble architecture, providing near-identical performance metrics with significantly lower computational latency.
*   **Feature Dominance:** Horizontal feature importance charts confirm that **BMI** and **Menstrual Irregularity** carry the highest statistical weight when predicting positive PCOS outcomes.

---

