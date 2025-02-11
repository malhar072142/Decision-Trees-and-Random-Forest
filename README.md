# 🏎️ Decision Trees & Random Forest in Formula 1

A practical explanation of Decision Trees and Random Forest regression using **Formula 1 weather prediction** as an example.

## 📌 Overview

Decision Trees and Random Forests are widely used machine learning models for **classification and regression** tasks. This project explores their implementation using **Formula 1 weather data**, demonstrating their **effectiveness in predictive modeling**.

## 🎯 Objectives

- Explain **Decision Trees** and their core concepts (nodes, splitting, pruning, impurity).
- Introduce the **Random Forest algorithm** and how it improves upon Decision Trees.
- Apply these models to **predict weather conditions** during F1 races.
- Compare **Random Forest vs Logistic Regression** for classification accuracy.

## 📂 Dataset

- **Source:** Formula 1 telemetry and weather monitoring systems.
- **Size:** 3,572,328 records collected over multiple races.
- **Features:**
  - **M_SESSION_UID:** Unique identifier for race session.
  - **M_TRACK_TEMPERATURE:** Temperature of the track (°C).
  - **M_AIR_TEMPERATURE:** Air temperature (°C).
  - **M_WEATHER:** Weather condition (target variable, categorical 0-5).

## 🌳 Decision Trees

- **Key Concepts:**
  - **Root Node:** The primary decision point.
  - **Splitting:** Dividing data based on feature values.
  - **Gini Impurity & Entropy:** Measures of node purity.
  - **Information Gain:** Selecting the best split.
  - **Pruning:** Preventing overfitting by limiting tree depth.

- **Implementation Steps:**
  - Compute Gini Impurity for attributes.
  - Select the root node based on impurity values.
  - Recursively split the tree until optimal classification is reached.

## 🌲 Random Forest Algorithm

- **How it Works:**
  - Uses **Bootstrap Aggregation (Bagging)** to create multiple Decision Trees.
  - Each tree makes a prediction, and the final result is based on **majority voting** (classification) or **averaging** (regression).

- **Advantages:**
  - Higher accuracy due to ensemble learning.
  - Handles **non-linearity** and **outliers** better.
  - Less prone to **overfitting** compared to single Decision Trees.

## 📊 Model Evaluation

- **Baseline Model:** Initial Random Forest model achieved **79% accuracy**.
- **Optimized Model:** Feature selection using ANOVA F-test improved accuracy to **91%**.
- **Comparison with Logistic Regression:**
  - **Random Forest:** 91% accuracy, high precision & recall.
  - **Logistic Regression:** 69% accuracy, lower performance on complex patterns.

## 📌 Future Enhancements

- **Hyperparameter tuning** for further optimization.
- **Handling class imbalance** by augmenting underrepresented classes.
- **Deploying as a real-time predictive system** for F1 race strategies.

## 👥 Contributors

- **Malhar Ghogare** *(GitHub: [@YourUsername](https://github.com/YourUsername))*
- **Shubham Gaur**

## 📜 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

Let me know if you'd like any changes! 🚀
