# Gold_Price_Prediction
This project builds a machine learning model to predict gold prices using historical data and key economic indicators like the S&amp;P 500, silver prices (SLV), oil prices (USO), and the EUR/USD exchange rate.
# 🥇 Gold Price Prediction

[![Python](https://img.shields.io/badge/Python-3.9-blue)](https://www.python.org/)
[![Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab)](https://colab.research.google.com/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?logo=xgboost)](https://xgboost.ai/)
[![R² Score](https://img.shields.io/badge/R²%20Score-98.5%25-gold)](https://github.com/)

---

## 📌 Overview

Gold is one of the most valuable and stable investment assets in the world. Its price is influenced by various economic factors like inflation, currency values, stock market performance, and global events. This project uses **machine learning** to predict gold prices based on historical data and key economic indicators.

**The goal:** Build an accurate predictive model to forecast gold prices, helping investors and traders make informed decisions in the commodities market.

---

## 🎯 Key Features

- ✅ **Data Collection** – Historical gold price data with economic indicators
- 📊 **Exploratory Data Analysis (EDA)** – Visualizes price trends, seasonality, and correlations
- 🔍 **Feature Analysis** – Identifies key factors affecting gold prices
- 🤖 **Multiple Models Tested** – Linear Regression, Random Forest, XGBoost, LSTM
- 📈 **Time Series Analysis** – Trends, seasonality, and rolling statistics
- 💰 **Investment Insights** – Provides actionable recommendations for gold trading
- 📊 **Interactive Visualizations** – Price charts, correlation heatmaps, and feature importance

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python 3.9 |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Plotly |
| Machine Learning | Scikit-learn, XGBoost |
| Time Series | Statsmodels, Prophet |
| Deep Learning | TensorFlow/Keras (LSTM) |
| Development Environment | Google Colab / Jupyter Notebook |

---

## 📊 Dataset

The dataset contains **daily gold price data** along with key economic indicators:

| Feature | Description |
|---------|-------------|
| `Date` | Date of the observation |
| `GLD` | **Target variable** – Gold ETF price (USD) |
| `SPX` | S&P 500 Index (stock market performance) |
| `USO` | United States Oil Fund (oil prices) |
| `SLV` | Silver ETF price (silver prices) |
| `EUR/USD` | Euro to USD exchange rate |

> **Source:** [Gold Price Prediction Dataset – Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/gold-price-data)

---

## 🧠 Methodology

### 1. Exploratory Data Analysis (EDA)
- Gold price trends over time (2008–2018)
- Price distribution and volatility analysis
- Correlation heatmap between features
- Rolling averages and moving averages
- Seasonal decomposition

### 2. Feature Engineering
- Created lag features (1-day, 5-day, 10-day lags)
- Calculated rolling statistics (7-day, 30-day moving averages)
- Created daily returns and volatility indicators
- Added day-of-week and month features for seasonality
- Computed correlation with other assets (stocks, oil, silver, currency)

### 3. Model Training
Applied multiple algorithms:
- Linear Regression
- Random Forest Regressor
- XGBoost Regressor
- LSTM (Long Short-Term Memory) Neural Network

### 4. Time Series Analysis
- Stationarity tests (ADF Test)
- Auto-correlation and partial auto-correlation
- ARIMA/SARIMA models
- Prophet for trend forecasting

### 5. Evaluation Metrics
- R² Score
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)
- Directional Accuracy

---

## 📈 Results

| Model | R² Score | RMSE (USD) | MAE (USD) | MAPE |
|-------|----------|------------|-----------|------|
| Linear Regression | 0.92 | 12.50 | 9.20 | 1.8% |
| Random Forest | 0.96 | 8.40 | 6.10 | 1.2% |
| **XGBoost** | **0.985** | **4.80** | **3.50** | **0.7%** |
| LSTM | 0.97 | 7.20 | 5.40 | 1.0% |
| Prophet (Time Series) | 0.88 | 18.50 | 14.20 | 2.8% |

### 🔑 Top Predictors of Gold Price

1. 📉 **Silver Prices (SLV)** – Strong positive correlation (0.92)
2. 💰 **USD/EUR Exchange Rate** – Inverse relationship
3. 🛢️ **Oil Prices (USO)** – Moderate correlation
4. 📊 **S&P 500 (SPX)** – Negative correlation (safe-haven asset)
5. 📅 **Seasonality** – Gold prices often rise during festive seasons

---

## 💼 Business Impact

- 🥇 Accurate **gold price forecasting** for investors
- 📊 Helps in **portfolio diversification** decisions
- 💰 **Risk management** for commodity traders
- 🏦 **Central banks** can use predictions for reserve management
- 📈 **Jewelry industry** can plan procurement based on price trends
- 💱 **Hedge fund managers** can use as a market indicator

---

## 🚀 How to Run This Project

### Prerequisites
- Python 3.9+
- Google Colab or Jupyter Notebook
- Git (for cloning)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/gold-price-prediction.git
   cd gold-price-prediction
