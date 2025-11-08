# Unsupervised Learning Trading Strategy: K-Means Clustering with Portfolio Optimization

A quantitative trading strategy that uses unsupervised machine learning (K-Means clustering) combined with technical indicators and Fama-French factor analysis to construct optimized portfolios from S&P 500 stocks.

## 📊 Strategy Overview

This project implements a systematic trading approach that:
1. Clusters stocks based on technical and fundamental features
2. Selects high-momentum stocks from optimal clusters
3. Optimizes portfolio weights using Modern Portfolio Theory (Efficient Frontier)
4. Rebalances monthly to maximize risk-adjusted returns

## 🔧 Features

### Technical Indicators
- **Garman-Klass Volatility** - Advanced volatility estimation
- **RSI (Relative Strength Index)** - Momentum indicator
- **Bollinger Bands** - Volatility bands
- **ATR (Average True Range)** - Volatility measure
- **MACD** - Trend-following momentum
- **Dollar Volume** - Liquidity metric

### Factor Analysis
- **Fama-French 5-Factor Model** - Rolling factor betas for:
  - Market Risk (Mkt-RF)
  - Size (SMB)
  - Value (HML)
  - Operating Profitability (RMW)
  - Investment (CMA)

### Portfolio Construction
- **K-Means Clustering** - Groups similar stocks based on features
- **Efficient Frontier Optimization** - Maximizes Sharpe ratio
- **Monthly Rebalancing** - Dynamic portfolio updates
- **Top 150 Most Liquid Stocks** - Filtered by 5-year rolling dollar volume

