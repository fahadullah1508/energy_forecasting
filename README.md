# Task 3: Energy Consumption Time Series Forecasting

## Overview
Forecast short-term household energy usage using historical time-based patterns and compare multiple forecasting models.

## Objective
Build and compare ARIMA, Prophet, and XGBoost models for energy consumption forecasting.

## Dataset
- **Source:** UCI Machine Learning Repository - Household Power Consumption
- **Features:** Global active power, reactive power, voltage, intensity, sub-metering values
- **Frequency:** Minute-level data, resampled to hourly
- **Target:** Global Active Power (kilowatts)

## Approach
1. **Data Loading:** Downloaded and parsed time series data
2. **Data Cleaning:** Handled missing values, resampled to hourly frequency
3. **EDA:** Decomposed time series, analyzed seasonal patterns, ACF/PACF analysis
4. **Feature Engineering:** Created time-based features, lag features, rolling statistics, cyclical encodings
5. **Modeling:** Trained ARIMA, Prophet, and XGBoost models
6. **Evaluation:** Compared models using MAE, RMSE, and MAPE
7. **Visualization:** Plotted actual vs forecasted values

## Models Compared
- **ARIMA** - Classical time series model
- **Prophet** - Facebook's forecasting tool with seasonality handling
- **XGBoost** - Gradient boosting with engineered time features

## Files
- `Task3_Energy_Forecasting.ipynb` - Main analysis notebook

## Requirements
```
pandas, numpy, matplotlib, seaborn, statsmodels, prophet, xgboost, scikit-learn
```

## How to Run
1. Open the Jupyter notebook
2. Run all cells sequentially (dataset will auto-download)
3. Forecast visualizations and metrics will be displayed inline

## Key Insights
- Clear daily and weekly seasonal patterns in energy consumption
- XGBoost with engineered features provides competitive accuracy
- Prophet effectively captures multiple seasonalities
- 24-hour lag features are highly predictive
