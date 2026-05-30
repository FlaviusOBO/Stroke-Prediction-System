# Stroke Prediction Using Machine Learning

## Project Overview

Stroke is one of the leading causes of death and long-term disability worldwide. Early identification of individuals at high risk can significantly improve prevention efforts and clinical outcomes. This project investigates the effectiveness of multiple machine learning algorithms for predicting stroke occurrence using demographic, lifestyle, and clinical health indicators.

The primary objective is to compare the performance of traditional and advanced machine learning models to determine the most accurate and clinically practical approach for stroke risk prediction.

---

## Problem Statement

Traditional statistical methods often struggle to capture the complex relationships between clinical and behavioral risk factors associated with stroke. This project evaluates whether modern machine learning techniques can improve predictive performance and support healthcare decision-making.

---

## Dataset

The dataset was obtained from Kaggle and contains demographic, behavioral, and clinical attributes commonly associated with stroke risk.

### Features

* Gender
* Age
* Hypertension
* Heart Disease
* Marital Status
* Work Type
* Residence Type
* Average Glucose Level
* Body Mass Index (BMI)
* Smoking Status

### Target Variable

* Stroke

  * 0 = No Stroke
  * 1 = Stroke

The dataset presents a realistic healthcare classification problem with class imbalance, making it suitable for evaluating predictive models.

---

## Methodology

### Data Preprocessing

* Data cleaning
* Handling missing values
* Categorical variable encoding
* Feature scaling and normalization
* Train-test splitting

### Machine Learning Models

The following models were implemented and compared:

#### Logistic Regression

Used as a baseline model due to its interpretability and simplicity.

#### Random Forest Classifier

An ensemble learning algorithm utilizing multiple decision trees to improve prediction accuracy and reduce overfitting.

#### Support Vector Classifier (SVC)

A margin-based classifier designed to identify optimal decision boundaries in high-dimensional feature space.

#### XGBoost Classifier

A gradient boosting algorithm capable of capturing complex nonlinear relationships while maintaining strong predictive performance.

---

## Evaluation Metrics

Model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

These metrics were selected to provide a comprehensive assessment of both predictive accuracy and clinical usefulness.

---

## Results

| Model                           | Accuracy |
| ------------------------------- | -------- |
| Logistic Regression             | 78%      |
| Support Vector Classifier (SVC) | 78%      |
| XGBoost                         | 93%      |
| Random Forest                   | 100%*    |

*The Random Forest model achieved perfect performance on the test dataset, which may indicate potential overfitting.

### Key Findings

* XGBoost achieved the strongest balance between accuracy and generalization.
* XGBoost attained 93% accuracy and 99% recall for stroke cases.
* Logistic Regression provided strong interpretability but lower predictive performance.
* SVC demonstrated competitive sensitivity in detecting stroke cases.
* Ensemble methods significantly outperformed traditional linear approaches.

---

## Technologies Used

### Programming Language

* Python

### Machine Learning

* Scikit-Learn
* XGBoost

### Data Processing

* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Development Environment

* Jupyter Notebook

---

## Project Structure

stroke-prediction/
│
├── data/
│   ├── raw_data.csv
│   └── processed_data.csv
│
├── notebooks/
│   └── Stroke_Prediction.ipynb
│
├── models/
│   ├── logistic_regression.pkl
│   ├── random_forest.pkl
│   ├── svc.pkl
│   └── xgboost.pkl
│
├── src/
│   ├── preprocessing.py
│   ├── training.py
│   ├── evaluation.py
│   └── visualization.py
│
├── outputs/
│   ├── confusion_matrices/
│   ├── metrics/
│   └── figures/
│
├── requirements.txt
├── README.md
└── main.py

---

## Conclusion

The comparative analysis demonstrates that ensemble learning approaches provide superior predictive performance for stroke risk prediction. Among the evaluated models, XGBoost emerged as the most practical solution due to its combination of high accuracy, strong recall, scalability, and resistance to overfitting. These findings highlight the potential of machine learning-driven decision support systems in healthcare and preventive medicine.

---

## Authors

Phronesis Research Group

CSCD613 – Machine Learning with Big Data Analytics

