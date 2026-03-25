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
![WhatsApp Image 2026-03-25 at 5 00 01 PM](https://github.com/user-attachments/assets/086272b1-7a81-4adc-a033-2241c9e94092)
![WhatsApp Image 2026-03-25 at 5 00 20 PM](https://github.com/user-attachments/assets/109ebcd3-894b-446d-82b8-df812215c6b6)
![WhatsApp Image 2026-03-25 at 5 00 35 PM](https://github.com/user-attachments/assets/e73aceb5-4e97-49b0-96ab-782f2510a013)
![WhatsApp Image 2026-03-25 at 5 00 54 PM](https://github.com/user-attachments/assets/852645bd-91c3-4f6f-9af3-2553b6d71872)
![WhatsApp Image 2026-03-25 at 9 07 20 PM](https://github.com/user-attachments/assets/264376d5-debe-4aba-a428-90a8abe4c543)
![WhatsApp Image 2026-03-25 at 9 07 34 PM](https://github.com/user-attachments/assets/3abd2d3e-32b7-446b-86b4-baa9a0761b07)
![WhatsApp Image 2026-03-25 at 9 07 47 PM](https://github.com/user-attachments/assets/81983e97-ad09-4377-94c5-48544fe9dc96)
![WhatsApp Image 2026-03-25 at 9 08 06 PM](https://github.com/user-attachments/assets/5cfbaaa4-9741-452d-8a5a-1006cb7d7f35)


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
