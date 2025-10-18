
# 💳 Credit Fraud Detector

### 📘 Overview

This project focuses on **detecting fraudulent credit card transactions** using Machine Learning techniques. It explores various **predictive models**, **resampling methods**, and **evaluation metrics** to handle the challenges of **imbalanced datasets** effectively.

> ⚠️ *Note:* Some aspects of this notebook are still being refined. The goal is to provide a clear explanation of the reasoning behind every step and ensure accurate fraud detection performance.

---

## 🚀 **Before We Begin**

If you find this project useful, please ⭐️ star or upvote this kernel — it motivates further research to enhance fraud detection accuracy across both **fraudulent** and **non-fraudulent** transactions.

---

## 🧠 **Introduction**

This project uses various **predictive models** to determine whether a transaction is a **normal payment** or **fraudulent**.
The dataset has **scaled features** and anonymized column names due to privacy concerns, yet it still allows for effective analysis and modeling.

---

## 🎯 **Project Goals**

* Understand the distribution of data and detect imbalances.
* Create a **50/50 balanced dataset** using **NearMiss Algorithm**.
* Implement and evaluate multiple **classifiers** to identify the most accurate model.
* Develop a **Neural Network** and compare it with traditional classifiers.
* Recognize and avoid common pitfalls in **imbalanced data handling**.

---

## 🧩 **Outline**

### I. Understanding the Data

* a) Gather sense of our dataset (EDA, class distribution).

### II. Preprocessing

* a) Scaling and distributing features.
* b) Splitting data into training and testing sets.

### III. Handling Imbalanced Data

* a) Random Undersampling and Oversampling.
* b) Distributing and correlating.
* c) Anomaly detection.
* d) Dimensionality reduction and clustering using **t-SNE**.
* e) Applying classifiers and tuning hyperparameters.
* f) Oversampling with **SMOTE**.

### IV. Testing and Evaluation

* a) Logistic Regression testing.
* b) Neural Network testing (Undersampling vs Oversampling comparison).

---

## ⚙️ **Techniques and Considerations**

### 🧮 Correcting Mistakes from Imbalanced Datasets

* Never test on oversampled or undersampled data — only the model should be trained on it.
* Apply resampling during cross-validation, **not before**.
* Avoid **accuracy** as a metric; use **F1-score**, **Precision/Recall**, and **Confusion Matrix** instead.

---

## 📊 **Summary Insights**

* The mean transaction amount ≈ **USD 88**.
* **No null values** in the dataset.
* **Fraudulent transactions:** ~0.17%
* **Non-fraudulent transactions:** ~99.83%

---

## 🧠 **Feature Details**

* **PCA Transformation:** Applied to most features (except `Time` and `Amount`).
* **Scaling:** All `V` features are already scaled as part of preprocessing.


## 📦 **Files Included**

* `creditcard.csv` — Dataset used for fraud detection
* `README.txt` — Project documentation (this file)

