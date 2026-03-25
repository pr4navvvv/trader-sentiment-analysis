# Primetrade.ai Data Science Assignment

## How to Run
1. Install requirements: pip install pandas openpyxl matplotlib seaborn scikit-learn
2. Place both Excel files in the same folder as the notebook
3. Open primetrade_analysis.ipynb in Jupyter and run all cells

---

## Project Overview
This project analyzes historical cryptocurrency trading data together with the Fear & Greed market sentiment index to identify patterns in trader behaviour, profitability, and risk exposure.

The goal of the analysis is to determine how market sentiment influences trading performance and to generate actionable strategy recommendations based on data-driven insights.

---

## Objectives
- Merge trading data with market sentiment indicators
- Analyze trader performance across Fear and Greed market conditions
- Evaluate relationship between trade size and profitability
- Identify behavioural patterns in trading activity
- Segment traders into meaningful groups using clustering techniques
- Generate strategy recommendations based on findings

---

## Dataset Description

### 1. Historical Trades Data
Contains transaction-level trading information including:
- Account
- Coin traded
- Execution price
- Trade size (USD and tokens)
- Trade direction (Buy/Sell)
- Closed profit and loss (PnL)
- Timestamp

### 2. Fear & Greed Index Data
Represents market sentiment classification:
- Extreme Fear
- Fear
- Neutral
- Greed
- Extreme Greed

---

## Methodology

### Data Preprocessing
- Converted timestamps into standardized date format
- Merged sentiment dataset with trade dataset using date field
- Checked for missing values and ensured consistency

### Exploratory Data Analysis
- Compared average PnL across sentiment categories
- Analyzed relationship between trade size and profitability
- Evaluated long vs short trading behaviour
- Generated correlation heatmaps to identify feature relationships

### Trader Segmentation
KMeans clustering was used to group traders based on:
- Average profitability
- Trade size
- Execution price behaviour
- Trading frequency

This helps identify different trading styles and performance patterns.

---

## Key Findings
- Market sentiment influences trading behaviour and profitability patterns
- Trade size has only weak correlation with profit outcomes
- Execution price alone is not a strong predictor of profitability
- Consistent traders tend to achieve more stable returns
- Different trader groups exhibit distinct risk and performance profiles

---

## Visual Insights

### 1. Trader Consistency Distribution
<p align="center">
<img src="Screenshot 2026-03-25 170053.png" width="400"/>
</p>

---

### 2. Trading Behaviour Metrics by Market Sentiment
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 5.00.01 PM.jpeg" width="700"/>
</p>

---

### 3. Average Trades per Day per Trader, Average Trade Size (USD), Long Ratio (%) by Market Sentiment
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 5.00.20 PM.jpeg" width="700"/>
</p>

---

### 4. Impact of Trade Size on Profitability and Win Rate
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 5.00.35 PM.jpeg" width="600"/>
</p>

---

### 5. Feature Importance for Predicting Profitability
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 5.01.08 PM.jpeg" width="500"/>
</p>

---

### 6. PnL Distribution across Market Sentiment
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 9.07.20 PM.jpeg" width="500"/>
</p>

---

### 7. Long vs Short Trades Distribution by Market Sentiment
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 9.07.34 PM.jpeg" width="500"/>
</p>

---

### 8. Trader Segmentation using K-Means Clustering
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 9.07.47 PM.jpeg" width="500"/>
</p>

---

### 9. Feature Correlation Heatmap (PnL, Trade Size, Execution Price)
<p align="center">
<img src="WhatsApp Image 2026-03-25 at 9.08.06 PM.jpeg" width="500"/>
</p>

---

## Key Insights
- Market sentiment influences trading behaviour and profitability patterns.
- Trades executed during **Extreme Greed** periods show higher average PnL but also higher variability, indicating increased risk-taking behaviour.
- Trade size has only a weak correlation with profitability, suggesting that increasing position size alone does not guarantee better returns.
- Execution price has minimal impact on profit outcomes, highlighting the importance of timing and strategy rather than price level alone.
- Consistent traders tend to achieve more stable returns compared to traders relying on occasional large profits.
- Clustering analysis reveals distinct trader profiles based on trading frequency, trade size, and profitability patterns.
- Different trader groups exhibit varying levels of risk exposure and performance stability.

---

## Strategy Recommendations

- Adjust trade size based on market sentiment. During Fear conditions, reducing position size can help manage downside risk and improve consistency.
- Focus on consistent trading behaviour rather than relying on infrequent high-risk trades.
- Incorporate sentiment indicators such as Fear & Greed Index to improve decision-making and align trading strategies with market mood.
- Emphasize risk-adjusted performance metrics instead of only maximizing trade size.
- Use trader segmentation insights to identify behavioural patterns and optimize trading strategies accordingly.

---

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn (KMeans clustering, StandardScaler)

---


## Project Structure

```
trader-sentiment-analysis/
│
├── primetrade_analysis.ipynb
├── historical_data.xlsx
├── fear_greed_index.xlsx
├── Screenshot 2026-03-25.png
└── README.md
```
