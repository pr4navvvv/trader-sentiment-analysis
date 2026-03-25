# Primetrade.ai Data Science Assignment

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
```trader-sentiment-analysis/
│
├── primetrade_analysis.ipynb
├── historical_data.xlsx
├── fear_greed_index.xlsx
├── Screenshot 2026-03-25.png
└── README.md
```
