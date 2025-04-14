# Bollinger Bands Mean Reversion Strategy

This project tests a simple mean reversion strategy on SPY using Bollinger Bands.

---

## ✅ Objectives:
- Load and visualize SPY historical price data
- Compute Bollinger Bands (20-day MA ± 2 std)
- Create entry/exit rules based on band crossovers
- Backtest performance using historical data

---

## 📊 Strategy Rules:
- **Buy** when price crosses below the lower band
- **Sell** when price crosses above the upper band
- **Exit** when price returns to the moving average

---

## 🧪 Data Source:
- Yahoo Finance (via `yfinance` package)

