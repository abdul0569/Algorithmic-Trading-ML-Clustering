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

## 📁 Project Structure

```
├── Algorithmic_Trading_Machine_Learning_Quant_Strategies.ipynb
├── README.md
└── requirements.txt (see below)
```

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib statsmodels pandas-datareader yfinance scikit-learn PyPortfolioOpt pandas-ta
```


## 📊 Results

The strategy generates monthly-rebalanced portfolios optimized for:
- **Risk-Adjusted Returns** - Maximum Sharpe ratio
- **Momentum Capture** - High RSI cluster selection
- **Diversification** - Weight constraints across stocks
- **Factor Exposure** - Fama-French aligned risk profile

## 🔍 Key Insights

- **Momentum Persistence**: Stocks clustered around RSI 70 tend to continue outperforming
- **Liquidity Filtering**: Top 150 stocks ensure tradability and reduce slippage
- **Rolling Factor Betas**: Capture time-varying risk exposures
- **Monthly Rebalancing**: Balances transaction costs with strategy adaptability

## 📝 Usage

1. Clone the repository
2. Install dependencies
3. Run the Jupyter notebook cells sequentially
4. Adjust parameters:
   - `lookback_period` - Historical data window
   - `n_clusters` - Number of K-Means clusters
   - `target_cluster` - Cluster selection logic
   - Weight constraints in portfolio optimization

## ⚠️ Disclaimer

This project is for **educational and research purposes only**. Past performance does not guarantee future results. Always conduct thorough due diligence and risk assessment before live trading.

## 📄 License

MIT License - See LICENSE file for details

---
