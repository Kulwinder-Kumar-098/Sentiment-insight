# Sentiment-insight
Trader Behavior Insights

This repository contains the analysis for the Sentiment insight analysis assignment, exploring the relationship between trader performance and market sentiment using Historic trader data and Fear and Greed Index.

Overview

The notebook (Sentiment_insight.ipynb) analyzes how market sentiment (Fear, Greed, etc.) impacts trader performance (Closed PnL, trade volume) on the Hyperliquid platform. It includes data preprocessing, merging, exploratory data analysis (EDA), visualizations, and proposed trading strategies.

How to Run
Requirements: Install dependencies:

pip install pandas seaborn matplotlib numpy
Datasets: Place fear_greed_index.csv and historical_data.csv in the same directory as the notebook.

Run: Open in Jupyter Notebook:
jupyter notebook Sentiment_insight.ipynb

Ensure datasets are accessible; outputs (plots, stats) will render in the notebook.

Key Findings
PnL by Sentiment: Highest average PnL in Extreme Greed (67.89 USD), lowest in Neutral (34.31 USD). Volatility highest in Greed (1116), lowest in Neutral (517).
Trade Behavior: Fear markets have the most trades (61,837), indicating panic or bargain hunting.
Coin-Specific: Top coins (e.g., FARTCOIN) lose in Fear but gain in Greed; outliers show high-reward potential.
Volatility: Greed/Fear markets are riskier; Neutral is stable.

Trading Strategies
Greed/Extreme Greed: Increase Buy positions for higher PnL; use stop-loss to manage volatility.
Fear/Extreme Fear: Hedge or short-sell; reduce trade size to limit losses.
Neutral: Steady trading on stable coins (e.g., top 10) for low-risk returns.
General: Diversify across coins; monitor fees in high-volume markets.
Advanced: Use sentiment thresholds (value >70 for buys); backtest strategies on historic data.

Notes
Datasets sourced from assignment links (not included in repo due to size).
Visualizations may be crowded for all coins; top-10 coins are highlighted for clarity.
Future work: Predictive modeling for PnL.
