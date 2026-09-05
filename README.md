# Personal Habit Drift Detection and Forecasting System

A machine learning-based system that analyzes daily lifestyle habits, detects behavioral changes, predicts future habit trends, and provides early warnings and recommendations.

## 📌 Project Overview

Traditional habit trackers mainly record daily activities. This project goes further by identifying whether a person's habits are **improving, stable, or declining**.

The system analyzes factors such as:

* Sleep
* Study/Work
* Exercise
* Screen Time
* Mood
* Stress
* Productivity
* Water & Caffeine Intake

## 🔄 System Workflow

```text
Daily Habit Data
      ↓
Data Preprocessing
      ↓
Habit Score
      ↓
Drift Score
      ↓
ML Model
      ↓
Drift Status
      ↓
Early Warning
      ↓
Future Forecast
      ↓
Explanation & Recommendation
```

## 🧮 Habit & Drift Score

A **Habit Score (0–100)** is calculated from daily behavioral factors.

The **Drift Score** measures the change from the previous day's Habit Score:

```text
Drift Score = Today's Habit Score - Previous Day's Habit Score
```

* Positive → Improving
* Near Zero → Stable
* Negative → Declining

## 🤖 Machine Learning

The project compares multiple regression models:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor

**Gradient Boosting Regressor** was selected as the final model based on the evaluation results.

### Evaluation Metrics

* MAE
* MSE
* RMSE
* R² Score

## 📊 Key Features

* Daily habit analysis
* Personal baseline calculation
* Habit drift detection
* Improving/Stable/Declining classification
* Early warning system
* Future Drift Score forecasting
* Feature importance analysis
* Personalized recommendations
* Habit trend visualization

## 🛠️ Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Joblib
* Google Colab / Jupyter Notebook

## 📁 Project Structure

```text
Personal-Habit-Drift/
│
├── data/
│   └── habit_dataset_final.csv
├── models/
│   └── habit_drift_model.pkl
├── notebooks/
│   └── habit_drift_engine.ipynb
├── README.md
└── requirements.txt
```

## ⚠️ Limitations

* Dataset size is limited.
* Some data is self-reported.
* Habit score ranges are predefined.
* Current forecasting is relatively simple.

## 🔮 Future Improvements

* Larger dataset
* Automatic personal baseline learning
* Advanced time-series models such as LSTM
* SHAP-based explanations
* Real-time web dashboard
* Wearable data integration

## 🎓 Purpose

This project was developed as an academic machine learning project to demonstrate **behavioral analysis, regression, drift detection, forecasting, and explainable recommendations**.

> **Track → Detect → Predict → Explain → Improve**
