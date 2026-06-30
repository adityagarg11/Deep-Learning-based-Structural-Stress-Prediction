Deep Learning-Based Structural Stress Prediction
<p align="center">












Deep Learning • Structural Mechanics • Regression • Classification • Engineering AI

</p>
Overview

This project investigates the application of Deep Learning as a surrogate modeling technique for structural mechanics. The objective is to predict the maximum von Mises stress of cantilever beam structures directly from material (volume fraction) distributions, eliminating the need for computationally expensive finite element simulations for every new design.

Two independent learning approaches were implemented and evaluated:

Regression for numerical stress prediction.
Classification for stress percentile prediction.

The project also compares both approaches in terms of

Prediction accuracy
Computational complexity
Dataset requirements
Practical applicability
Problem Statement

Given the material distribution of a cantilever beam,

predict its maximum von Mises stress.

Two approaches were investigated.

Approach 1 — Regression
Material Distribution
          │
          ▼
Neural Network
          │
          ▼
Maximum von Mises Stress
Approach 2 — Classification
Material Distribution
          │
          ▼
Neural Network
          │
          ▼
Stress Category

0–10%
11–25%
26–50%
51–100%
Repository Structure
.
├── data/
├── notebooks/
├── models/
├── images/
│   ├── training_loss.png
│   ├── regression_parity.png
│   ├── confusion_matrix.png
│   └── regression_loss.png
├── requirements.txt
└── README.md
Methodology
Data Preparation
Material distribution data preprocessing
Feature normalization
Train-validation-test split
Regression Model

The regression network learns

Material Distribution → Maximum von Mises Stress

allowing continuous stress prediction for unseen designs.

Classification Model

Instead of predicting the exact stress value, the network classifies each design into one of four stress percentile ranges.

Class	Stress Percentile
0	0–10%
1	11–25%
2	26–50%
3	51–100%
Technologies Used
Category	Tools
Programming	Python
Deep Learning	TensorFlow, Keras
Data Processing	NumPy, Pandas
Machine Learning	Scikit-Learn
Visualization	Matplotlib
Results
Training Progress

The regression model converges smoothly during training.

<p align="center"> <img src="images/training_loss.png" width="750"> </p>
Regression Performance

Predicted vs Actual maximum von Mises stress.

<p align="center"> <img src="images/regression_parity.png" width="650"> </p>
Classification Performance

Confusion Matrix for the classification network.

<p align="center"> <img src="images/confusion_matrix.png" width="500"> </p>
Model Convergence

Training error throughout optimization.

<p align="center"> <img src="images/regression_loss.png" width="750"> </p>
Key Findings

✔ Neural networks successfully learned the relationship between material distribution and structural response.

✔ Regression provides accurate continuous stress prediction.

✔ Classification offers a computationally simpler alternative for identifying high- and low-stress structural designs.

✔ The study highlights the trade-offs between prediction accuracy, model complexity, and data requirements.

Skills Demonstrated
Deep Learning
Neural Networks
Regression
Multi-class Classification
Structural Mechanics
Engineering Data Analysis
Scientific Computing
Model Evaluation
Machine Learning for Physical Systems
Future Improvements
Implement Convolutional Neural Networks (CNNs)
Explore Physics-Informed Neural Networks (PINNs)
Predict the complete stress field instead of only the maximum stress
Compare performance with Finite Element Analysis (FEA)
Extend the framework to more complex structural geometries
Author

Aditya Garg

B.Tech, Mechanical Engineering

Indian Institute of Technology Ropar
