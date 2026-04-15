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

### 2. Data Cleaning
- Handling missing values  
- Formatting dates  
- Organising data by ticker  

### 3. Analysis

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
