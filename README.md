# ✈️ Airline Passenger Forecasting using ARIMA & SARIMA

## Project Overview
This project focuses on **forecasting airline passenger traffic** using **Time Series Analysis** techniques.  
We use the famous **Airline Passengers dataset**, which contains the number of international airline passengers from **1949 to 1960**.  
The main objective is to **analyze historical data**, make the series **stationary**, and **predict future passenger counts** using **ARIMA** and **SARIMA** models.

---

## Key Features
- Perform **Exploratory Data Analysis (EDA)** on airline passenger data.
- Check **stationarity** using:
  - Rolling Mean & Standard Deviation
  - Augmented Dickey-Fuller (ADF) Test
- Apply **log transformation** and **rolling mean differencing** to make data stationary.
- Build and train **ARIMA** and **SARIMA** models.
- Forecast **future passenger trends** for **2 years** and **5 years**.
- Visualize predictions vs actual trends.

---

## 📂 Dataset
- **File**: `airline_passengers.csv`
- **Rows**: 145  
- **Columns**:
  - `Month` → Date column
  - `Thousands of Passengers` → Monthly passenger count
- **Duration**: **January 1949 → December 1960**
- **Source**: Commonly available time series dataset used in forecasting tutorials.

---

## 🧠 Concepts Covered
### 1. Time Series Stationarity Check
- **Before Transformation**:
  - Rolling mean & standard deviation **not constant**
  - ADF p-value ≈ **0.99** → **Non-stationary**
- **After Log Transformation + Rolling Differencing**:
  - ADF p-value ≈ **0.02** → **Stationary** ✅

### 2. ARIMA & SARIMA Models
- **ARIMA (Auto-Regressive Integrated Moving Average)**:
  - Selected using PACF & ACF plots.
  - **Order (p, d, q) = (2, 0, 3)**
- **SARIMA (Seasonal ARIMA)**:
  - Added seasonality: `(2, 0, 3, 12)`

### 3. Forecasting
- Forecasted for:
  - **24 months** (2 years)
  - **60 months** (5 years)
- Predictions plotted alongside historical data.

---

## 📊 Visualizations
- Rolling Mean & Standard Deviation
- PACF & ACF Plots
- ARIMA vs Actual Data
- SARIMA vs Actual Data
- 5-Year Forecast Trend
