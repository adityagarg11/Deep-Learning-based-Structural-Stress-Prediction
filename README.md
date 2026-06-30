<p align="center">

# Deep Learning-Based Structural Stress Prediction

**Neural Networks • Structural Mechanics • Regression • Classification • von Mises Stress Prediction**

</p>
# Deep Learning-Based Structural Stress Prediction

A deep learning project focused on predicting the **maximum von Mises stress** of cantilever beam structures from material (volume fraction) distributions. The project explores both **regression** and **classification** approaches for structural stress prediction and compares their performance, complexity, and data requirements.

---

## Project Overview

This project investigates the application of **Artificial Neural Networks (ANNs)** to surrogate structural analysis. Instead of performing computationally expensive finite element simulations for every design, neural networks are trained to learn the relationship between material distribution and the resulting maximum **von Mises stress**.

Two different machine learning approaches were implemented and evaluated:

- **Regression Model** – Predicts the numerical value of the maximum von Mises stress.
- **Classification Model** – Categorizes structures into stress percentile ranges (0–10%, 11–25%, 26–50%, and 51–100%).

The objective was to compare both methods in terms of predictive capability, computational complexity, and dataset requirements.

---

## Features

- **Neural Network-based structural stress prediction**
- **Regression model** for maximum von Mises stress estimation
- **Classification model** for stress percentile prediction
- Performance comparison between regression and classification approaches
- Evaluation of model complexity and data requirements

---

## Dataset

The dataset consists of **cantilever beam structures** with randomly generated **material (volume fraction) distributions**.

Each sample contains:

- Material (volume fraction) distribution
- Corresponding maximum **von Mises stress**

The data was used to train and evaluate both regression and classification neural network models.

---

## Methodology

### Regression

The regression model learns the mapping

> **Material Distribution → Maximum von Mises Stress**

The model predicts the exact stress value for unseen structural designs.

### Classification

The classification model predicts the stress category instead of the exact numerical value.

The stress ranges are divided into:

- **0–10 Percentile**
- **11–25 Percentile**
- **26–50 Percentile**
- **51–100 Percentile**

This formulation enables faster identification of structurally efficient designs.

---

## Technologies Used

- **Python**
- **TensorFlow / Keras**
- **NumPy**
- **Pandas**
- **Scikit-learn**
- **Matplotlib**

---

## Project Structure

```
├── Dataset/
├── Regression_Model/
├── Classification_Model/
├── Results/
├── Figures/
├── notebooks/
├── requirements.txt
└── README.md
```

---

## Results

The project demonstrates that:

- Neural networks can accurately approximate the relationship between material distribution and structural stress.
- Regression provides precise stress predictions.
- Classification offers a computationally simpler alternative for identifying high- and low-stress designs.
- Both approaches have distinct trade-offs in prediction accuracy, model complexity, and data requirements.

---

## Learning Outcomes

Through this project, I gained practical experience in:

- **Deep Learning**
- **Neural Network Design**
- **Regression & Classification**
- **Structural Mechanics**
- **Engineering Data Analysis**
- **Model Evaluation**
- **Scientific Computing with Python**

---

## Future Work

- Implement Convolutional Neural Networks (CNNs)
- Investigate Physics-Informed Neural Networks (PINNs)
- Extend the model to predict complete stress fields
- Compare against traditional finite element simulations
- Improve generalization using larger datasets

---

## Author

**Aditya Garg**

B.Tech, Mechanical Engineering  
Indian Institute of Technology Ropar

---

## License

This project is intended for **academic and educational purposes**.
