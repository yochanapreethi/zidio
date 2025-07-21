## Stock Market Forecasting using Time Series Models

This project was developed during a data science internship at Zidio and focuses on forecasting stock prices using time series models. The analysis was performed on Apple Inc. (AAPL) using historical stock market data sourced from Kaggle.

### Objective

- Apply and compare statistical and deep learning models for time series forecasting.
- Evaluate models using real-world financial data.
- Identify the best-performing method for predicting stock prices.
- 
### Dataset

- **Source:** [Kaggle - Stock Market Dataset](https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset)
- **Stock Used:** AAPL (Apple Inc.)
- **Features:** Date, Open, High, Low, Close, Adjusted Close, Volume
- **Preprocessing:** Null handling, date formatting, filtering NASDAQ non-ETFs

### Tools and Libraries

Python, Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Facebook Prophet, TensorFlow, Keras, Scikit-learn

### Models Implemented

- Naive Forecast (baseline)
- ARIMA (5,2,2)
- SARIMA (1,2,1)(1,0,1,7)
- Facebook Prophet
- LSTM Neural Network

### Evaluation Summary

| Model        | MSE     | MAE     | RMSE    |
|--------------|---------|---------|---------|
| ARIMA        | 83.16   | 5.50    | 9.12    |
| LSTM         | 83.24   | 5.49    | 9.12    |
| SARIMA       | 83.36   | 5.51    | 9.13    |
| Naive        | 115.74  | 7.76    | 10.76   |
| Prophet      | 32046.5 | 178.94  | 179.02  |

### Key Takeaways

- ARIMA and LSTM were the most effective models.
- Prophet did not generalize well for high-frequency financial data.
- Classical models can match deep learning in certain use cases with proper tuning.
