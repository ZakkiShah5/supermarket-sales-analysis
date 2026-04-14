# Supermarket Sales Analysis (EDA + Machine Learning + Time Series)

## 📌 Overview

This project performs Exploratory Data Analysis (EDA), Machine Learning, and Time Series Forecasting on a supermarket sales dataset to uncover patterns, understand customer behavior, and predict future sales.

---

## 🎯 Objectives

* Analyze sales distribution and customer behavior
* Identify top-performing product categories
* Explore relationships between features
* Predict total sales using regression models
* Forecast future sales using time series analysis

---

## 📂 Dataset

* File: `data.csv`
* Contains transaction-level supermarket sales data
* Key features include:

  * Product line
  * Sales
  * Quantity
  * Unit price
  * Payment method
  * Gender
  * Rating
  * Date

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Statsmodels

---

## 🔍 Exploratory Data Analysis (EDA)

Steps performed:

* Data loading and inspection
* Handling missing values (dropped nulls)
* Statistical summary (`describe`, `info`)
* Category-wise analysis
* Distribution plots (histograms)
* Correlation analysis (heatmap)

### 📊 Key Visualizations

* Product line distribution
* Sales histogram
* Correlation heatmap
* Sales by category
* Gender distribution
* Payment method distribution

---

## 📈 Key Insights

* **Fashion & Accessories** generated the highest number of sales
* **Food & Beverages** contributed significantly to revenue
* Sales distribution is **right-skewed** (more low-value transactions)
* Female customers made more purchases than males
* **E-wallet and Cash** are the most commonly used payment methods

---

## 🤖 Machine Learning

### 1️⃣ Sales Prediction

* Model: Linear Regression
* Features used:

  * Quantity
  * Tax
  * Unit Price

📌 Goal: Predict total sales amount

👉 Result: Moderate performance (basic linear relationship captured)

---

### 2️⃣ Customer Rating Prediction

* Models:

  * Linear Regression
  * Random Forest Regressor

📌 Goal: Predict customer satisfaction

👉 Result: Low accuracy → ratings are harder to predict from available features

---

## ⏱️ Time Series Analysis

### Steps:

* Converted `Date` column to datetime
* Resampled data to daily sales
* Applied ARIMA model

### Model Used:

* ARIMA(5,1,0)

### 📉 Findings:

* No strong trend or seasonality
* Sales show high randomness
* Forecast converges to mean value

---

## 📊 Results Summary

* EDA revealed strong business insights
* ML models showed limited predictive power
* Time series forecasting indicates random sales behavior

---

## 🚀 How to Run

```bash
pip install pandas matplotlib seaborn scikit-learn statsmodels
```

Run the notebook or script:

```bash
python your_script_name.py
```

---

## 📁 Project Structure

```
project/
│
├── data.csv
├── eda.ipynb
├── README.md
```

---

## ⚠️ Limitations

* Small dataset → weak time series patterns
* Limited features for accurate ML predictions
* No hyperparameter tuning performed

---

## 🔮 Future Improvements

* Feature engineering
* Try advanced models (XGBoost, LSTM)
* Larger dataset for better forecasting
* Hyperparameter tuning

---

## 👤 Author

Zakki Shah
