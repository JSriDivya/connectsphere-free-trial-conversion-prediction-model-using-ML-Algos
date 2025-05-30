# 🧠 Predicting Free Trial Conversion for ConnectSphere using Artificial Neural Network (ANN)

## Overview

This project simulates a real-world business scenario for **ConnectSphere**, a fictional collaboration platform, aiming to predict which users are most likely to convert from a **free trial** to a **paid subscription**. The goal is to apply machine learning techniques, specifically an **Artificial Neural Network (ANN)**, to understand user behavior and improve marketing and product strategies.

---

## 📊 Business Context

ConnectSphere offers a 14-day free trial. Thousands of users sign up every month, but only a small percentage convert to paid users. The team wants to:
- Identify which usage patterns indicate a high probability of conversion
- Proactively engage high-potential users to boost conversion rates
- Reduce churn during the trial period

---

## 🎯 Objective

Build and evaluate an ANN model using **dummy behavioral data** to:
- Predict whether a user will convert to a paid plan
- Understand which features contribute most to conversion
- Simulate a working prototype that could be adapted for real user data

---

## 🧪 Data Simulation

Since real data isn't available, we simulate a dataset with the following features:

| Feature | Description |
|--------|-------------|
| `projects_created` | Number of projects created during trial |
| `tasks_created` | Number of tasks added |
| `team_members_invited` | Number of teammates invited |
| `features_used_count` | Number of different features used |
| `avg_daily_session_time_minutes` | Average time spent per day (in minutes) |
| `completed_onboarding_checklist` | Whether the user completed onboarding |
| `support_tickets_opened` | Number of support requests raised |
| `marketing_source` | How the user found ConnectSphere (`Organic`, `Paid Ad`, `Referral`) |
| `converted_to_paid` | Target variable (0 = No, 1 = Yes) |

The `converted_to_paid` column is derived using simple rule-based logic for simulation purposes.

---

## 🧠 Model Architecture

We use a simple **Feedforward Neural Network (ANN)** built with **TensorFlow/Keras**:

- **Input Layer**: Scaled numeric + one-hot encoded categorical features
- **Hidden Layers**: 
  - Dense(16) with ReLU
  - Dense(8) with ReLU
- **Output Layer**: Dense(1) with Sigmoid activation (binary classification)

---

## ⚙️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib (optional for visualization)

---

## 📈 Evaluation Metrics

- Accuracy
- Confusion Matrix
- Precision / Recall / F1 Score

