# 📈 Small Cap Trading Bot

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE) [![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://python.org) [![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange.svg)](https://jupyter.org)

**Quantitative backtesting system for small-cap stocks with ATR-based risk management and position sizing**

---

## 📝 Overview

A systematic backtesting engine for long-only small-cap equity strategies. Uses ATR-based dynamic stop-loss and take-profit levels with fixed fractional position sizing (1% risk per trade). The bot processes historical OHLC data via `yfinance`, simulates trade execution, and produces performance dashboards with key metrics.

## 🔑 Key Features

- **Dynamic ATR-based Stop Loss (1.9× ATR) and Take Profit (3.2× ATR)**
- **Fixed fractional position sizing (1% capital risk per trade)**
- **Small-cap universe filter ($1–$20 stocks)**
- **In-Sample / Out-of-Sample split to avoid overfitting**
- **Performance dashboards: expectancy, max drawdown, profit factor, win rate**
- **Trade-by-trade analysis with entry/exit tracking**


## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/elbrujo325/small-cap-trading-bot.git
cd small-cap-trading-bot

# Install dependencies
pip install pandas numpy matplotlib yfinance

# Run the notebook
jupyter notebook small_cap_trading_bot.ipynb
```

The notebook walks through the entire pipeline: data download → signal generation → backtesting → performance analysis.

## 🛠️ Tech Stack

Python · Pandas · NumPy · Matplotlib (GridSpec) · yfinance

## 📄 License

This project is licensed under the MIT License — see [LICENSE](./LICENSE) for details.

---

<div align="center">

*By [Henry Paolo Alfaro Sotil](https://github.com/elbrujo325) — Physicist & Data Scientist*

</div>
