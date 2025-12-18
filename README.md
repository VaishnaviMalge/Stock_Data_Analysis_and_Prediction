# Stock Data Analysis and Prediction

## Overview

Analyze the historical data of TCS stock to gain insights into stock behavior, identify trends, and forecast future stock prices.

## Data Preparation

#### Dataset:

Raw features: Date, Open, High, Low, Close, Volume

#### Cleaning Steps:
- Handled missing values
- Removed duplicates
- Dropped irrelevant columns like dividends and stock splits

2. Feature Engineering

Derived features used for modeling:

- Prev_Close (previous day’s close)

- 50-day and 200-day moving averages (MA50, MA200)

- Range (High - Low)

- Date-based features: Month, Day_of_Week

3. Exploratory Data Analysis (EDA)

- Stock shows increasing volatility over time.

- Open, High, Low strongly correlate with Close.

- Volume provides context for short-term market events.

- Visualizations include line charts, correlation heatmaps, and trend analysis.

4. Models and Evaluation

- Models tried: Linear Regression, Ridge Regression, Random Forest, Gradient Boosting, XGBoost, and ARIMA(time-series model).

- Evaluation Metrics: RMSE, MAE, MSE, R²

### Findings:

- Linear and Ridge Regression performed best (R² ≈ 0.9999, lowest RMSE).

- Tree-based models captured non-linear patterns but had slightly higher errors.

- ARIMA provided forecasts but did not outperform regression models on this dataset.

## Learnings

- Comparing and evaluating multiple machine learning models using multiple metrics (RMSE, MAE, MSE, R²) for stock price prediction.

- Understanding time-series forecasting using ARIMA.


## Future Enhancements

- Incorporate a dashboard or app for visualization and predictions.

- Automate dataset updates using stock APIs for real-time predictions.

- Explore additional time-series models like SARIMA or Prophet.


**Note**
This README content was assisted by AI for clarity and structure; all project work, analysis, and results are fully authentic.
