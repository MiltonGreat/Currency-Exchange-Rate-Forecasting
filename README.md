# Currency Exchange Rate Forecasting

![screenshot-localhost_8888-2025 03 31-15_59_14](https://github.com/user-attachments/assets/57abf186-558e-4b98-80d7-dc37e1fa7a2e)

### Project Overview

This project explores forecasting currency exchange rates using two different time-series modeling approaches:

- SARIMA (Seasonal AutoRegressive Integrated Moving Average) – A statistical method that captures trends and seasonality in historical exchange rate data.

- LSTMs (Long Short-Term Memory networks) – A deep learning approach capable of learning complex temporal dependencies in forex movements.

By comparing these models, the goal is to improve the accuracy of exchange rate predictions, which is crucial for traders, investors, and policymakers.

### Dataset

The dataset consists of daily exchange rates from 2000 to 2019 for major currencies, including USD, EUR, GBP, JPY, and others. The data includes:

- Date (timestamp)
- Currency Pair (e.g., USD/EUR)
- Exchange Rate (historical price movements)

### Methodology

1. SARIMA Model (Statistical Approach)
- Identified seasonality and trends in exchange rate data.
- Plotted ACF & PACF to determine SARIMA parameters.
- Trained a SARIMA model on historical data and forecasted future values.
- Evaluated performance using RMSE (Root Mean Squared Error).

2. LSTM Model (Deep Learning Approach)
- Normalized data for deep learning compatibility.
- Created sequences of past exchange rate data to predict future values.
- Built an LSTM network using TensorFlow/Keras.
- Trained the model and evaluated forecast accuracy.

### Results & Evaluation

SARIMA Model Performance:
- Captured seasonal trends in exchange rates.
- RMSE: 0.0486 – Moderate accuracy but lacks adaptability to sudden market shocks.

LSTM Model Performance:
- Better at capturing non-linear relationships in forex movements.
- Outperformed SARIMA in capturing short-term fluctuations.
- Computationally expensive but provided more flexible predictions.

### Key Takeaways

- SARIMA is effective for trend-based forecasting but lacks adaptability to sudden market changes.
- LSTM networks perform better in capturing short-term fluctuations but require more data and tuning.
- Combining SARIMA with deep learning (Hybrid Models) could improve forecasting accuracy.

### Future Work

- Hybrid Models: Combining SARIMA’s statistical power with LSTM’s deep learning capabilities.
- Macroeconomic Data: Incorporating factors like GDP, interest rates, and inflation to improve predictive accuracy.
- Real-Time Forecasting: Implementing a system to update forecasts using live forex data.

### Conclusion

This project demonstrates that time-series forecasting is essential for financial markets. While SARIMA provides a good baseline, LSTMs are better suited for capturing short-term fluctuations. Future improvements should explore hybrid models and macroeconomic integrations to enhance predictive accuracy.

### Source

![Forex Exchange Rates Since 2004 from Kaggle](https://www.kaggle.com/datasets/asaniczka/forex-exchange-rate-since-2004-updated-daily)


