# 4. Develop an LSTM-based model for time-series forecasting using stock price, weather, or sales datasets.

## 1. Project Overview

This project implements a **Long Short-Term Memory (LSTM)** neural network for predicting Apple's (AAPL) stock closing prices using historical stock market data.

The model learns patterns from previous stock prices and predicts future closing prices using time-series forecasting.

## 2. Objectives

- Collect historical stock market data.
- Perform data preprocessing and normalization.
- Create sequential training and testing datasets.
- Implement an LSTM-based prediction model.
- Evaluate prediction performance using RMSE and MAE.
- Forecast the next day's closing price.

## 3. Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- yfinance
- Google Colab

## 4. Dataset

**Apple (AAPL) Historical Stock Data**

- Source: Yahoo Finance
- Time Period: January 2015 – December 2024
- Total Records: 2,516
- Features: Open, High, Low, Close, Adjusted Close, Volume

The closing price is selected as the primary feature for prediction.

## 5. Model Architecture

The project uses a stacked LSTM architecture.

**Workflow:**

Historical Stock Data → Data Normalization → Sequence Generation → LSTM Layers → Dense Layers → Predicted Stock Price

The model consists of:
- First LSTM layer with 50 units.
- Dropout layer (0.2).
- Second LSTM layer with 50 units.
- Dropout layer (0.2).
- Dense layer with 25 neurons.
- Output layer with 1 neuron.

## 6. Model Configuration

| Parameter | Value |
|---|---|
| Model | Stacked LSTM |
| Time Steps | 60 |
| Learning Rate | Adam (default) |
| Batch Size | 32 |
| Epochs | 20 |
| Dropout | 0.2 |
| Loss Function | Mean Squared Error |

## 7. Evaluation Metrics

The model is evaluated using:

- **RMSE:** Root Mean Squared Error.
- **MAE:** Mean Absolute Error.

### Results

| Metric | Value |
|---|---:|
| RMSE | 6.0581 |
| MAE | 4.7102 |

The actual and predicted stock prices are visualized using Matplotlib to analyze model performance.

## 8. Next-Day Prediction

The trained model uses the previous 60 days of stock prices to forecast the next day's closing price.

**Sample Output:**

```text
Predicted next day's closing price: 246.0237
```

## 9. Conclusion

The project demonstrates the application of LSTM networks for stock price forecasting. By learning temporal patterns from historical stock data, the model generates future price predictions. RMSE and MAE are used to evaluate prediction accuracy.

## 10. How to Run

1. Open the notebook in Google Colab.
2. Install the required dependencies.
3. Execute the notebook cells sequentially.
4. Download historical stock data using yfinance.
5. Train and evaluate the LSTM model.
6. Generate the next-day stock price prediction.

**Task:** Time-Series Forecasting  
**Dataset:** Apple (AAPL) Stock Data  
**Model:** LSTM  
**Framework:** TensorFlow / Keras
