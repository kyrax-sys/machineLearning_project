# 🎗️ Breast Cancer Classification: Model Performance Comparison

## 📖 Project Overview
This project focuses on the classification of breast cancer tumors as either benign or malignant using machine learning. In this study, we utilize the Breast Cancer dataset to build and compare the predictive performance of two fundamental classification algorithms: **Logistic Regression** and a **Decision Tree Classifier**.

## 🎯 Objective
The primary objective of this project is to:
1. Train a Logistic Regression model and a Decision Tree model on breast cancer feature data.
2. Evaluate and compare their performance metrics on both seen (training) and unseen (testing) data.
3. Identify which model generalizes better for real-world diagnostic predictions.

## 📊 Dataset & Methodology
* **Dataset:** The project utilizes a standard Breast Cancer dataset (such as the Breast Cancer Wisconsin dataset).
* **Target Variable:** Diagnosis (Malignant vs. Benign).
* **Data Split:** To rigorously evaluate our models, the dataset was split into two subsets:
  * **70% Training Data:** Used to train the models and allow them to learn the underlying patterns.
  * **30% Testing Data:** Kept hidden during training and used strictly to evaluate how well the models generalize to new, unseen data.

---

## 📈 Model Evaluation Summary

After training the models on the 70% split, we evaluated their accuracy on both the training and testing sets. The table below summarizes the performance metrics of the two primary models evaluated:

| Model | Training Accuracy (70%) | Testing Accuracy (30%) |
| :--- | :---: | :---: |
| **Logistic Regression** | `96.23%` | `96.49%` |
| **Decision Tree** | `100.00%` | `94.15%` |

---

## 🏆 Final Conclusion

* **Winner: Logistic Regression** (Better Generalization)
* **Observation: Decision Tree** (Overfitting Observed)

### 🧠 Explanation
**Logistic Regression** is the recommended model for this dataset. It performed highly and consistently across both the training and testing sets (96.23% and 96.49% respectively), demonstrating strong generalization capabilities without memorizing the training data. 

Conversely, the **Decision Tree** achieved a perfect `100.00%` accuracy on the training data but experienced a noticeable drop to `94.15%` on the unseen testing data. This gap between training and testing performance is a classic indicator of **overfitting**. It indicates that the tree became too complex, modeling the specific noise and outliers in the training data rather than capturing the true, underlying biological patterns needed to accurately diagnose new cases.
