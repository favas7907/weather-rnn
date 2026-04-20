# Weather Forecasting with RNN

This project uses a **vanilla Recurrent Neural Network (RNN)** to predict the next day's weather from historical weather data.

## Overview
- Load and preprocess weather data
- Create time-series sequences
- Train a vanilla RNN model
- Evaluate with MSE and MAE
- Plot actual vs predicted values

## Model
- Input: past 7 days of weather features
- Layer 1: `nn.RNN`
- Layer 2: Fully connected output layer
- Loss: Mean Squared Error
- Optimizer: Adam

## Files
- `weather_rnn_forecasting_rnn.ipynb` - main notebook
- `requirements.txt` - dependencies

## How to Run
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Upload your CSV file when prompted.
3. Make sure the dataset has a `date` column and weather columns such as temperature, humidity, rainfall, or related numeric features.
4. Run all cells.

## Results
The notebook prints:
- MSE
- MAE

It also shows:
- Actual vs predicted plot
- Training loss curve
- Next-day prediction

## Notes
- This version uses a **true RNN**, not GRU or LSTM.
- If your dataset has different column names, update the feature selection cell.