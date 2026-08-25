# 📊 Model Evaluation Summary

This repository contains the evaluation results of our machine learning models. The dataset was split into a **70% training set** and a **30% testing set** to assess the performance and generalization capabilities of the models.

## 📈 Performance Metrics

The table below summarizes the accuracy of the two primary models evaluated:

| Model | Training Accuracy (70%) | Testing Accuracy (30%) |
| :--- | :---: | :---: |
| **Logistic Regression** | `96.23%` | `96.49%` |
| **Decision Tree** | `100.00%` | `94.15%` |

---

## 🏆 Final Conclusion

*   **Winner: Logistic Regression** (Better Generalization)
*   **Observation: Decision Tree** (Overfitting Observed)

### 🧠 Explanation
**Logistic Regression** is the recommended model for this dataset. It performed consistently across both the training and testing sets, demonstrating strong generalization capabilities without memorizing the data. 

Conversely, the **Decision Tree** achieved a perfect `100.00%` accuracy on the training data but experienced a noticeable drop to `94.15%` on the unseen testing data. This gap between training and testing performance is a classic indicator of **overfitting**, meaning the tree became too complex and modeled the noise in the training data rather than the underlying pattern.
