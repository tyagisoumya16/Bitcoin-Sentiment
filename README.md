# Bitcoin-Sentiment

📌 Objective

This project analyzes whether Bitcoin market sentiment (Fear vs Greed) influences trader performance and behavior using historical trading data from Hyperliquid.

We explore:

1.Profitability differences across sentiment regimes

2.Behavioral shifts (trade frequency, size, directional bias)

3.Trader segmentation

4.Strategy recommendations based on findings

📂 Datasets Used

1.Bitcoin Fear & Greed Index

Columns: timestamp, value, classification, date

Sentiment labels: Fear / Greed

2.Hyperliquid Historical Trader Data

Fields include: account, coin, execution_price, size_usd, side, closed_pnl, timestamp, etc.

⚙️ Methodology

1. Data Cleaning

Removed duplicates

Handled missing values

Converted timestamps to daily format

Merged both datasets on date

2. Feature Engineering

Daily PnL per trader

Win rate (PnL > 0)

Trade frequency per day

Average position size

Long/Short ratio

Trader segmentation:

High vs Low size

Frequent vs Infrequent

Consistent winners vs losers

3. Comparative Analysis

Performance comparison: Fear vs Greed

Behavioral change analysis

Segment-based performance breakdown

📈 Key Insights

1. Traders show higher average PnL during Greed days compared to Fear days.

2.Trade frequency increases significantly during Fear periods, indicating volatility-driven activity.

3. Large position traders experience deeper losses during Fear regimes.

4. Long bias increases during Greed sentiment.

🎯 Strategy Recommendations

1. Risk Control Strategy
During Fear days, reduce position size by 30% to control downside volatility.

2. Trend Exploitation Strategy
During Greed days, increase long exposure for consistent winning traders.

3. Overtrading Control
Implement trade frequency cap during Fear periods to reduce drawdowns.

▶️ How to Run

1.Open notebook.ipynb in Google Colab or Jupyter.
2.Upload both datasets.
3.Run cells sequentially.
4.Charts and insights will be generated automatically.
