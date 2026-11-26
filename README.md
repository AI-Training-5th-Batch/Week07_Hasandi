# Week 7 – Time-Series Forecasting & Predictive Maintenance

## Project Overview

This project implements time-series forecasting for predictive
maintenance using daily machine vibration data.

The objective is to identify machine degradation, forecast future
vibration levels, and support proactive maintenance decisions before
critical thresholds are reached.

## Dataset

- Dataset: `machine_vibration.csv`
- One year of daily machine vibration observations
- Inspection threshold: 4.5 mm/s
- Stop threshold: 6.0 mm/s
- Weekly seasonality

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

## Forecasting Models

1. Seasonal Naive
2. Holt-Winters Exponential Smoothing
3. Gradient Boosting Regressor

## Implementation Steps

### Step 1 – Explore the Fleet

Visualize machine vibration levels and identify the degrading machine.

### Step 2 – Time-Based Train/Test Split

Split the historical data into 300 training observations and
65 testing observations without random shuffling.

### Step 3 – Three Forecasts

Implement Seasonal Naive, Holt-Winters and Gradient Boosting
forecasting models.

### Step 4 – Backtesting

Evaluate the forecasting models using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)

### Step 5 – The Extrapolation Trap

Generate 120-day future forecasts to compare the long-term
forecasting behaviour of Holt-Winters and Gradient Boosting.

### Step 6 – Predictive Maintenance Across the Fleet

Forecast machine vibration over a 180-day horizon and calculate
days until inspection and stop thresholds are reached.

Classify machines into:

- URGENT
- watch
- healthy

### Step 7 – Retraining Policy

- Scheduled weekly retraining
- Error-triggered retraining
- Immediate retraining after machine repair

### Step 8 – Final Report

Summarize the methodology, forecasting results, extrapolation
findings and maintenance recommendations.

Status: Pending completion.

## Installation

Install the required Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn statsmodels jupyter
```

## How to Run

1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install the required libraries.
4. Place `machine_vibration.csv` in the project directory.
5. Open `week7_predictive_maintenance.ipynb`.
6. Run all notebook cells sequentially.

## Project Structure

```text
Week7_TimeSeries/
├── .gitignore
├── README.md
├── machine_vibration.csv
└── week7_predictive_maintenance.ipynb
```

## Conclusion

This project demonstrates the importance of selecting a forecasting
model based on both prediction accuracy and long-term forecasting
behaviour.

Trend-aware forecasting supports predictive maintenance by
identifying potential threshold crossings and enabling proactive
maintenance planning.

```

```
