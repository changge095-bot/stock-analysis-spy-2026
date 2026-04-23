# Stock Performance Analysis with Benchmark (SPY)

## Project Overview
This project analyses the stock performance of three major companies — **Apple (AAPL), Microsoft (MSFT), and Tesla (TSLA)** — using data from WRDS (CRSP database).  

The analysis focuses on:
- Price trends  
- Return behaviour  
- Risk (volatility)  

Additionally, the **S&P 500 ETF (SPY)** is included as a **market benchmark**, allowing for a more meaningful comparison of individual stock performance against the overall market.

---

## Objectives
The main objectives of this project are:
- To analyse stock price movements over time  
- To compare return and risk across companies  
- To evaluate stock performance relative to the market benchmark (SPY)  
- To provide insights for beginner investors  

---

## Data Source
- **WRDS (Wharton Research Data Services)**  
- **CRSP Daily Stock File (crsp.dsf)**  
- Selected variables:
  - Price (`prc`)
  - Return (`ret`)
  - Volume (`vol`)

Stocks included:
- AAPL  
- MSFT  
- TSLA  
- SPY (Benchmark)

---

## Methodology

### 1. Data Extraction
Data is extracted using SQL queries from WRDS.
The dataset includes daily stock data for AAPL, MSFT, TSLA, and SPY in 2023.

### 2. Data Cleaning
The dataset was cleaned to ensure consistency and accuracy:

Handling missing values
Converting date format
Transforming variables into numeric values
Sorting data by ticker and date
Removing invalid observations
Converting negative prices to absolute values

### 3. Function Design
To improve efficiency and reduce repetition, reusable functions were implemented:

- plot_time_series()
- Generates consistent time-series visualisations (price & volatility)
- calculate_metrics()
- Computes:
- average return
- risk (standard deviation of returns)

This improves code readability and structure.

### 4. Analysis

#### Price Analysis
- Visualizes stock price trends over time  

#### Return Analysis
- Calculates daily returns  
- Compares average returns across stocks  

#### Risk Analysis
- Measures risk using standard deviation of returns  
- Higher standard deviation = higher risk  

---
## Key Findings
- TSLA provides the highest return but also exhibits the highest volatility, indicating a high risk–high return profile  
- MSFT demonstrates stable and consistent performance with relatively low risk  
- AAPL shows balanced performance in terms of both return and risk  

### Benchmark (SPY)
- TSLA outperforms SPY in returns but carries significantly higher risk  
- AAPL and MSFT show performance closer to SPY, suggesting more stable investment behaviour  
- SPY represents overall market performance and serves as a useful benchmark for comparison

## How to Run
1. Open the Jupyter Notebook file (`notebook.ipynb`)
2. Ensure required libraries are installed (pandas, matplotlib, wrds)
3. Connect to WRDS using your account
4. Run all cells in order:
   - Data extraction
   - Data cleaning
   - Analysis and visualisation

Note: WRDS access is required to reproduce the results.

## Demo
This project is implemented as a Jupyter Notebook.

All analysis, visualisations, and results can be viewed directly in:
- `notebook.ipynb`

## Conclusion
This project highlights the importance of evaluating both return and risk when analysing stock performance.  

While TSLA may attract investors seeking higher returns, it also involves greater volatility and risk. In contrast, AAPL and MSFT provide more stable investment options.  

The inclusion of SPY as a benchmark allows for a clearer comparison with overall market performance, improving the depth and reliability of the analysis.  

## Tools
- Python  
- Jupyter Notebook  
- Pandas  
- Matplotlib  
- WRDS  

## Author
**Name:** Chang Ge  
**University:** Xi’an Jiaotong-Liverpool University  
**Course:** ACC102 Financial Data Analysis  
