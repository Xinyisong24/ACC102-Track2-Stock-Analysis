# Stock Analysis Project: AAPL, MSFT, GOOGL
ACC102 Track 2 – GitHub Data Analysis Project

## 1. Project Overview
This project analyzes the historical stock performance of three major U.S. technology companies: Apple (AAPL), Microsoft (MSFT), and Alphabet (GOOGL). The analysis includes data cleaning, return calculation, risk measurement, visualization, and correlation analysis to help investors understand price trends and risk characteristics.

## 2. Dataset Information
- **Data Source**: WRDS
- **Time Period**: 2025.04 – 2026.04 (1 year)
- **Stocks**: AAPL, MSFT, GOOGL
- **Key Variables**:
  - date: trading date
  - TICKER: stock ticker
  - PRC: closing price
  - VOL: trading volume
  - RET: daily return
- **File**: stock_data.csv

## 3. Methods & Workflow
1. Load and clean data
2. Convert date format and remove missing values
3. Calculate daily returns
4. Plot closing price trends
5. Compute annualized volatility and maximum drawdown
6. Analyze monthly average closing prices
7. Calculate return correlation and plot heatmap

## 4. Key Findings
- All three tech stocks show strong positive return correlation.
- Volatility and drawdown reflect different risk levels.
- Monthly price trends show similar sector-wide movement.
- Correlation heatmap confirms strong co‑movement among tech stocks.

## 5. How to Run
1. Ensure `stock_data.csv` is in the same folder as the notebook
2. Install required packages:
   pandas numpy matplotlib seaborn
3. Run all cells in `StockAnalysis.ipynb` sequentially

## 6. Files in Repository
- StockAnalysis.ipynb: main analysis notebook
- stock_data.csv: dataset
- README.md: project documentation

## 7. Limitations & Improvements
- Limitations: 1‑year data only; no macroeconomic factors included
- Improvements: add more stocks; extend time range; include risk‑adjusted return metrics