# Technical Analysis Script

This repository contains Python scripts for conducting technical analysis using the Moving Average Convergence Divergence (MACD), Bollinger Bands and Volume indicators. These scripts are designed to fetch historical stock price data, calculate the indicators, and generate visualizations.

## MACD Script

### Overview

The MACD script fetches historical stock price data from Yahoo Finance, calculates the MACD and Signal Line, and produces a time series plot with MACD plotted below the stock price. Users can customize the short-term, long-term, and signal span parameters for the MACD calculation.

### Usage

1. Install the required libraries:

    ```bash
    pip install pandas yfinance matplotlib
    ```

2. Run the script:

    ```bash
    python MACD.ipynb
    ```

3. Use the configure function to input asset tickers and date ranges, as well as MACD parameter values.

4. View the generated time series plot with MACD.

### Dependencies

- pandas
- yfinance
- matplotlib

## Bollinger Bands Script

### Overview

The Bollinger Bands script fetches historical stock price data from Yahoo Finance, calculates Bollinger Bands, and generates a time series plot with the stock price and Bollinger Bands. Users can customize the window size and standard deviation for the Bollinger Bands calculation.

### Usage

1. Install the required libraries:

    ```bash
    pip install pandas yfinance matplotlib
    ```

2. Run the script:

    ```bash
    python Bollinger_Bands.ipynb
    ```

3. Use the configure function to input asset tickers, date range, window size, and standard deviation values.

4. View the generated time series plot with Bollinger Bands.

### Dependencies

- pandas
- yfinance
- matplotlib

## Volume Analysis Script

This Python script analyzes volume-related indicators for a given stock, identifying support and resistance levels based on volume thresholds.

### Requirements
- Python 3
- Pandas
- Matplotlib

### Usage
1. Import the necessary libraries:
    ```python
    import pandas as pd
    import matplotlib.pyplot as plt
    ```

2. Define or load your stock data as a Pandas DataFrame.

3. Import the `plot_volume_levels` function from the script:
    ```python
    from stock_analysis import plot_volume_levels
    ```

4. Call the function with your stock data and ticker:
    ```python
    plot_volume_levels(data, 'AAPL', volume_factor=2.0)
    ```
   Adjust parameters such as `volume_factor` and `window` as needed.

### Parameters
- `data` (pd.DataFrame): DataFrame containing stock data.
- `ticker` (str): Stock ticker.
- `volume_factor` (float, optional): Factor to determine the volume threshold. Default is 1.5.
- `window` (int, optional): Rolling window size for moving average calculation. Default is 20.

### Output
The function generates a Matplotlib plot with two subplots:
1. Price chart with support and resistance levels highlighted.
2. Volume chart.

Additionally, it prints the calculated support and resistance levels.

## Contributors

- [Nicky Taylor](https://github.com/CoderNicky)

Feel free to contribute, report issues, or suggest improvements!

## License

This project is licensed under the MIT License.
