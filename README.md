# Equal Weight S&P 500 Screener

## Overview

The **Equal Weight S&P 500 Screener** is an algorithmic trading tool that analyzes and screens stocks in the S&P 500 index, assigning equal weights to all stocks instead of market-cap-weighted allocation. This allows investors to diversify their portfolio with an unbiased weightage distribution.

## Features

- Fetches real-time or historical S&P 500 stock data.
- Screens stocks based on predefined financial metrics.
- Calculates equal weight allocation for all stocks.
- Provides visualization and insights for portfolio balancing.
- Automated rebalancing strategy.
- Exports recommended trades to an Excel file with formatted output.

## Tech Stack

- **Programming Language**: Python
- **Libraries Used**:
  - `pandas` (data handling)
  - `numpy` (mathematical computations)
  - `requests` (fetching data from APIs)
  - `xlsxwriter` (exporting data to Excel)
  - `math` (mathematical operations)
  - `matplotlib.pyplot` (data visualization)
  - `webbrowser` (open files in the browser)
- **Data Source**: CSV file containing S&P 500 stock information

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/equal-weight-sp500.git
   ```

2. Ensure you have a CSV file (`sp500_companies.csv`) with the following columns:
   - `Symbol` (Stock Ticker)
   - `Currentprice` (Latest stock price)
   - `Marketcap` (Market capitalization)


## How It Works

1. **Load S&P 500 Stock Data**: The program reads stock symbols, prices, and market capitalization from `sp500_companies.csv`.
2. **Data Sorting**: Stocks are sorted alphabetically by ticker symbol.
3. **Chunking Stocks**: The list of stocks is split into smaller groups for easier processing.
4. **Portfolio Input**: The user inputs their total investment amount.
5. **Position Sizing**: The program calculates an equal weight allocation per stock.
6. **Number of Shares Calculation**: Determines how many shares of each stock to buy.
7. **Export to Excel**: Outputs the recommended trades into a well-formatted Excel file (`Recommended trades.xlsx`).
8. **Excel Formatting**: Applies background color, font styling, and currency formatting for readability.

## Configuration

Modify `sp500_companies.csv` to update stock data before running the script.

## Future Enhancements

- Automate stock data fetching using an API (Yahoo Finance or Alpha Vantage).
- Implement error handling for missing or incorrect stock data.
- Add visualization for portfolio performance trends.
- Include sentiment analysis for better screening.


## Contact

For any questions or contributions, reach out at [thelogical369@gmail.com](mailto:thelogical369@gmail.com).
