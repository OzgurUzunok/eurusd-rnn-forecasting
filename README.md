# Recurrent Neural Network Model for EUR/USD Price Prediction

This project develops a SimpleRNN model to forecast the hourly closing prices of the Euro/USD currency pair using historical data. The notebook includes data preprocessing, model building, iterative multi-step forecasting, and performance evaluation.

## Tools & Libraries
- Python
- TensorFlow / Keras
- NumPy, Pandas
- Matplotlib (for visualizations)
- TraderMade API (for real-time data)

## How to Run
1. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the notebook `eurusd_rnn_forecasting.ipynb` in Jupyter or Colab.
3. API key from TraderMade is required to fetch live data.

## Results
- Best MSE achieved: **0.0008243834046896665**
- Best architecture: Single-layer SimpleRNN with 16 neurons.
- Observations: The model effectively tracks the immediate past but struggles to detect trend reversals. Multi-step predictions tend to converge toward the initial forecast, capturing general trend direction but not identifying reversals.

## Future Improvements
- Incorporate additional features (volume, momentum, technical indicators).
- Experiment with deeper architectures (LSTM, GRU).
- Implement validation and cross-validation for more robust performance.
