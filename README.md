# Temperature Forecasting with Deep Learning

## Overview
Implemented a temperature forecasting model using deep learning techniques to predict future temperature values based on historical data.

## Data Processing
- Processed temperature data recorded every 10 minutes, resulting in 144 data points per day and 1,440 for the first 10 days, used for training and forecasting.
- Used a sliding window approach to predict future temperatures while preserving temporal dependencies.
- Created training (200,000 samples), validation (100,000 samples), and test sets for model evaluation.

## Model Development and Performance
- Started with a common-sense baseline model (Test MAE: 2.62), but fully connected (Test MAE: 2.66) and CNN models failed due to the loss of temporal order.
- Improved forecasting by using an LSTM model (Test MAE: 2.60, achieving a 0.76% improvement over FC).
- Further optimized performance with dropout regularization, reducing Test MAE to 2.47 (5.72% improvement over the baseline).

