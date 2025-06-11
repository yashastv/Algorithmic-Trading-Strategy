
# 📈 Algorithmic Trading Strategy – S&P 500 with Technical Indicators

This project implements a multi-indicator algorithmic trading strategy using S&P 500 data. It calculates advanced technical signals and performs regression-based feature engineering for predictive analysis and portfolio optimization.

---

## 🔍 Problem Statement

Design and evaluate a rule-based trading strategy on S&P 500 stocks using rolling regressions and common technical indicators. The strategy is intended to generate alpha signals that can be used for position sizing and risk-managed exposure.

---

## 📊 Data Sources

- **S&P 500 stock data** fetched using:
  - `yfinance`
  - `pandas_datareader`
- Historical OHLCV data including: open, high, low, close, and volume

---

## 📈 Technical Indicators Used

- **Garman-Klass Volatility**
- **Relative Strength Index (RSI)**
- **Bollinger Bands**
- **Average True Range (ATR)**
- **Moving Average Convergence Divergence (MACD)**
- **Dollar Volume**

These indicators are used to construct features for signal generation and to enhance regression-based prediction performance.

---

## 🔧 Tools and Libraries

- `statsmodels` – Rolling OLS regressions
- `pandas`, `numpy` – Data manipulation
- `matplotlib`, `seaborn` – Visualization
- `yfinance`, `pandas_datareader` – Data sourcing
- `PyPortfolioOpt` – Portfolio optimization
- `pandas-ta` – Technical analysis

---

## 🧠 Strategy Logic

1. Download daily price data for selected S&P 500 stocks
2. Compute multiple technical indicators
3. Use Rolling OLS regressions to build a dynamic factor model
4. Generate alpha signals from coefficients and feature values
5. Apply portfolio optimization to allocate weights
6. Backtest the strategy

---

## 📁 Notebook File

The full implementation is in:
```bash
ATS.ipynb
