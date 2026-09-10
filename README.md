⚠️ Correction — please read first

This project was evaluated with a temporal data leakage. Rows were split randomly, but consecutive rows come from the same simulation run and are strongly correlated — so near-identical samples appeared in both the training and test sets.

The original accuracy was inflated and did not measure generalisation.

With a correct run-level split the honest figures are 83.5% accuracy and a 2.11% false alarm rate. And three of the twenty faults turn out to be undetectable — their detection rate equals the false alarm rate, because the disturbed variable is not measured at all. That is an instrumentation limit, not a modelling one.

The corrected analysis is published at [EngMtaleb/TEP](https://github.com/EngMtaleb/TEP).


🏭 Fault Detection & Predictive Maintenance

Bridging Chemical Engineering expertise with Machine Learning to detect process faults in industrial chemical plants.

📌 Project Overview

Chemical plants face costly and dangerous unplanned shutdowns due to undetected process faults. This project builds an end-to-end Industrial AI system for early fault detection and predictive maintenance, tested on the Tennessee Eastman Process (TEP) — the global benchmark dataset for industrial fault detection research.

🎯 Problem Statement
Undetected faults in chemical processes lead to safety risks, production loss, and high maintenance costs
Traditional rule-based monitoring systems miss complex, multi-variable fault patterns
This project replaces manual monitoring with intelligent ML-based fault detection
⚙️ What's Inside
1. Fault Detection Models
Model	Type
Random Forest	Ensemble
XGBoost	Gradient Boosting
LightGBM	Gradient Boosting
CatBoost	Gradient Boosting
Neural Network (MLP)	Deep Learning
LSTM	Sequential / Time-Series
TCN (Temporal Convolutional Network)	Deep Learning
2. Classification Tasks
Binary Classification — Normal vs. Faulty operation
Multi-class Classification — Identifying which of 20 distinct fault types is occurring
3. Preprocessing Pipeline
Class imbalance handling — RandomUnderSampler
Feature scaling — StandardScaler
Feature engineering informed by chemical process knowledge

⚠️ The train/test split used here is the flaw described in the correction notice above. On time-ordered process data the split must separate simulation runs, not rows.

4. Interactive Dashboard
Animated process flow diagrams
Risk matrix visualization
Root cause analysis panels
Predictive maintenance indicators
Built as a standalone interactive HTML tool
📊 Dataset

Tennessee Eastman Process (TEP) — a standard chemical process simulation benchmark used globally in fault detection research.

52 process variables (41 measured + 11 manipulated)
20 fault types + normal operation
Time-series sensor data
🛠 Tech Stack
Python · Scikit-learn · TensorFlow · Keras
XGBoost · LightGBM · CatBoost
Pandas · NumPy · Matplotlib · Plotly
Google Colab · Kaggle
🧠 Domain Expertise Applied

A chemical engineering background was used to:

Select physically meaningful process variables as features
Interpret fault signatures against known process mechanisms
Design a dashboard aligned with how plant engineers think about faults

And to find the error above. The leakage was not visible in any metric — it was visible in knowing that consecutive rows of a simulation run are not independent samples.

📁 Repository Structure
├── Final_Capstone_Project (1).ipynb   # Main notebook
├── index.html                         # Interactive dashboard
└── README.md
🔗 Live Dashboard
👤 Author

Mohammed Taleb — chemical engineer and instructor, working on AI systems for industrial process problems.

LinkedIn


