# 📊 Mean Reversion Strategy using Bollinger Bands

## 📌 Strategy Overview

This project implements a **mean reversion trading strategy** on the SPY ETF using **Bollinger Bands**.

The core idea:  
> When price falls below the lower Bollinger Band, we assume it will revert back to the mean — so we enter a long position.

## 🧮 Strategy Rules

- **Buy signal:** When `Close price < Lower Bollinger Band`
- **Exit signal:** When `Close price > Upper Bollinger Band`
- **Position is held until exit signal is triggered**
- **No leverage, no transaction costs included**

## ⚙️ Technical Details

- Bollinger Bands are calculated as:
  - `MA20 = 20-day Moving Average`
  - `Upper Band = MA20 + 2 * STD`
  - `Lower Band = MA20 - 2 * STD`
- Data Source: `yfinance`
- Backtest period: `2020-01-01` to `2024-12-31`

## 📈 Performance

| Metric              | Value           |
|---------------------|------------------|
| Sharpe Ratio        | 0.8   |
| Number of Trades    | 32   |
| Cumulative Return (Strategy) | *see chart below* |
| Cumulative Return (Buy & Hold) | *see chart below* |

### 🔍 Comparison Chart:

![Strategy vs Market](./your_plot_filename.png)

## 🧠 Observations

- The strategy underperformed SPY buy-and-hold during the tested period.
- Most of the time, the strategy stayed out of the market or generated small profits/losses.
- Performance could be improved by:
  - Adding trend filters (e.g. only trade when MA50 > MA200)
  - Including stop-loss / take-profit rules
  - Testing on other instruments or timeframes

## 📂 Files

- `bollinger_backtest.ipynb`: Main notebook for strategy logic and visualization
- `README.md`: This file

---

## 📌 Next Steps

- [ ] Explore RSI or momentum-based strategies
- [ ] Add a proper backtesting framework (like `backtrader` or `bt`)
- [ ] Compare multiple strategies in one dashboard

