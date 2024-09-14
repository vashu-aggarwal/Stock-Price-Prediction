# Stock Price Prediction using LSTM Neural Networks

## Overview
This project predicts stock prices using a Long Short-Term Memory (LSTM) neural network. The model is trained on historical stock data sourced from Yahoo Finance, with the goal of forecasting future stock prices. The project includes both the prediction model and a simple web app built with Streamlit to visualize the results.

## Features
Predict stock prices using LSTM model.
Visualize moving averages (MA50, MA100, MA200).
Compare actual stock prices with predicted prices.
User-friendly web interface using Streamlit.
Data
Source: Yahoo Finance
Stock: Google (GOOG) (or any stock symbol entered by the user)
Date range: 2010-01-01 to 2023-01-01

## Dependencies
Python 3.x
Libraries:
numpy
pandas
matplotlib
yfinance
keras
tensorflow
streamlit
sklearn

## LSTM Model Architecture
4 LSTM layers with 50, 60, 80, and 120 units, each followed by a Dropout layer to prevent overfitting.
The model is trained to predict stock prices based on the last 100 days of stock data.

## How to Run
1. Clone the repository
bash
Copy code
git clone https://github.com/your-username/your-repository-name.git
2. Install dependencies
bash
Copy code
pip install -r requirements.txt
3. Train the LSTM model
Run the stock_price_prediction.py script to train the model and visualize stock trends.

bash
Copy code
python stock_price_prediction.py
4. Launch the web app
Run the following command to start the Streamlit web app.

bash
Copy code
streamlit run stock_price_webapp.py
5. Enter the Stock Symbol
In the web app, enter any valid stock symbol (e.g., GOOG) and visualize the stock's historical data, moving averages, and price predictions.

## Results
The model predicts future stock prices with reasonable accuracy, and the web app provides a comparison between predicted prices and actual historical prices.
Screenshots
Stock Data Visualization: Visualizes the stock prices with MA50, MA100, and MA200.

Price Prediction: Compares predicted prices vs. actual prices.

## Model Training
The model was trained for 50 epochs using the Adam optimizer and Mean Squared Error (MSE) as the loss function. It predicts the stock price for the next day based on the last 100 days of data.

## Conclusion
This project demonstrates how LSTM networks can be used for time-series forecasting. While the model shows promising results, improvements could be made by fine-tuning the network architecture or incorporating more features into the data.
