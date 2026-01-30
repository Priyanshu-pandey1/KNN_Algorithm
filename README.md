# Heart Disease Prediction using KNN (Optimized)

This repository contains a Machine Learning project that uses the **K-Nearest Neighbors (KNN)** algorithm to classify heart disease cases. The model has been optimized using **GridSearchCV** and **Pipelines** for better performance and scalability.

## 📌 Project Overview
The goal is to accurately predict heart disease based on clinical data. This implementation focuses on finding the best number of neighbors ($K$) and using feature scaling to ensure the model makes reliable predictions.

## 🛠️ Tech Stack & Workflow
* **Language:** Python
* **Preprocessing:** `StandardScaler` (to normalize health metrics).
* **Optimization:** `GridSearchCV` (for hyperparameter tuning).
* **Automation:** Scikit-Learn `Pipeline`.

## 📊 Dataset Information
* **File:** `heart.csv`
* **Features:** Clinical attributes (age, sex, cholesterol, max heart rate, etc.).
* **Target:** `1` = Presence of heart disease, `0` = Absence.

## 📈 Model Performance
After performing hyperparameter tuning, the model achieved its best results with **K=9**. The evaluation metrics on the test set are as follows:

| Metric | Score (Decimal) | Score (Percentage) |
| :--- | :--- | :--- |
| **Accuracy** | 0.8524 | **85.25%** |
| **Precision** | 0.8055 | **80.56%** |
| **Recall** | 0.9354 | **93.55%** |

> **Key Insight:** The model has an exceptionally high **Recall (93.55%)**, which means it is very safe for medical use as it rarely misses a patient who actually has heart disease.

## ⚙️ Best Parameters
Based on the Grid Search results, the following parameter was selected:
* **Best K (n_neighbors):** 9

## 📂 File Structure
* `knn.ipynb`: Main Jupyter Notebook with code and analysis.
* `heart.csv`: The dataset used for training and testing.
* `README.md`: Documentation and performance report.
