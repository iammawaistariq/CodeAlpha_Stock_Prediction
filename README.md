# Amazon Stock Price Prediction Using LSTM

## Overview

This project aims to predict Amazon's stock price using historical data and an LSTM (Long Short-Term Memory) neural network model. The dataset includes stock price data from Yahoo Finance, and the model is trained to forecast future prices based on historical trends.

## Project Structure

- **Data Collection**: Retrieves historical stock price data from Yahoo Finance.
- **Data Preprocessing**: Scales the data and prepares it for training.
- **Model Building**: Constructs and compiles an LSTM model for time series forecasting.
- **Model Training**: Trains the model on the prepared data.
- **Prediction**: Uses the trained model to predict stock prices on new data.
- **Evaluation**: Calculates the Mean Squared Error (MSE) to evaluate prediction accuracy.
- **Visualization**: Plots actual vs. predicted stock prices.

## Data Collection:
* Historical stock data is downloaded from Yahoo Finance using the yfinance library.

## Data Preprocessing:
* Extracts the 'Close' price.
* Scales the data using MinMaxScaler.
* Prepares the dataset with a window of 60 timestamps for training.

## Model Building:
* Constructs an LSTM model with two LSTM layers and two Dense layers.
* Compiles the model using the Adam optimizer and mean squared error loss function.

## Model Training:
* Trains the model on the training data for 20 epochs with a batch size of 32.

## Prediction:
* Retrieves new test data and scales it.
* Uses the trained model to predict future prices.
* Inverse transforms the scaled predictions to obtain actual price values.

## Evaluation:
Calculates the Mean Squared Error (MSE) between the predicted and actual prices.

## Visualization:
Plots the actual vs. predicted stock prices for comparison.



