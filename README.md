# Project Overview

## Project Name
Financial Time Series Analysis and Forecasting

## Aim
The aim of this project is to analyze historical stock price data and build a time series forecasting model to predict future stock prices. The focus is on using statistical time series models to understand patterns, trends, and make informed predictions for financial decision-making.

## Tools Used
- Python
- Pandas, NumPy, Matplotlib, Seaborn for data analysis and visualization
- Statsmodels for time series analysis and modeling
- pmdarima for automatic ARIMA model selection
- scikit-learn for train-test split and performance evaluation
- yfinance for fetching historical stock price data from Yahoo Finance

## Process
1. **Data Collection:**
   - Historical stock price data for the chosen stock (e.g., Adani Ports) is fetched from Yahoo Finance using the `yfinance` library.

2. **Exploratory Data Analysis (EDA):**
   - The data is explored through summary statistics, visualizations, and decomposition to understand its characteristics and identify any patterns.

3. **Stationarity Check:**
   - Stationarity of the time series is checked using the Dickey-Fuller test, and necessary transformations are applied to achieve stationarity.

4. **Model Selection:**
   - ARIMA and SARIMAX models are explored for time series modeling.
   - The `auto_arima` function from `pmdarima` is used to automatically select the optimal hyperparameters for the ARIMA model.

5. **Model Training and Evaluation:**
   - The selected model (e.g., ARIMA(3, 1, 2)) is trained on the training dataset and evaluated on a separate test dataset.
   - Performance metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE) are calculated.

6. **Results Interpretation:**
   - The results of the model, including coefficients, statistical tests, and diagnostics, are interpreted to understand the model's effectiveness and any potential issues.

## Findings
- The SARIMAX (ARIMA(3, 1, 2)) model has been successfully fitted to the financial time series data.
- The model shows promising results in terms of log likelihood, AIC, BIC, and diagnostic tests.
- Further analysis and refinement may be needed to optimize and improve the forecasting accuracy.

Feel free to explore the notebooks and scripts in the repository for a detailed step-by-step walkthrough of the analysis and modeling process.
