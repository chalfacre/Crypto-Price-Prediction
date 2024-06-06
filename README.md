# Crypto-Price-Prediction
 Uses LSTM model to predict BTC price

The provided code uses a Long Short-Term Memory (LSTM) neural network model to predict future cryptocurrency prices based on historical data.

This code retrieves historical price data for Bitcoin (BTC) against USD from Yahoo Finance, starting from January 1, 2020, to the current date.

The closing prices are normalized to a range between 0 and 1 using MinMaxScaler. This is a common preprocessing step for neural networks to help improve their performance.

The model consists of three LSTM layers, each with 50 units, followed by Dropout layers to prevent overfitting.
The final Dense layer outputs a single value, which is the predicted price.
The model is compiled with the Adam optimizer and mean squared error loss function, and trained for 25 epochs with a batch size of 32.

The model uses the test sequences to predict future prices.
The predicted prices are then inverse-transformed back to the original scale.
