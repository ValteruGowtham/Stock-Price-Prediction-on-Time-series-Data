# Stock-Price-Prediction-on-Time-series-Data

This project uses a Long Short-Term Memory (LSTM) recurrent neural network (RNN) to predict the closing price of Reliance stock based on historical time-series data. Built with Keras and TensorFlow backend.

## Features
- Loads and preprocesses historical stock data from `RELIANCE.csv`.
- Scales features using `MinMaxScaler`.
- Uses 60-day lookback window to predict next day's closing price.
- Trains on 80% data, tests on 20% with RMSE evaluation.
- Forecasts next 30 days via autoregressive method.
- Visualizes predictions with Matplotlib.

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/yourusername/Stock-Price-Prediction-on-Time-series-Data.git
   cd Stock-Price-Prediction-on-Time-series-Data
   ```
   (Replace `yourusername` with your GitHub username.)

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

## Data
- `RELIANCE.csv`: Historical stock data for Reliance (columns: Date, Open, High, Low, Close, Volume).

## Requirements
Listed in `requirements.txt`:
- `numpy>=1.19.5`
- `pandas>=1.3.5`
- `matplotlib>=3.5.1`
- `scikit-learn>=1.0.2`
- `tensorflow>=2.5.0`

## Usage
1. Place `RELIANCE.csv` in the root directory.
2. Run the Jupyter notebook:
   ```
   jupyter notebook Stock_Price_Prediction.ipynb
   ```
3. Execute cells sequentially for data loading, model training, evaluation, and forecasting.

## License
MIT License. See [LICENSE](LICENSE) for details.
