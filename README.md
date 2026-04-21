# -Trader-Performance-vs-Market-Sentiment-Data_analysis
Analyze how market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid. Your goal is to uncover patterns that could inform smarter trading strategies.
# 📊 Market Sentiment vs Trader Behavior Analysis (Hyperliquid)

## 🧠 Objective

This project analyzes how **market sentiment (Fear vs Greed)** influences **trader behavior and performance** on Hyperliquid.
The goal is to uncover patterns that can help design **better trading strategies**.

---

## 📁 Datasets

### 1. Bitcoin Market Sentiment (Fear/Greed)

* Columns: `Date`, `Classification`
* Values: Fear / Greed

### 2. Hyperliquid Historical Trader Data

* Key fields:

  * `account`
  * `symbol`
  * `execution price`
  * `size`
  * `side` (LONG/SHORT)
  * `time` / `Timestamp IST`
  * `closedPnL`
  * `leverage`

---

## ▶️ How to Run

### 🔹 Step 1: Place Datasets

Put your datasets inside the project folder:

```
fear_greed_index.csv
historical_data.csv
```

---

### 🔹 Step 2: Run Analysis Script

```bash
python analysis.py
```

This will:

* Clean and merge datasets
* Generate trader metrics
* Perform sentiment-based analysis
* Output insights and charts

---

## 🔄 Data Processing Steps

* Convert timestamps (IST → datetime)
* Align both datasets by **daily date**
* Handle missing values and duplicates
* Merge sentiment with trading data

---

## 📈 Key Features Engineered

* Daily PnL per trader
* Win rate
* Number of trades per day
* Average trade size
* Leverage usage
* Long/Short ratio

---

## 📊 Analysis Performed

### ✔ Performance vs Sentiment

* PnL comparison (Fear vs Greed)
* Win rate differences
* Drawdown proxy

### ✔ Behavioral Analysis

* Trade frequency changes
* Leverage variation
* Position sizing
* Long vs Short bias

### ✔ Trader Segmentation

* High vs Low leverage traders
* Frequent vs Infrequent traders
* Consistent vs Inconsistent traders

---

## 🔍 Key Insights

* Fear markets show **higher volatility** and inconsistent performance
* Greed markets favor **trend-following strategies**
* High leverage increases both **risk and reward**
* Overtrading reduces overall profitability

---

## 💡 Strategy Recommendations

1. **During Fear Periods**

   * Reduce leverage
   * Avoid overtrading
   * Focus on risk management

2. **During Greed Periods**

   * Follow market trends (long bias)
   * Use moderate leverage
   * Increase participation cautiously

---

## 🤖 Bonus (Optional)

* Predict trader profitability using ML models

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Streamlit

---

## 📌 Notes

* Ensure timestamp format is correctly parsed:

  ```
  %d-%m-%Y %H:%M
  ```
* Watch out for **outliers in PnL**
* Always compare **mean vs median** for reliable insights


