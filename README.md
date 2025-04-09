# This project is part of a Data Science internship assignment focused on forecasting daily sales for different product families across multiple stores in Ecuador. The aim is to build a robust forecasting pipeline that can predict the next 15 days of sales after the last training date using various models and real-world influencing factors like oil prices, holidays, and promotions.

File	Description
train.csv-->	Historical sales data
test.csv-->	Data for final 15-day forecast
stores.csv-->	Store metadata (location, cluster, type)
oil.csv-->	Daily oil prices
holidays_events.csv-->	Information about holidays and events
forecast_15_day_output.csv	Final predicted sales for each store/family for 15 days
README.md	You are here


✅ Part 1: Data Processing & Feature Engineering
Merged data from multiple sources

Cleaned missing values (especially oil prices)

Created time-based, event-based, and rolling statistical features

Flagged holidays, promotions, paydays, and economic events

Included lag features for past sales behavior

Added store-level aggregation like average sales per type and top-selling families per cluster

✅ Part 2: Modeling, Forecasting, and Evaluation
Trained 3 models:

XGBoost (gradient boosting)

Random Forest

ARIMA (time series)

Evaluated using:

RMSE (Root Mean Squared Error)

MAPE (Mean Absolute Percentage Error)

R² Score

Visualized actual vs. predicted sales for model comparison

Forecasted the next 15 days of sales per store & family
