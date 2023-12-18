# SBIN-Stock-Visualization
# Stock Analysis with yfinance and Matplotlib

This Python script uses the `yfinance` library to fetch historical stock data for State Bank of India (SBIN) for the month of November 2023. The closing prices are then plotted using `matplotlib`.

## Installation

Ensure you have the required libraries installed by running the following commands:

```bash
pip install yfinance
pip install matplotlib

## Usage
Open the Python script or Jupyter notebook containing the code.
Run the code to fetch historical stock data and plot the closing prices for SBIN.

## Code
import yfinance as yf
import matplotlib.pyplot as plt

# Fetch historical stock data for SBIN
data = yf.download("SBIN.BO", start="2023-11-01", end="2023-11-30")

# Plot the closing prices
data['Close'].plot()
plt.title('SBIN Stock Closing Prices')
plt.xlabel('Date')
plt.ylabel('Closing Price')
plt.show()
