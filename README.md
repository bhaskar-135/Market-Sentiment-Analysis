Market-Sentiment-Analysis
Analyze how market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid. Your goal is to uncover patterns that could inform smarter trading strategies

📊 Market Sentiment & Trader Behavior Analysis (Hyperliquid)

 Project Overview
This project analyzes how Bitcoin market sentiment (Fear & Greed Index) influences trader behavior and performance on the Hyperliquid exchange.  
The goal is to uncover behavioral patterns, build simple predictive signals, and translate insights into actionable trading strategies.

The project progresses from descriptive analytics → predictive modeling → behavioral clustering → interactive dashboarding.

---

 Objectives
- Understand how trader performance changes across Fear vs Greed market regimes
- Identify behavioral shifts in trade frequency, sizing, and directional bias
- Segment traders into behavioral archetypes
- Build a simple predictive model for next-day profitability or risk
- Create a lightweight Streamlit dashboard for exploration

---

 📂 Dataset Description

1) Bitcoin Fear & Greed Index
- Source: Public crypto sentiment index
- Granularity: Daily
- Key Fields:
  - date
  - classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

2) Hyperliquid Trade Data
- Granularity: Trade-level
- Key Fields:
  - Account
  - Symbol
  - Side (Buy/Sell)
  - Trade Size (USD)
  - Timestamp (epoch seconds)
  - Closed PnL

 Data Preparation
- Converted timestamps from epoch to datetime
- Aligned both datasets at **daily level**
- Removed duplicates and validated missing values
- Engineered key metrics at **account–day level**

Engineered Metrics
- Daily PnL per trader
- Win rate
- Number of trades per day
- Average trade size
- Long/Short ratio
- PnL volatility (risk proxy)

 Exploratory Analysis

 Key Questions Answered
- Does performance differ between Fear vs Greed days?
- Do traders change behavior based on sentiment?
- Which trader segments are most sensitive to sentiment shifts?

Core Findings
- Traders reduce activity and position size during Fear regimes
- Over-trading and directional bias increase during Greed
- Consistent traders adapt behavior better than inconsistent traders
