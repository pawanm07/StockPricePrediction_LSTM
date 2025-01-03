# Stock Price Prediction using LSTM

This project focuses on predicting stock prices and converting the predictions into Indian Rupees (INR) using a predefined conversion rate. The model utilizes Long Short-Term Memory  neural networks to predict future stock prices based on historical data. Additionally, interactive visualizations are created using Plotly to help visualize the predictions.

## Table of Contents
- Overview
- Requirements
- Installation
- Data
- Model Architecture
- Conversion to INR
- Interactive Visualization
- Usage
- Results
- License

## Overview
This project demonstrates the use of an LSTM model to predict stock prices and convert them from USD to INR. We provide an interactive visualization to track the performance of the model's predictions alongside real stock prices.

## Requirements
- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `plotly`
  - `yfinance`
  - `keras`
  - `tensorflow`

## Installation
- Clone the repository:
   ```bash
   git clone https://github.com/yourusername/stock-price-prediction-inr.git
   ```
## Data

- The stock data (e.g., AAPL.csv) needs to be added to the project using (yfinance) this library. You can use any stock dataset, but make sure it includes columns for the stock's closing prices.
## Model Architecture

#### The model uses the following layers:

1) Two LSTM layers:
- First LSTM layer with 50 units, returning sequences.
- Second LSTM layer with 50 units.
2) Two Dense layers:
- One Dense layer with 25 units.
- One Dense layer with 1 unit for the final prediction.
## Conversion to INR

To convert the USD prices to INR, we use a predefined exchange rate of 83. This is hardcoded to avoid real-time fetching of the exchange rate.

The conversion is applied to both the real stock prices and the model's predictions.

## Interactive Visualization

Plotly is used to create interactive graphs showing:

- The real stock prices in INR (Train dataset).
- The validation stock prices in INR (Valid dataset).
- The model's predictions in INR.
## Usage

1) Train the LSTM model with the provided dataset.
2) Convert the closing prices and predictions from USD to INR using the predefined exchange rate.
3) Visualize the stock prices and predictions using the interactive Plotly graph.
## Results

After training the model and converting the data to INR, the interactive graph shows:

- Real stock prices (Train) in INR.
- Validation stock prices in INR.
- Model's predictions in INR.

## PowerBI Dashboard
![PowerBI Dashboard Screenshot](https://github.com/pawanm07/CodeAlphaProject1/blob/main/OUTPUT.png)
