# Cryptocurrency Dataset Prediction

This project contains tools and analyses for predicting cryptocurrency prices and volatility using machine learning and statistical models.

## Project Structure

- **`Volatility Prediction.ipynb`**: A comprehensive notebook for analyzing and forecasting financial volatility.
    - **Methods**: GARCH models (Arch library) and LSTM (Long Short-Term Memory) neural networks.
    - **Features**: Data preprocessing, stationarity testing (ADF), autocorrelation analysis, and rolling forecasts.
    - **Input**: Uses `datasets/abc.csv` (or generates dummy data if missing).
- **`invest.ipynb`**: A notebook focused on price prediction using LSTM models.
    - **Methods**: LSTM neural networks for sequence prediction.
    - **Features**: Training on historical data to predict future prices (e.g., next 7 days).
    - **Input**: Uses `datasets/Preprocess.csv`.
- **`datasets/`**: Directory containing the CSV data files used by the notebooks.
    - `abc.csv`: Historical ticker data (Open, High, Low, Close, Volume).
    - `Preprocess.csv`: Preprocessed dataset for price prediction models.

## Prerequisites

To run this project, you will need Python installed along with the following libraries:

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn statsmodels arch tensorflow pandas-datareader
```

**Note:** The `arch` library is specifically required for the GARCH modeling in the Volatility Prediction notebook.

## Usage

1.  **Environment Setup**: Ensure you have a Python environment set up with the required packages.
    *   *Tip: Recommended to use Python 3.9+.*
2.  **Data**: Verify that the `datasets/` directory contains the necessary `.csv` files.
3.  **Run Notebooks**: Open the Jupyter notebooks (`.ipynb` files) and execute the cells sequentially.

## Documentation

Additional documentation files are available:
- `Comprehensive Volatility Forecasting.pdf`
- `Volatility Forecasting Script Documentation.pdf`
