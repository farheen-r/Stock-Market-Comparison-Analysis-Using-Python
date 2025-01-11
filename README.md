# Nvidia & Microsoft Stock Market Comparison Analysis

This project analyzes and compares the stock market performance of NVIDIA and Microsoft relative to the S&P 500 index, using Python. The analysis includes calculating daily returns and Beta values to assess their relative volatility against the market benchmark.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Requirements](#requirements)
3. [Setup and Execution](#setup-and-execution)
4. [Methodology](#methodology)
5. [Results](#results)
6. [Notes and Assumptions](#notes-and-assumptions)
7. [License](#license)

---

## Introduction

This script evaluates NVIDIA and Microsoft stocks to determine their Beta values relative to the S&P 500 index. Beta measures a stock's volatility in comparison to the overall market, helping investors assess risk levels and sensitivity to market movements.

---

## Requirements

Ensure the following Python libraries are installed:

- `yfinance`
- `pandas`
- `numpy`
- `plotly`

Install missing dependencies using:
```bash
pip install yfinance pandas numpy plotly
```

---

## Setup and Execution

1. **Clone the repository or download the script**.
2. **Specify the analysis date range**:
   - Modify `start_date` and `end_date` in the script to define the period of analysis.
3. **Run the script**:
   ```bash
   python analysis_script.py
   ```
4. **Results will be displayed in the terminal and visualized using Plotly.**

---

## Methodology

1. **Data Retrieval**:
   - Historical stock data for NVIDIA, Microsoft, and the S&P 500 is fetched using `yfinance`.

2. **Daily Returns Calculation**:
   - Computes percentage change in daily stock prices.

3. **Beta Calculation**:
   - Calculates the covariance of each stock's returns with the market and divides it by the market's variance.

4. **Comparison**:
   - Compares the Beta values of NVIDIA and Microsoft to identify the more volatile stock.

---

## Results

- Beta values for both NVIDIA and Microsoft are printed in the console.
- A conclusion indicates which stock is more volatile relative to the market.

---

## Notes and Assumptions

- **Data Source**: Stock data is retrieved from Yahoo Finance using the `yfinance` API.
- **Columns**: Ensure that stock data includes either `Adj Close` or `Close` for calculations.
- **Timeframe**: Analysis is based on the specified date range (`start_date` and `end_date`).

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

