# 📊 Stock Data Extractor using yFinance

A Python script to extract historical stock **closing prices** using the [`yfinance`] library. The script reads a list of company tickers from an Excel file and exports the data to a CSV file for further analysis. It also logs failed ticker fetch attempts for review.

---

## ✅ Features

- 📥 Reads a list of company names and tickers from an Excel sheet  
- 🔍 Fetches historical **closing price data** for each ticker  
- 🗃️ Saves the combined data into a CSV file (`stock_data.csv`)  
- 🧾 Logs tickers that failed to download into `failed_tickers.txt`  
- ⏳ Allows configuration of date range for historical data  
- 💼 Supports both Indian and global tickers (e.g., `INFY.NS`, `AAPL`)  

---

## 📁 Input Format (`companies.xlsx`)

The Excel file should contain a sheet (default `Sheet1`) with the following columns:

| Company Name | Ticker   |
|--------------|----------|
| Infosys      | INFY.NS  |
| TCS          | TCS.NS   |
| Apple Inc    | AAPL     |

- `Ticker`: The valid stock symbol recognized by Yahoo Finance.  
- `Company Name`: For identification/logging (not used in fetch itself).  

---

## 🔧 Installation

Ensure Python 3.7+ is installed. Then, install the dependencies:

```bash
pip install pandas openpyxl yfinance

