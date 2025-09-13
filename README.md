# 🍷 Wine Dataset Classification – Model Comparison

## 📌 Description

This project applies **multiple Machine Learning algorithms** on the **Wine Dataset** (from `sklearn.datasets`) to classify different wine types based on their chemical properties.
The goal is to **compare at least 5 ML models** and select the **best performing model** using accuracy as the metric.

---

## ❓ Reason for Project

Machine Learning offers various algorithms for classification, but their performance differs depending on the dataset.
The **Wine dataset** is widely used in ML research and education, making it a great candidate for benchmarking algorithms.
This project demonstrates **model selection** through systematic comparison.

---

## 📂 Table of Contents

1. [Description](#-description)
2. [Reason for Project](#-reason-for-project)
3. [Dataset Information](#-dataset-information)
4. [Requirements](#-requirements)
5. [Algorithms Compared](#-algorithms-compared)
6. [Results](#-results)
7. [Why These Results?](#-why-these-results)
8. [Visualization](#-visualization)
9. [Acknowledgment](#-acknowledgment)

---

## 🍇 Dataset Information

The **Wine Dataset** is a classic dataset available in `scikit-learn` and originally from the **UCI Machine Learning Repository**.

* **Classes (Target):** 3 types of wines (Class 0, Class 1, Class 2).
* **Features:** 13 chemical properties (e.g., Alcohol, Malic acid, Ash, Magnesium, Flavanoids, Proline, etc.).
* **Samples:** 178 wine samples in total.

This dataset is commonly used for **classification** and is linearly separable in many cases, making it ideal for comparing algorithms.

---

## 🛠 Requirements

Install dependencies before running the program:

```bash
pip install scikit-learn matplotlib
```

---

## 🤖 Algorithms Compared

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Decision Tree
* Random Forest
* Naive Bayes
* Gradient Boosting

---

## 📊 Results

| Algorithm           | Mean Accuracy | Std Deviation |
| ------------------- | ------------: | ------------: |
| Logistic Regression |     **0.956** |         0.038 |
| KNN                 |         0.691 |         0.049 |
| SVM                 |         0.663 |         0.046 |
| Decision Tree       |         0.882 |         0.059 |
| Random Forest       |     **0.978** |         0.021 |
| Naive Bayes         |         0.966 |         0.021 |
| Gradient Boosting   |         0.933 |         0.041 |

✅ **Best Model: Random Forest** with \~97.8% accuracy.

---

## 🧐 Why These Results?

* **Random Forest (Best)** – Performs well due to ensemble learning, reducing overfitting and handling nonlinear feature interactions effectively.
* **Naive Bayes & Logistic Regression** – Work well since the dataset is relatively small, clean, and somewhat linearly separable.
* **Decision Tree** – Good performance but slightly less stable (higher variance).
* **Gradient Boosting** – Strong performance, but slightly lower than Random Forest on this dataset due to limited sample size.
* **KNN & SVM (Lowest)** – Struggled because of feature scaling sensitivity and overlapping class boundaries in high dimensions.

---

## 📈 Visualization

Boxplot comparing classification accuracy of models:

<img width="555" height="418" alt="Image" src="https://github.com/user-attachments/assets/46c51f9c-284b-4f40-a2dc-212aad94411f" />

---

## 🙏 Acknowledgment

* **scikit-learn developers** for providing the Wine dataset and ML models.
* **UCI Machine Learning Repository** (original source of Wine dataset).
* Open-source contributors of **Matplotlib** for visualization.

