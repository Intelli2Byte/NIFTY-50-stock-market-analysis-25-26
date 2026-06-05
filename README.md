# 📈 NSE NIFTY50 Stock Market Exploratory Data Analysis (EDA)

> **Dataset Update Notice**
>
> This project uses an updated NIFTY50 stock market dataset containing historical market data from **04 June 2025 to 03 June 2026**.
>
> The dataset includes daily price movements, trading activity, technical indicators, volatility metrics, trend signals, and performance statistics engineered specifically for stock market analysis and predictive modeling.
>
> **Date Range:** 2025-06-04 → 2026-06-03  
> **Market:** NSE NIFTY50  
> **Frequency:** Daily Trading Data  
> **Dataset Version:** Updated 2025–2026 Release

## Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on the NIFTY50 stock market dataset to understand market behavior, trading activity, technical indicators, risk metrics, and price trends.

The analysis includes data cleaning, statistical summaries, missing value treatment, technical indicator evaluation, correlation analysis, visualization dashboards, and statistical testing.

---

## Dataset

**Source:** Kaggle

🔗 Dataset Link: https://www.kaggle.com/datasets/nehamaurya1/nse-dataset-2025-2026-stock-market-prediction

### Dataset Description

The dataset contains historical NIFTY50 market data along with engineered technical indicators commonly used in quantitative finance and algorithmic trading.

### Key Features

#### Price Information

* Open
* High
* Low
* Close

#### Trading Activity

* Shares Traded
* Turnover (Crores)
* Volume Ratio
* Volume Moving Average

#### Technical Indicators

* SMA (5, 10, 20, 50)
* EMA (5, 10, 20, 50)
* RSI (14)
* MACD
* MACD Signal
* MACD Histogram
* ATR (14)
* Bollinger Bands
* Volatility Indicators

#### Performance Metrics

* Daily Returns
* Cumulative Returns
* Drawdown Percentage
* Gap Percentage

#### Market Signals

* Trend Classification
* MACD Crossovers
* RSI Signals

---

# Project Objectives

The primary objectives of this analysis are:

* Understand historical price movement patterns
* Analyze market volatility and risk
* Evaluate technical indicators
* Study trading volume behavior
* Identify trend distributions
* Examine relationships between technical indicators
* Perform statistical analysis on returns
* Build a foundation for future stock price prediction models

---

# Technologies Used

## Programming Language

* Python 3.x

## Libraries

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn
* Plotly

### Statistical Analysis

* SciPy

---

# Data Preprocessing

## Date Handling

* Converted Date column to datetime format
* Sorted records chronologically

## Missing Value Treatment

### Technical Indicators

Applied Forward Fill (FFill) followed by Backward Fill (BFill) to:

* SMA
* EMA
* RSI
* MACD
* ATR
* Bollinger Bands
* Volatility Metrics

### Volume-Based Features

Applied:

* Forward Fill
* Backward Fill

for:

* Volume_MA_20
* Volume_Ratio
* Turnover_MA_20

### Return Features

Filled missing values with zero:

* Daily_Return_Pct
* Gap_Pct
* Gap_Up_Down
* Change_from_Prev_Close

### Categorical Features

Handled missing values in:

* Trend
* MACD_Crossover

---

# Exploratory Data Analysis

## 1. Dataset Overview

Performed:

* Dataset shape analysis
* Date range inspection
* Price range analysis
* Maximum drawdown evaluation
* Data type inspection

---

## 2. Descriptive Statistics

Generated descriptive statistics for:

### Price Variables

* Open
* High
* Low
* Close
* Daily Returns
* Cumulative Returns
* Drawdown Percentage

### Volume Variables

* Shares Traded
* Turnover
* Volume Ratio

### Technical Indicators

* RSI
* MACD
* ATR
* Volatility

---

## 3. Price Movement Analysis

Analyzed:

* Starting Price
* Ending Price
* Total Return
* Highest Price
* Lowest Price
* Average Close Price
* Price Volatility
* Maximum Daily Gain
* Maximum Daily Loss
* Maximum Drawdown

---

## 4. Trading Activity Analysis

Calculated:

* Total Trading Days
* Up Days vs Down Days
* Win Rate
* Average Daily Volume
* Maximum Volume
* Average Turnover
* Total Turnover

---

## 5. Technical Indicator Analysis

Evaluated:

### RSI Analysis

* Current RSI
* Average RSI
* Overbought Days (RSI > 70)
* Oversold Days (RSI < 30)

### MACD Analysis

* Current MACD
* Signal Crossovers
* Momentum Trends

### Volatility Analysis

* Average Volatility
* Current ATR

---

## 6. Trend Analysis

Examined market trend distribution using:

* Bullish Trends
* Bearish Trends
* Sideways Trends

---

# Visualizations

The project includes multiple visualization dashboards:

## Price Analysis

### Price with Moving Averages

Displays:

* Close Price
* SMA 20
* SMA 50
* Trend Zones

---

## Volume Analysis

Displays:

* Daily Trading Volume
* Volume Moving Average
* Up-Day vs Down-Day Activity

---

## Return Distribution

Visualizes:

* Daily Return Histogram
* Mean Return
* Return Frequency

---

## Cumulative Return Analysis

Shows:

* Investment Growth
* Positive and Negative Return Zones

---

## RSI Indicator

Highlights:

* Overbought Regions
* Oversold Regions
* Momentum Strength

---

## MACD Dashboard

Includes:

* MACD Line
* Signal Line
* Histogram

---

## Bollinger Bands

Visualizes:

* Upper Band
* Middle Band
* Lower Band
* Price Position

---

## Volatility Analysis

Displays:

* Rolling 20-Day Volatility

---

## Drawdown Analysis

Shows:

* Historical Drawdown
* Maximum Risk Exposure

---

## Volume Ratio Analysis

Compares:

* Current Volume
* Historical Average Volume

---

## Monthly Returns Heatmap

Provides:

* Monthly Performance
* Seasonal Market Behavior

---

## Trend Distribution

Visualized using pie charts.

---

# Correlation Analysis

Generated a correlation matrix using:

* Close Price
* Daily Returns
* Trading Volume
* Turnover
* RSI
* MACD
* ATR
* Volatility
* Volume Ratio

### Purpose

* Identify strong relationships
* Detect multicollinearity
* Understand feature dependencies

---

# Statistical Testing

## Normality Test

Applied:

### D'Agostino and Pearson Normality Test

Outputs:

* Test Statistic
* P-value
* Normality Conclusion

---

## Distribution Analysis

Computed:

### Skewness

Measures asymmetry of return distribution.

### Kurtosis

Measures tail risk and extreme events.

---

# Key Insights

The analysis provides insights into:

* Historical market performance
* Momentum behavior
* Risk exposure
* Volatility patterns
* Volume dynamics
* Technical indicator effectiveness
* Trend persistence

These findings can be used as a foundation for:

* Stock Price Forecasting
* Machine Learning Models
* Quantitative Trading Strategies
* Risk Management Systems

---

# Future Work

Potential extensions include:

* ARIMA Forecasting
* Prophet Forecasting
* Random Forest Regression
* XGBoost Models
* LSTM Deep Learning Models
* Portfolio Optimization
* Trading Signal Generation
* Backtesting Strategies

---

# Repository Structure

```text
├── data/
│   └── NIFTY50.csv
│
├── notebooks/
   └── NSE_NIFTY50_EDA.ipynb

---

# Author

**Neha Maurya**

Data Science | Machine Learning | Financial Analytics

GitHub: https://github.com/your-github-username

---

# License

This project is intended for educational, research, and portfolio purposes.
