# 📊 Simple Pairs Trading & Quantitative Analysis in Python

## 🚀 Overview

This project implements a collection of **quantitative finance techniques** for stock market analysis using Python. It focuses on:

* Pairs Trading (Statistical Arbitrage)
* Cointegration-based strategies
* PCA-based pair selection
* Clustering methods (K-Means, DBSCAN, Agglomerative)
* Financial data collection from Yahoo Finance

This repository serves as a **baseline research framework** for developing and testing trading strategies.

---

## ⚙️ Features

### 📈 1. Data Collection

* Fetch historical stock data using `yfinance`
* Web scraping using `requests` and `BeautifulSoup`
* Support for multiple tickers

---

### 🔗 2. Pair Identification Methods

#### ✔ Cointegration-Based

* Uses statistical tests to find long-term relationships
* Identifies mean-reverting pairs

#### ✔ PCA-Based

* Reduces dimensionality of returns
* Selects pairs based on principal component similarity

#### ✔ Correlation-Based

* Identifies highly correlated stock pairs

---

### 📊 3. Trading Strategy

* Z-score based mean-reversion strategy
* Entry/Exit signals:

  * Long: Z-score < -2
  * Short: Z-score > 2
  * Exit: |Z-score| < 0.5

---

### 🧠 4. Machine Learning (Clustering)

* K-Means
* DBSCAN
* Agglomerative Clustering

Used to group similar stocks and identify potential trading pairs.

---

### 📉 5. Backtesting & Performance

* Simple PnL calculation
* Sharpe ratio estimation
* Portfolio rebalancing (monthly)

---

## 🛠️ Tech Stack

* Python
* pandas
* numpy
* yfinance
* statsmodels
* scikit-learn
* BeautifulSoup

---

## 📂 Project Structure

```
project/
│── data_collection.py
│── pairs_trading_cointegration.py
│── pca_pairs.py
│── clustering_analysis.py
│── backtesting.py
│── README.md
```

---

## ▶️ How to Run

1. Install dependencies:

```bash
pip install pandas numpy yfinance statsmodels scikit-learn beautifulsoup4 requests
```

2. Run scripts:

```bash
python pairs_trading_cointegration.py
python clustering_analysis.py
```

---

## 📌 Example Output

* Identified stock pairs
* Trading signals (long/short/exit)
* Strategy PnL
* Clustering summary table

---

## ⚠️ Limitations

* Uses static Z-score (no rolling window)
* No transaction costs or slippage
* Simplified PnL calculation
* Limited ticker universe
* Some modules are prototype-level
* basic implementation
  

---

## 🎯 Future Improvements

* Rolling window Z-score
* Hedge ratio (OLS regression)
* Full backtesting engine
* Risk management (drawdown, position sizing)
* Integration with advanced methods (e.g., MFDCCA)

---

## 📚 Use Case

This project is ideal for:

* Learning pairs trading
* Academic research baseline
* Experimenting with quantitative strategies
* Comparing with advanced models

---

## 📜 License

This project is for educational and research purposes only.

---

## 🙌 Author

Anil Thapa

---


📉 5. Backtesting & Performance
Simple PnL calculation
Sharpe ratio estimation
Portfolio rebalancing (monthly)
🛠️ Tech Stack
Python
pandas
numpy
yfinance
statsmodels
scikit-learn
BeautifulSoup
📂 Project Structure
project/
│── data_collection.py
│── pairs_trading_cointegration.py
│── pca_pairs.py
│── clustering_analysis.py
│── backtesting.py
│── README.md
▶️ How to Run
Install dependencies:
pip install pandas numpy yfinance statsmodels scikit-learn beautifulsoup4 requests
Run scripts:
python pairs_trading_cointegration.py
python clustering_analysis.py
📌 Example Output
Identified stock pairs
Trading signals (long/short/exit)
Strategy PnL
Clustering summary table

🎯 Future Improvements
Rolling window Z-score
Hedge ratio (OLS regression)
Full backtesting engine
Risk management (drawdown, position sizing)
Integration with advanced methods (e.g., MFDCCA)
📚 Use Case

This project is ideal for:

Learning pairs trading
Academic research baseline
Experimenting with quantitative strategies
Comparing with advanced models
📜 License

This project is for educational and research purposes only.

🙌 Author

Anil Thapa
