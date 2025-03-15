# Netflix Stock Price Prediction Using Machine Learning
# Team Members
- Sai Nitish Gadde – 700758589
- Bhuma Kishore babu – 700752976
- Charith Reddy Putta - 700759727

## Project Overview
This project aims to predict Netflix's stock price using various machine learning models, including Linear Regression, Random Forest, XGBoost, ARIMA, and LSTM. The dataset consists of historical stock prices, and the models are trained and evaluated using key performance metrics.

## Dataset
- Data Source: `NFLX.csv`
- Features: Open, High, Low, Close, Volume, Adjusted Close, Technical Indicators (SMA, EMA, RSI, MACD, Lag Features)
- Target: Next day's Close price

## Data Preprocessing
- Converted 'Date' column to datetime format
- Computed technical indicators such as SMA, EMA, RSI, MACD
- Created lag features for time-series forecasting
- Scaled data using MinMaxScaler
- Split data into training (80%) and testing (20%)

## Models Implemented
1. **Linear Regression**
2. **Random Forest Regressor**
3. **XGBoost Regressor**
4. **ARIMA** (Time-Series Forecasting)
5. **LSTM Neural Network**

## Model Evaluation Results

| Model                    | MSE       | RMSE    | MAPE  |
|--------------------------|-----------|---------|-------|
| **Linear Regression**    | 170.4188  | 13.0545 | 1.53% |
| **Random Forest**        | 2907.7595 | 53.9236 | 6.01% |
| **XGBoost Regressor**    | 4401.3409 | 66.3426 | 7.48% |
| **ARIMA**                | 384.8935  | 19.6187 | 2.35% |
| **LSTM**                 | 1108.8858 | 33.2999 | 5.05% |

## LSTM Model Training Progress:
```
Epoch 1/20
Loss: 0.0534 - Val Loss: 0.0103
Epoch 2/20
Loss: 0.0079 - Val Loss: 0.0075
Epoch 3/20
Loss: 0.0055 - Val Loss: 0.0040
Epoch 4/20
Loss: 0.0052 - Val Loss: 0.0049
Epoch 5/20
Loss: 0.0049 - Val Loss: 0.0046
Epoch 6/20
Loss: 0.0045 - Val Loss: 0.0048
Epoch 7/20
Loss: 0.0041 - Val Loss: 0.0047
Epoch 8/20
Loss: 0.0037 - Val Loss: 0.0037
Epoch 9/20
Loss: 0.0044 - Val Loss: 0.0036
Epoch 10/20
Loss: 0.0041 - Val Loss: 0.0055
Epoch 11/20
Loss: 0.0039 - Val Loss: 0.0105
Epoch 12/20
Loss: 0.0037 - Val Loss: 0.0066
Epoch 13/20
Loss: 0.0032 - Val Loss: 0.0068
Epoch 14/20
Loss: 0.0035 - Val Loss: 0.0035
Epoch 15/20
Loss: 0.0033 - Val Loss: 0.0034
Epoch 16/20
Loss: 0.0030 - Val Loss: 0.0038
Epoch 17/20
Loss: 0.0026 - Val Loss: 0.0032
Epoch 18/20
Loss: 0.0029 - Val Loss: 0.0037
Epoch 19/20
Loss: 0.0023 - Val Loss: 0.0038
Epoch 20/20
Loss: 0.0023 - Val Loss: 0.0076
```

## Conclusion
- Linear Regression had the best performance with the lowest RMSE and MAPE.
- ARIMA performed well for time-series forecasting.
- LSTM model showed promising results but requires further tuning.

## Dependencies
- Python 3.11+
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn, XGBoost, Statsmodels
- TensorFlow, Keras

## How to Run
1. Upload `NFLX.csv` in Google Colab.
2. Run the provided notebook cells.
3. Evaluate results and visualize predictions.
