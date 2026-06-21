> ⚠️ **Este repositorio fue consolidado y mejorado en [smallcap-quant-ml](https://github.com/elbrujo325/smallcap-quant-ml). Se conserva aquí por historial.**

---

# Small Cap Trading Bot

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange.svg)](https://jupyter.org/)

**Quantitative backtesting system for small-cap stocks with ATR-based risk management and position sizing**

---

## 📋 Overview

A systematic backtesting engine for long-only small-cap equity strategies. Uses ATR-based dynamic stop-loss and take-profit levels with fixed-fractional position sizing (1% risk per trade).

### Key Features
- **Dynamic ATR-based Risk Management** — Stop Loss (1.9×ATR) and Take Profit (3.2×ATR)
- **Fixed Fractional Position Sizing** — 1% capital risk per trade
- **Small-Cap Universe Filter** — Price range $1–$20
- **Discrete Event-Driven Backtest** — Trade-by-trade simulation with MAE/MFE tracking
- **Performance Analytics** — Win Rate, Profit Factor, Sharpe Ratio, Max Drawdown
- **Visualization** — Equity curve, PnL distribution, exit reason analysis

---

## 🚀 Quick Start

```bash
git clone https://github.com/elbrujo325/small-cap-trading-bot.git
cd small-cap-trading-bot
pip install pandas numpy matplotlib yfinance
jupyter notebook PROYECTO_BOT_TRADING_v2.ipynb
```

---

## 📊 Strategy Parameters

| Parameter | Value |
|-----------|-------|
| Universe | Small Cap ($1–$20) |
| Timeframe | 1 Hour |
| Indicators | ATR(50), SMA(10), ROC(5), Price Structure |
| Stop Loss | 1.9×ATR |
| Take Profit | 3.2×ATR |
| Time Exit | 40 bars max |
| Risk/Trade | 1% Capital |
| Initial Capital | $10,000 |

**Entry Condition (Long):**
- Price ∈ [$1.00, $20.00]
- Open > SMA(10)
- ROC decaying (momentum fading)
- Price structure: Open[7] > High[9]

---

## 🛠️ Tech Stack

Python · Pandas · NumPy · Matplotlib · yfinance · Jupyter

---

## 📄 License

MIT License — see [LICENSE](./LICENSE)

---

<div align="center">

**By Henry Paolo Alfaro Sotil — Physicist & Data Scientist**

[GitHub](https://github.com/elbrujo325) · [LinkedIn](https://linkedin.com/in/henry-paolo-alfaro-sotil-3b75a9338)

</div>
