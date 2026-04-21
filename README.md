# USD/TRY Exchange Rate Forecasting with ARIMA

This project analyzes the historical trends of the **USD/TRY** exchange rate and provides a 3-month forecast using the **ARIMA (Autoregressive Integrated Moving Average)** model.

## 📊 Overview
The goal of this study is to model the exchange rate dynamics and predict future values based on monthly historical data.

## 🛠️ Methodology
* **Data Source:** Monthly USD/TRY data (2010 - 2026) retrieved via the `yfinance` library.
* **Pre-processing:** Logarithmic transformation and first-differencing were applied to ensure **stationarity**.
* **Model Selection:** ARIMA(1,0,1) was selected as the optimal model based on **AIC (Akaike Information Criterion)** values.
* **Diagnostics:** Residual analysis was performed using Ljung-Box and normality tests to ensure model reliability.

## 📈 Key Findings
* The series became stationary after logarithmic differencing, confirmed by the **ADF Test**.
* The model effectively captures the underlying trend, and residuals behave like **White Noise**.
* A 3-month upward trend is projected for the USD/TRY pair.

## 💻 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Statsmodels, Matplotlib, yfinance
