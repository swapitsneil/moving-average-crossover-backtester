# moving-average-crossover-backtester

## 📌 Overview
This project implements and backtests a **Moving Average Crossover** trading strategy for Bitcoin (**BTC-USD**).  
It downloads historical price data, applies a trading rule based on two simple moving averages (SMA), compares the results with a **buy-and-hold** benchmark, and generates visual performance reports.

---

## 📈 Strategy Logic
The **Moving Average Crossover** strategy works by:
- **Short SMA (50 days)** and **Long SMA (200 days)** are calculated.
- **Buy signal:** Short SMA crosses above Long SMA.
- **Sell signal:** Short SMA crosses below Long SMA.
- The system is either **fully invested** or **fully out of the market** based on signals.

---

## 🛠 Features
- Download historical BTC-USD price data using [Yahoo Finance](https://pypi.org/project/yfinance/).
- Compute moving averages, trading signals, and returns.
- Backtest the strategy vs. a buy-and-hold benchmark.
- Calculate performance metrics:
  - CAGR (Compound Annual Growth Rate)
  - Volatility
  - Sharpe Ratio
  - Maximum Drawdown
- Generate and save plots:
  - Price & Moving Averages chart
  - Equity curve comparison
  - Drawdown chart
- Save metrics summary as a CSV file.

---


---

## 📊 Example Outputs
### Price & Moving Averages
Shows BTC-USD price along with the 50-day and 200-day SMAs.

### Equity Curve
Compares strategy vs buy-and-hold over the test period.

### Drawdown
Highlights periods of peak-to-trough losses for the strategy.

---

## ⚙️ Installation
1. Clone the repository:
   
       git clone https://github.com/yourusername/moving-average-crossover-backtester.git
       cd moving-average-crossover-backtester
   
2. Install dependencies:

        pip install pandas numpy matplotlib yfinance

   
## 🚀 Usage
Run the backtester script:

    python backtester.py
The results (charts and metrics) will be saved in the results/ folder.

## 📅 Default Parameters
ticker: BTC-USD

start date: 2020-01-01

end date: 2025-01-01

short SMA window: 50 days

long SMA window: 200 days

You can change these values in the script to test different assets and timeframes.

## 📌 Performance Metrics
The script calculates:

Metric	Description
CAGR	Compound Annual Growth Rate
Volatility	Annualized standard deviation of returns
Sharpe Ratio	Risk-adjusted return (risk-free rate = 0)
Max Drawdown	Largest peak-to-trough decline


## 🤝 Contributing
Pull requests and improvements are welcome!
If you find this project useful, please ⭐ the repository.

### 📧 Contact
Author: Swapnil Nicolson Dadel

Email: swapnilnicolson.201@gmail.com

GitHub: swapitsneil

