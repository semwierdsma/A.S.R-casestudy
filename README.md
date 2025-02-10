# A.S.R-casestudy
A.S.R casestudy

Overview

This Python script implements a command-line interface (CLI) for managing an investment portfolio. It allows users to: Add stocks to the portfolio, Track stock prices and transaction costs, view the portfolio's composition, analyze historical stock price trends using graphs, calculate portfolio value and asset weights.

Features
1. Add Asset to Portfolio
Users can enter details such as the stock ticker, sector, asset class, quantity, purchase price, and market.
Transaction costs are automatically calculated based on the selected market:
EAM: €3
TDG: €3.90
NDQ: $0.50 + 0.25% currency conversion fee
XET: €4
If the asset already exists, the system updates the quantity, recalculates the average purchase price, and adjusts the total transaction cost.
Stock prices are retrieved using Yahoo Finance (yfinance).
If the stock is listed in the EAM, TDG, or XET markets, the system converts USD prices to EUR.

2. View Portfolio
Displays details of each asset, including:
Ticker
Sector
Asset class
Quantity
Average purchase price
Transaction cost
Current market price
Total profit

3. Plot Stock History
Users can input stock tickers and a start date.
Retrieves historical stock prices using yfinance.
Displays a line graph of stock price movements over time.

4. Calculate Portfolio Value & Weights
Calculates the total portfolio value by summing the market value of all assets.
Provides breakdowns of portfolio value and weight distribution by:
Individual assets
Asset class
Sector
Dependencies
forex_python.converter (for currency exchange rates)
yfinance (for stock price data)
matplotlib (for plotting stock price trends)
datetime (for handling date inputs)

Usage

The script provides a CLI menu with the following options:
1. Add Asset: Add a new stock to your portfolio.
2. View Portfolio: Display all portfolio assets.
3. Show Historical Prices (Graph): View stock price history.
4. Calculate Portfolio Value and Weights: Analyze portfolio distribution.
5. Exit: Quit the program.

Dependencies
forex_python.converter (for currency exchange rates)
yfinance (for stock price data)
matplotlib (for plotting stock price trends)
datetime (for handling date inputs)
