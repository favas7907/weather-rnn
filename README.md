# Weather Forecasting using Vanilla RNN

This project implements a **Recurrent Neural Network (RNN)** using PyTorch to predict the next day's weather based on historical data.

## Overview

* Preprocessed historical weather dataset
* Converted data into time-series sequences (past 7 days → next day prediction)
* Built and trained a **vanilla RNN model**
* Evaluated performance using regression metrics
* Visualized predictions against actual values

## Model Architecture

* Input: Sequence of past 7 days (multiple weather features)
* RNN Layer: `nn.RNN` with hidden size 64
* Output Layer: Fully connected (`Linear`) layer
* Loss Function: Mean Squared Error (MSE)
* Optimizer: Adam

## Files

* `weather_rnn_forecasting_rnn.ipynb` – Main implementation notebook


## How to Run

1. Open the notebook in **Google Colab** or Jupyter Notebook
2. Upload the dataset when prompted
3. Ensure the dataset includes a `date` column and numerical weather features
4. Run all cells sequentially

## Evaluation Metrics

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)

## Output

* Actual vs Predicted values plot
* Training loss curve
* Predicted value for the next day

## Notes

* This implementation uses a **vanilla RNN (nn.RNN)** — no GRU or LSTM
* Missing values are handled using forward fill
* Data is normalized using MinMaxScaler
* Sequence length is fixed at 7 days
