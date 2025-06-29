# End-to-End ML Regression Project

This repository demonstrates a **complete machine learning pipeline**, covering everything from data acquisition to feature transformation. It is based on **Chapter 2** of *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow* by Aurélien Géron.

The project uses the **California housing dataset** and is designed to serve as a robust template for structuring real-world regression workflows.

---

## Project Highlights

- Clean, modular pipeline using **Scikit-Learn**
- Exploratory Data Analysis (EDA) with insightful visualizations
- Feature engineering (ratios, log transforms, cluster similarities)
- Custom transformers and reusable pipeline components
- One-hot encoding of categorical features
- Unified `ColumnTransformer`-based preprocessing pipeline
- Output-ready dataset with **24 engineered features**

---

## Goal

To provide a clear, modular, and reproducible example of a real-world machine learning pipeline for regression tasks—structured in a way that supports scaling, experimentation, and future model training.

---

## Dataset

**California Housing Dataset** from the 1990 U.S. Census  
- Predicts median house value from 9+ features
- Common benchmark for regression modeling and pipeline design  
- Loaded via `fetch_california_housing` or from external `.tgz` file

---

## Core Concepts Covered

| Concept                      | Implementation                               |
|-----------------------------|-----------------------------------------------|
| Data Loading                | `fetch_housing_data()` with caching          |
| Visualization               | Histograms, scatterplots, `scatter_matrix`   |
| Stratified Sampling         | Based on income categories                   |
| Correlation Analysis        | Pearson coefficient, matrix, and plots       |
| Feature Engineering         | Rooms-per-household, income ratios, etc.     |
| Pipelines                   | `Pipeline` + `ColumnTransformer`             |
| Custom Transformers         | `CombinedAttributesAdder`, cluster encoder   |
| Categorical Encoding        | `OneHotEncoder`                              |
| Scaling                     | `StandardScaler`                             |

---

## Reference

Based on concepts from:

> *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow*  
> by **Aurélien Géron**

- [📘 Book Website](https://github.com/ageron/handson-ml3)
- [📓 Google Colab Notebooks](https://colab.research.google.com/github/ageron/handson-ml3/blob/main)

---

## Notes

This repo focuses only on data handling and preprocessing. **Model training, evaluation, and hyperparameter tuning**
