📌 Overview

This project focuses on classifying wine quality using machine learning techniques. The goal is to predict whether a wine sample is of high quality or low quality based on its physicochemical properties.

🧠 Problem Formulation

The original dataset contains a quality score (0–10).
We convert it into a binary classification problem:

1 → High Quality (quality ≥ 6)
0 → Low Quality (quality < 6)
📂 Dataset
Red Wine Dataset
White Wine Dataset

Both datasets are:

Combined into a single dataset
A new feature wine_type is added:
0 → Red Wine
1 → White Wine
⚙️ Workflow
1. Data Preprocessing
Merging datasets
Creating target labels
Feature scaling using StandardScaler
2. Exploratory Data Analysis (EDA)
Data inspection (info, describe)
Distribution analysis
Understanding feature behavior
3. Train-Test Split

The dataset is divided into:

Training Set
Testing Set
🤖 Models Used
🔹 Hard Margin SVM
Kernel: Linear
C = 100
Assumes near-perfect linear separability
🔹 Soft Margin SVM
Kernel: Linear
C = 1.0
Allows misclassification for better generalization
🔹 XGBoost Classifier
n_estimators = 100
learning_rate = 0.1
max_depth = 3
Gradient boosting-based model with strong performance
📊 Evaluation Metrics

Models are evaluated using:

Accuracy
F1 Score
ROC AUC Score
📈 Results & Comparison
ROC Curves are plotted for all models
XGBoost generally achieves the best performance
Soft Margin SVM performs better than Hard Margin in real-world scenarios
🛠️ Technologies Used
Python
NumPy & Pandas
Matplotlib & Seaborn
Scikit-learn
XGBoost
🎯 Key Learnings
Understanding the difference between Hard Margin and Soft Margin SVM
Applying preprocessing techniques like feature scaling
Comparing traditional ML models with boosting methods
Evaluating models using multiple performance metrics
📎 Notes

This project was implemented as part of a Pattern Recognition course assignment, focusing on practical application of classification algorithms.
