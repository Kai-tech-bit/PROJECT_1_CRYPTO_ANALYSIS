# 📊 Crypto Asset Risk Analysis & Algorithmic Backtesting

## 📌 Overview
This project performs **comprehensive statistical analysis and backtesting** on selected cryptocurrencies — **BTC, ETH, SOL, DOGE, BNB, ADA** — using hourly OHLCV data. The goal is to **evaluate asset-specific risk/return profiles**, explore inter-asset relationships, and test **systematic trading strategies** with robust performance metrics.

---

## 🎯 Objectives
- Fetch and process historical OHLCV data using **CCXT**.
- Calculate **log returns**, **volatility**, **skewness**, **kurtosis**, and cross-asset **correlations**.
- Visualize **risk-return tradeoffs** and interdependence using advanced plots.
- Implement and compare **two systematic trading strategies**:
  1. **SMA Crossover** — 50-period vs 100-period.
  2. **Hybrid Filter** — **Supertrend** & **MACD Crossover**.
- Evaluate and compare performance: **CAGR**, **Sharpe ratio**, **max drawdown**, **win-rate**, and total returns.

---

## 🛠️ Tech Stack
- **Python** — Data analysis & backtesting
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `plotly`, `ccxt`, `ta`, `seaborn`
- **Visualization**: Interactive charts for drawdowns, correlation heatmaps, and PnL curves.

---

## 📊 Key Analysis Steps
1. **Data Collection**  
   - Hourly OHLCV data for 6 cryptocurrencies.
   - Clean & preprocess into aligned DataFrames.

2. **Statistical Diagnostics**  
   - Mean returns, volatility (hourly/daily/monthly).
   - Higher moments (skew, kurtosis).
   - Covariance and correlation matrices.

3. **Risk-Return Plotting**  
   - Mean-variance scatter plots with annotations.
   - Volatility vs return charts for different horizons.

4. **Drawdown Analysis**  
   - Rolling maximum drawdowns per asset.
   - Visual comparison across all assets.

5. **Strategy Implementation**  
   - **SMA Crossover** (50/100).
   - **Supertrend + MACD** hybrid signal filter.

6. **Backtest Evaluation**  
   - PnL curves.
   - Performance metrics comparison between strategies.

---

## 📈 Results Summary
- The **Supertrend + MACD** hybrid strategy outperformed SMA crossover in both total returns and Sharpe ratio across most assets.
- SMA crossover struggled during sideways markets due to whipsaw trades.
- Correlation heatmaps revealed strong BTC-ETH co-movement and weaker correlations for DOGE.

---

## 📂 Full Quant Report
Detailed statistical outputs, optimization results, and plots are documented here:  
[📄 View  Report](https://drive.google.com/file/d/1DOws3cSLYMLaoipWWp-h29t25RGw5_8l/view?usp=sharing)

---
