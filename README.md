# 📊 Trader Behavior vs Market Sentiment

This project analyzes how trader behavior and performance change based on crypto market sentiment (Fear, Greed, Neutral), using real trading data and Bitcoin Fear-Greed Index.

## 🔍 Objective
Explore:
- How trader PnL varies across sentiments
- Risk-taking behavior in different emotional states
- Most traded coins per sentiment
- Buy/Sell trends and performance metrics

## 📂 Dataset
- Historical trader data from Hyperliquid
  (https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view)
- Bitcoin Fear-Greed Index (value + classification)
  (https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view)

## 🧮 Features Engineered
- `risk_score`: Risk proxy based on size × price deviation
- `pnl_efficiency`: Profit per dollar spent
- `price_deviation`: Execution deviation from average cost

## 📈 Key Insights
- No significant PnL difference across sentiments
- Traders take **more risk in Neutral** conditions
- **Worst PnL efficiency in Greed**, possibly due to overconfidence
- High **PnL volatility** in Fear & Greed
- Specific coins like **HYPE & @107** are sentiment-sensitive
- T-test confirms **no statistical difference** in PnL across Fear vs Greed
- Our analysis reveals not just how traders perform, but how their behavior, asset preferences, and risk posture adapt to market sentiment. By quantifying these patterns, we open up new possibilities for building sentiment-aware trading models.
- Sentiment-Aware Strategies Could Reduce Risk and Improve Entry Timing:
  The data suggests that trading behavior shifts with sentiment — not necessarily performance. By integrating the Fear-Greed Index into strategy logic (e.g., scaling down trades in Neutral), traders may better      manage risk exposure, avoid overtrading in uncertain times, and exploit behavioral patterns in specific coins.

## 📊 Tools Used
- Python, Pandas, Seaborn, Matplotlib
- Scipy (for t-tests)

## 🚀 How to Run
1. Clone this repo
2. Install required libraries: `pip install pandas matplotlib seaborn scipy`
3. Edit the dataset location.
4. Run the notebook: `Trader_Behavior_Insights.ipynb`

