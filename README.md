# Stock Analysis: AAPL, MSFT, GOOGL
ACC102 Track 2 – GitHub Data Analysis Project

## 1. Problem & User
This project analyzes the historical stock performance of three major U.S. tech companies (AAPL, MSFT, GOOGL) to identify price trends, risk metrics, and return correlations. The target users include finance students, investors, or anyone interested in understanding basic financial data analysis using Python.

## 2. Data
- **Source**: WRDS (Wharton Research Data Services)
- **Time Period**: 2023-12-31 to 2024-12-31 (1 full year of trading data)
- **Key Fields Used**:
  - `date`: Trading date
  - `TICKER`: Stock ticker symbol
  - `PRC`: Daily closing price
  - `RET`: Daily simple return
- **File Name**: `stock_data.csv`

## 3. Methods (Main Python Steps)
1. **Library Import**: Load `pandas` for data manipulation, `numpy` for calculations, and `matplotlib/seaborn` for visualization.
2. **Data Loading & Cleaning**: Read the CSV file, parse datetime objects, and drop missing values in critical columns (`PRC`, `RET`).
3. **Return Calculation**: Compute daily percentage changes of closing prices grouped by stock ticker.
4. **Risk Analysis**: Calculate annualized volatility (standard deviation × $\sqrt{252}$) and maximum drawdown (worst peak-to-trough decline).
5. **Visualization**: Generate line plots for price trends, bar charts for risk metrics, and a heatmap for return correlation matrix.

## 4. Key Findings (3-5 bullets)
- All three tech stocks exhibit **strong positive correlations** in daily returns.
- **Volatility varies**: GOOGL has the highest annualized volatility (0.2808), indicating higher risk.
- **Trend consistency**: Monthly price movements show similar sector-wide upward trends during the period.
- **Risk measurement**: MSFT shows the smallest maximum drawdown (-0.1548), making it relatively the most stable in terms of loss severity.

## 5. How to run
1. Ensure the dataset file `stock_data.csv` is placed in the same directory as the notebook.
2. Install required packages: `pandas`, `numpy`, `matplotlib`, `seaborn`.
3. Open `StockAnalysis.ipynb` and run all cells sequentially.
4. Check the output cells for printed results (risk metrics, correlation matrix) and generated visualizations.

## 6. Limitations & next steps
- **Limitations**:
  - The analysis is based on only **one year** of data, which may not reflect long-term market patterns.
  - No macroeconomic factors (e.g., interest rates, GDP) or company fundamental data (e.g., P/E ratio) are included.
  - The study focuses solely on price and return data; financial ratios are omitted.
- **Next steps**:
  - Extend the time range to include 3-5 years of historical data for deeper insight.
  - Incorporate macroeconomic indicators to analyze external market impacts.
  - Calculate risk-adjusted performance metrics (e.g., Sharpe Ratio) for a comprehensive evaluation.
