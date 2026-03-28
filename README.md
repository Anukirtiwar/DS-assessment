# DS-assessment
# Trader Behavior Insights: Market Sentiment vs Trading Performance

## Overview
This project analyzes the relationship between **Bitcoin market sentiment** (Fear & Greed Index) and **trader performance** using historical trading data from **Hyperliquid**.

The goal is to identify whether trader behavior and profitability vary across different market sentiment conditions such as **Fear** and **Greed**.

---

## Objective
The main objectives of this project are:

- Analyze trader profitability under different market sentiment conditions
- Compare trading performance during **Fear** vs **Greed**
- Study the effect of sentiment on:
  - trade profitability
  - trade size
  - trade direction
  - trader behavior
- Generate actionable insights that can support smarter trading strategies

---

## Datasets Used

### 1. Historical Trader Data
Contains trade-level historical data from Hyperliquid.

Important fields used:
- Account
- Coin
- Execution Price
- Size Tokens
- Size USD
- Side
- Timestamp IST
- Direction
- Closed PnL
- Fee

### 2. Bitcoin Fear & Greed Index
Contains daily Bitcoin market sentiment.

Important fields used:
- Date
- Classification
- Value

---

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

---

## Workflow

The project was completed in the following stages:

1. **Data Loading**
   - Import both datasets

2. **Data Cleaning**
   - Standardize column names
   - Convert date/time columns
   - Handle null values and duplicates
   - Convert numeric fields properly

3. **Feature Engineering**
   - Create trade date field
   - Create profit/loss indicators
   - Create trade value and bucketed features

4. **Data Merging**
   - Merge trader data with sentiment data using trade date

5. **Exploratory Data Analysis**
   - Sentiment-wise performance analysis
   - Trader-level analysis
   - Coin-wise analysis
   - Direction-wise analysis
   - Time-based trend analysis

6. **Statistical Testing**
   - T-test between Fear and Greed profitability

7. **Output Generation**
   - Summary tables
   - Visualizations
   - Final insights

---

## Key Analyses Performed

- Number of trades by sentiment
- Average PnL by sentiment
- Win rate by sentiment
- Coin-wise profitability
- Direction-wise profitability
- Top trader performance
- Daily PnL trend
- Statistical significance testing

---

## Project Outputs

The notebook generates the following output files:

- `sentiment_summary.csv`
- `trader_performance_summary.csv`
- `coin_performance.csv`
- `direction_performance.csv`
- `daily_pnl_summary.csv`

It also generates the following visualizations:

- Trades by sentiment
- Average PnL by sentiment
- Win rate by sentiment
- PnL distribution boxplot
- Coin-wise profitability
- Direction-wise profitability
- Top traders chart
- Daily PnL trend

---

## How to Run the Project

### Step 1
Place these files in the same folder as the notebook:
- `historical_data.csv`
- `fear_greed_index.csv`

### Step 2
Install dependencies:
```bash
pip install -r requirements.txt
```

### Step 3
Run the notebook:
```bash
jupyter notebook trader_sentiment_analysis.ipynb
```

### Step 4
Execute all cells in order.

---

## Folder Structure

```bash
submission/
│
├── trader_sentiment_analysis.ipynb
├── README.md
├── requirements.txt
├── final_report.pdf
├── historical_data.csv
├── fear_greed_index.csv
├── sentiment_summary.csv
├── trader_performance_summary.csv
├── coin_performance.csv
├── direction_performance.csv
└── daily_pnl_summary.csv
```

---

## Key Takeaways

This project demonstrates how **market sentiment data** can be combined with **real trader performance data** to identify useful patterns in:

- profitability
- behavior
- trade direction
- asset preference
- strategy opportunities

Such analysis can help improve **data-driven trading decisions** and support future work in predictive analytics and strategy optimization.

---

## Future Improvements

Possible future enhancements include:

- Predictive modeling
- Trader clustering / segmentation
- Sentiment-based strategy recommendation
- Dashboard deployment using Streamlit / Power BI
- Risk scoring and regime detection

---

## Author
**Aniruddha Kirtiwar**
