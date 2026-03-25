# 🌩️ Storm Formation Analysis using Feature Selection

> *Understanding atmospheric dynamics behind extreme rainfall events using data science and machine learning.*

---

## 🧭 Project Overview

This project investigates how key meteorological variables influence **storm formation**, using extreme rainfall as a storm proxy.

By leveraging long-term atmospheric observations from NASA POWER, the study combines **visual exploration, statistical feature selection, and machine learning models** to identify the most significant drivers of storm events in a coastal environment.

The goal is not just prediction — but **interpretability and insight into atmospheric behaviour.**

---

## 🎯 Objectives

* Examine temporal patterns in extreme rainfall
* Identify dominant atmospheric variables influencing storm formation
* Apply **filter and wrapper feature selection methods**
* Compare predictive performance across multiple ML models
* Derive interpretable conclusions from model behaviour

---

## 🌐 Dataset

* **Source:** NASA POWER API
* **Location:** Visakhapatnam, India 🌊
* **Time Span:** 2014 – 2024
* **Resolution:** Hourly Observations

### 🌦️ Meteorological Features

* Air Temperature
* Dew Point Temperature
* Wet Bulb Temperature
* Relative Humidity
* Specific Humidity
* Surface Pressure
* Wind Speed
* Wind Direction
* Precipitation

Storm events were defined using a **data-driven threshold based on the 95th percentile of precipitation**, ensuring focus on extreme rainfall rather than routine monsoon activity.

---

## 📐 Methodology

### ⚗️ Data Preparation

* Removed NASA metadata rows
* Converted missing value markers (`-999`)
* Created unified datetime index
* Structured dataset as time-series
* Engineered binary storm label

---

### 🌧️ Exploratory Data Analysis

* Rainfall distribution and skewness analysis
* Storm vs Non-storm feature comparisons
* Seasonal storm frequency patterns
* Extreme rainfall spike detection
* Correlation heatmaps

---

### 🧮 Feature Selection

#### 🔎 Filter Techniques

* Correlation Analysis
* Mutual Information
* Variance Threshold

#### 🔁 Wrapper Techniques

* Recursive Feature Elimination (RFE)
* Forward Feature Selection

### 🌬️ Key Influential Variables

* Specific Humidity
* Dew Point Temperature
* Relative Humidity
* Surface Pressure
* Wet Bulb Temperature
* Wind Speed

These variables collectively represent **moisture buildup, atmospheric instability, and low-pressure dynamics** commonly associated with storm systems.

---

## 📈 Model Training & Evaluation

Models Implemented:

* Logistic Regression
* Decision Tree
* Random Forest
* Gradient Boosting

Performance Metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

---

## 📊 Results

| Model               | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Random Forest       | 0.91     | 0.64      | 0.30   | 0.41     | 0.89    |
| Decision Tree       | 0.87     | 0.37      | 0.40   | 0.38     | 0.66    |
| Gradient Boosting   | 0.90     | 0.64      | 0.21   | 0.32     | 0.87    |
| Logistic Regression | 0.90     | 0.72      | 0.10   | 0.17     | 0.85    |

---

## 🧠 Key Insights

* Moisture-driven variables are the strongest predictors of extreme rainfall
* Low surface pressure shows consistent association with storm events
* Random Forest demonstrated the most balanced performance across evaluation metrics

---

## 🔮 Future Directions

* Address class imbalance using SMOTE / resampling strategies
* Perform advanced hyperparameter tuning
* Integrate additional instability indicators
* Develop real-time storm prediction dashboards

---

## 💻 Tech Stack

* Python
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn

---

## 🧑‍💻 Author

**Krishna Kireeti**

---

## 🌟 Acknowledgements

* NASA POWER for providing open meteorological datasets
* Academic guidance through Applied Data Science coursework

---
