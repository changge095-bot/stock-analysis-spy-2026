# 📊 Stock Performance Analysis with Benchmark (SPY)

## 📌 Project Overview
This project analyses the stock performance of three major companies — **Apple (AAPL), Microsoft (MSFT), and Tesla (TSLA)** — using data extracted from WRDS (CRSP database).  

The analysis focuses on:
- Price trends  
- Return behaviour  
- Risk (volatility)  

Additionally, the **S&P 500 ETF (SPY)** is included as a **market benchmark**, allowing for a more meaningful comparison of individual stock performance against the overall market.

---

## 🎯 Objectives
The main objectives of this project are:
- To understand how different stocks perform over time  
- To compare return and risk across companies  
- To evaluate stock performance relative to the market benchmark (SPY)  
- To provide insights for beginner investors  

---

## 🗂️ Data Source
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

## ⚙️ Methodology

### 1. Data Extraction
Data is extracted using SQL queries from WRDS.

### 2. Data Cleaning
- Handling missing values  
- Formatting dates  
- Organizing data by ticker  

### 3. Analysis

#### 📈 Price Analysis
- Visualizes stock price trends over time  

#### 📊 Return Analysis
- Calculates daily returns  
- Compares average returns across stocks  

#### ⚠️ Risk Analysis
- Measures risk using standard deviation of returns  
- Higher standard deviation = higher risk  

---

## 🧩 Functions Used

To improve code structure and reusability, functions are implemented:

### ✔️ Plot Function
```python
def plot_time_series(data, value_col, title, y_label):
