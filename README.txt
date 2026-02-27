📊 Trader Performance vs Market Sentiment Analysis
📌 Overview
 
This project analyzes the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader behavior & performance using historical trading data from Hyperliquid.

The objective is to uncover behavioral and profitability patterns across different sentiment regimes and derive actionable trading insights.

🎯 Problem Statement

Does trader performance differ during:

Extreme Fear?

Fear?

Neutral?

Greed?

Extreme Greed?

And if so:

How does win rate change?

How does PnL distribution vary?

Do traders change directional behavior (Long vs Short)?

What strategic adjustments can be made?


📂 Datasets
1️⃣ Bitcoin Market Sentiment Dataset

Date

Sentiment Classification (Extreme Fear → Extreme Greed)

2️⃣ Hyperliquid Historical Trader Data

Account

Coin

Execution Price

Position Size (USD & Tokens)

Direction (Long/Short)

Closed PnL

Timestamp

🛠 Methodology
Step 1: Data Preparation

Converted timestamps to datetime format

Standardized daily granularity

Cleaned missing values

Verified dataset integrity

Step 2: Data Alignment

Merged trader data with sentiment data on daily date

Validated merge correctness

Ensured no sentiment mismatches

Step 3: Feature Engineering

Created binary win indicator (PnL > 0)

Calculated win rate per sentiment regime

Aggregated PnL statistics by classification

Computed Long vs Short distribution

Step 4: Exploratory Analysis

PnL distribution (boxplots)

Win rate comparison (bar charts)

Behavioral analysis (Long vs Short ratio)


📈 Key Findings
1️⃣ Performance Peaks During Extreme Greed

Extreme Greed periods show the highest win rate (~46%) and stronger profitability patterns, suggesting momentum-driven market behavior benefits traders.

2️⃣ Extreme Fear Shows Lower Predictability

Win rate drops significantly (~37%) during Extreme Fear, indicating higher uncertainty and inconsistent outcomes.

3️⃣ Sentiment Influences Trader Behavior

Directional bias (Long/Short distribution) shifts across sentiment regimes, reflecting emotional market conditions affecting positioning.

💡 Actionable Strategy Recommendations

1️⃣ Risk Reduction During Fear

Reduce leverage

Decrease position sizing

Avoid overtrading during volatile periods

2️⃣ Controlled Exposure During Greed

Increase exposure gradually in bullish sentiment

Maintain strict stop-loss discipline

Avoid excessive leverage despite higher win rates

🧰 Tech Stack

Python

Pandas

Matplotlib

Google Colab

GitHub

📊 Repository Structure
Trader_Performance_vs_Sentiment.ipynb
README.md



🚀 Conclusion

Market sentiment has a measurable impact on trader profitability and behavior.
Incorporating sentiment-aware risk adjustments can improve trading performance and capital preservation.