# Walmart Stock Price Movement Estimation 🛒📊

A predictive modeling project using **Linear Regression** to estimate the continuous future stock price of Walmart (WMT) using 50+ years of historical market data.

## Project Overview
This project was built to fulfill the Predictive Modeling assignment requirements. It utilizes a **Linear Regression** algorithm from `scikit-learn` to estimate next-day closing prices based on engineered time-series indicators.

## Dataset
* **Source:** Kaggle (Walmart Stock Data 1972–2025)
* **Type:** Publicly available real-world time series dataset covering daily Open, High, Low, Close, and Volume records.

## Methodology & Implementation
1. **Data Preprocessing:** Standardized dates, ordered chronologically, and removed missing values.
2. **Feature Engineering:** Derived technical indicators including:
   * 20-Day & 50-Day Simple Moving Averages (SMA)
   * Daily Percentage Returns
3. **Model Training:** Fit a Scikit-Learn `LinearRegression` model using an 80/20 chronological train/test split.
4. **Evaluation:** Assessed regression accuracy using Root Mean Squared Error (RMSE) and R-squared ($R^2$) score.

## Results
The model demonstrated exceptional predictive accuracy on the test set:
* **Root Mean Squared Error (RMSE):** $0.62
* **R-squared ($R^2$) Score:** 0.9990

## Visualization
Below is the scatter plot with the regression line comparing the actual vs. predicted next-day closing prices.

![Actual vs Predicted Prices](visualization.png)

## Tech Stack
* Python | Scikit-Learn | Pandas | NumPy | Matplotlib | Seaborn
