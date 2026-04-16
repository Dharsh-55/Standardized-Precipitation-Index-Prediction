# 🌧️ Drought Prediction using Deep Learning (SPI-Based Analysis)

## 📌 Overview

This project focuses on predicting **meteorological drought conditions** using deep learning techniques applied to the **Standardized Precipitation Index (SPI)**.

The study leverages **120 years of rainfall data** from Coimbatore, India, to model drought patterns across multiple time scales. Advanced deep learning architectures are used to improve prediction accuracy and reliability compared to traditional statistical methods.

---

## 🎯 Objectives

* Predict drought severity using SPI at multiple time scales
* Compare performance of different deep learning models
* Analyze short-term and long-term drought prediction accuracy
* Improve reliability of drought forecasting systems

---

## 🧠 Key Concepts

### 🔹 Standardized Precipitation Index (SPI)

SPI is a widely used indicator to quantify drought severity based on precipitation data.

SPI = \frac{X - \mu}{\sigma}

Where:

* (X) = precipitation
* (\mu) = mean precipitation
* (\sigma) = standard deviation

SPI values are computed across multiple time scales:

* Short-term: SPI-1
* Medium-term: SPI-3, SPI-6, SPI-9
* Long-term: SPI-12, SPI-24, SPI-48, Yearly

---

## 🚀 Models Implemented

* **LSTM (Long Short-Term Memory)**
* **Stacked LSTM (S-LSTM)**
* **Bidirectional LSTM (BiLSTM)**
* **Stacked BiLSTM (S-BiLSTM)**

These models are designed to capture temporal dependencies in rainfall data, especially long-range patterns.

---

## 📊 Dataset

* **Location:** Coimbatore, India
* **Duration:** ~120 years
* **Type:** Historical rainfall data
* **Preprocessing:**

  * Handling missing values
  * Normalization
  * SPI computation at multiple scales

---

## 📈 Results & Observations

* **Short-term (SPI-1):**

  * Low prediction accuracy
  * R² ≤ 0.11, high RMSE (~1.0)

* **Medium-term (SPI-3 to SPI-9):**

  * S-LSTM showed significant improvement
  * R² ≈ 0.62 to 0.89

* **Long-term (SPI-12 to SPI-24):**

  * S-BiLSTM achieved best performance
  * R² > 0.94
  * Strong ability to learn long-term dependencies

* **Yearly SPI:**

  * Weak predictions due to smoothing of short-term variability

---

## 🔍 Key Insights

* Stacked and bidirectional models outperform basic LSTM
* Long-term drought patterns are easier to model than short-term fluctuations
* Deep learning significantly improves SPI prediction accuracy
* Model interpretability and data variability remain key challenges

---

## 🏗️ Tech Stack

* **Programming Language:** Python
* **Libraries:**

  * TensorFlow / Keras
  * NumPy, Pandas
  * Scikit-learn
  * Matplotlib / Seaborn

---

## ▶️ Usage

1. Load the dataset
2. Compute SPI values for required time scales
3. Train deep learning models (LSTM variants)
4. Evaluate using R² and RMSE
5. Analyze predictions across different time scales

---

## 📊 Evaluation Metrics

* R² Score (Coefficient of Determination)
* RMSE (Root Mean Square Error)

---


