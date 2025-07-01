# 📊 Real-Time Financial Strategy Analyzer

An interactive backtesting and analytics dashboard developed to evaluate quantitative trading strategies using historical financial data. This project was built entirely by me using Python, with a strong focus on clean design, performance, and usability for data-driven financial analysis.

---

## 📌 Project Overview

The Real-Time Financial Strategy Analyzer allows users to test and compare algorithmic trading strategies using real-world market data. It helps assess performance through widely used financial metrics and intuitive visualizations. The project supports modular strategy development and can be extended to include new indicators and techniques.

---

## 🧠 Key Features

- ✅ Backtesting support for common trading strategies:
  - Mean Reversion
  - Moving Average (MA) Crossover
  - Pairs Trading
- 📈 Performance Metrics:
  - Sharpe Ratio
  - Maximum Drawdown
  - Cumulative Return
- 📉 Visual Analytics:
  - Equity curves
  - Strategy comparisons
  - Risk-return plots
- ⚡ Efficient data processing using Polars for faster computation than pandas
- 🌐 Real-time data retrieval using yfinance API
- 🖥️ Streamlit-powered interactive user interface
- 🧩 Modular codebase for easy expansion and customization

---

## 🛠️ Technologies Used

- Python – Core programming language for strategy logic and data processing
- Polars – High-performance DataFrame library for fast, memory-efficient analysis
- pandas – Used for compatibility and preprocessing where required
- yfinance – API for fetching historical financial data from Yahoo Finance
- Streamlit – Lightweight Python framework for building the interactive web dashboard
- Matplotlib & Seaborn – For generating clear financial visualizations and performance plots

---
## 💡 Use Cases

- Academic research in quantitative finance
- Learning and experimentation with trading strategies
- Portfolio strategy testing before deployment
- Visual storytelling of financial model performance

---

## ⚙️ Performance Insights

- Replacing pandas with Polars has reduced data loading and processing time significantly, especially for large datasets
- Modularized components ensure strategy logic is isolated and easy to maintain
- Visualization is lightweight and renders instantly for small to medium datasets

---

## 🚀 Future Improvements

- Add live data integration via WebSocket APIs for streaming market data
- Support portfolio-level strategy combination and risk allocation
- Implement additional metrics such as Calmar Ratio, Sortino Ratio, and win rate
- Integrate interactive filters for date ranges, instruments, and volatility thresholds
- Add export options for reports (PDF/CSV)

---

## ⚙️ Getting Started

### 1. Set Python Path (only if modules fail to import)

For Linux/macOS:

   export PYTHONPATH=src

For Windows CMD:

   set PYTHONPATH=src

### 2. Run the Streamlit Application

   streamlit run src/financial_analyzer/app.py

This will open the dashboard in your default browser at http://localhost:8501.

---

## 📊 Supported Strategies

### 1. Mean Reversion

Detects when a stock's price deviates significantly from its mean and places trades expecting it to revert to the mean.

### 2. Moving Average Crossover

Uses short- and long-term moving averages. A buy/sell signal is triggered when the short MA crosses the long MA.

### 3. Pairs Trading

Identifies pairs of cointegrated stocks. Trades are executed based on statistical divergence and convergence of price ratios.

---
