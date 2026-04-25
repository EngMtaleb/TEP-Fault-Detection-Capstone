# 🏭 Fault Detection & Predictive Maintenance

> **Bridging Chemical Engineering expertise with Machine Learning to detect process faults in industrial chemical plants.**

---

## 📌 Project Overview

Chemical plants face costly and dangerous unplanned shutdowns due to undetected process faults. This project builds an **end-to-end Industrial AI system** for early fault detection and predictive maintenance, tested on the **Tennessee Eastman Process (TEP)** — the global benchmark dataset for industrial fault detection research.

---

## 🎯 Problem Statement

- Undetected faults in chemical processes lead to safety risks, production loss, and high maintenance costs
- Traditional rule-based monitoring systems miss complex, multi-variable fault patterns
- This project replaces manual monitoring with intelligent ML-based fault detection

---

## ⚙️ What's Inside

### 1. Fault Detection Models
| Model | Type |
|---|---|
| Random Forest | Ensemble |
| XGBoost | Gradient Boosting |
| LightGBM | Gradient Boosting |
| CatBoost | Gradient Boosting |
| Neural Network (MLP) | Deep Learning |
| LSTM | Sequential / Time-Series |
| TCN (Temporal Convolutional Network) | Deep Learning |

### 2. Classification Tasks
- **Binary Classification** — Normal vs. Faulty operation
- **Multi-class Classification** — Identifying which of **20 distinct fault types** is occurring

### 3. Preprocessing Pipeline
- Class imbalance handling — `RandomUnderSampler`
- Feature scaling — `StandardScaler`
- Train/Test split — 80/20
- Feature engineering based on chemical process domain knowledge

### 4. Interactive Dashboard
- Animated process flow diagrams
- Risk matrix visualization
- Root cause analysis panels
- Predictive maintenance indicators
- Built as a standalone interactive HTML tool

---

## 📊 Dataset

**Tennessee Eastman Process (TEP)** — a standard chemical process simulation benchmark used globally in fault detection research.

- 52 process variables (41 measured + 11 manipulated)
- 20 fault types + normal operation
- Time-series sensor data

---

## 🛠 Tech Stack

```
Python · Scikit-learn · TensorFlow · Keras
XGBoost · LightGBM · CatBoost
Pandas · NumPy · Matplotlib · Plotly
Power BI · Google Colab · Kaggle
```

---

## 🧠 Domain Expertise Applied

This project leverages a **Chemical Engineering background** to:
- Select the most physically meaningful process variables as features
- Interpret fault signatures using process knowledge
- Design a dashboard aligned with how plant engineers think about faults

> This domain-guided approach is what separates this work from a purely data-driven analysis.

---

## 📁 Repository Structure

```
├── Final_Capstone_Project (1).ipynb   # Main notebook
├── README.md
└── dashboard/
    └── index.html    # Interactive dashboard
```

---

## 👤 Author

**Mohammed Taleb**
Chemical Engineer → AI & Data Science

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/mohammed-taleb-4b4195115/)


