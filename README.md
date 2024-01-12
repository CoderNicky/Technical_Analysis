# Time Series Analysis Scripts

This repository contains Python scripts for conducting time series analysis using the Moving Average Convergence Divergence (MACD) and Bollinger Bands indicators. These scripts are designed to fetch historical stock price data, calculate the indicators, and generate visualizations.

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
    python Bollinger_bands.ipynb
    ```

3. Use the configure function to input asset tickers, date range, window size, and standard deviation values.

4. View the generated time series plot with Bollinger Bands.

### Dependencies

- pandas
- yfinance
- matplotlib

## Contributors

- [Nicky Taylor](https://github.com/CoderNicky)

Feel free to contribute, report issues, or suggest improvements!

## License

This project is licensed under the MIT License.
