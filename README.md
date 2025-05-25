# 📊 fear-greed-vs-trading-performance

**Exploring how crypto market emotions—Fear & Greed—affect real trading outcomes on Hyperliquid.**

---

## 🧠 Project Overview

This project analyzes the relationship between **Bitcoin market sentiment** (Fear & Greed Index) and **trader performance** using real trading data from **Hyperliquid**.

By merging sentiment signals with trading metrics like **PnL**, **trade volume**, and **execution price**, we explore whether **market emotions** influence **profitability and behavior**—and how these insights can drive smarter Web3 trading strategies.

---

## 📁 Datasets Used

Due to file size, datasets are hosted externally:

- 📌 [Fear & Greed Index CSV](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)
- 📌 [Hyperliquid Historical Trades CSV](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)

Please **download and place them** in a `/data` folder before running the analysis.

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas & NumPy
- Matplotlib & Seaborn
- SciPy ( ANNOVA )
- Google Colab Notebook

---

## 📊 Analysis Steps

### 1. **Data Loading & Preprocessing**
- Parsed timestamps, normalized timezones
- Filtered BTC-only trades
- Mapped sentiment labels to numerical scores
- Grouped both datasets by **daily granularity**

### 2. **Data Merging**
- Joined both datasets on the `date` column
- Focused on days with valid trades

### 3. **Feature Engineering**
- Calculated daily metrics:
  - 🔹 `total_volume_usd`
  - 🔹 `avg_execution_price`
  - 🔹 `net_pnl`
  - 🔹 `trade_count`

### 4. **Visual Analysis**
- 📉 Scatter plot: Sentiment Value vs Net PnL  
- 📊 Bar chart: Avg. PnL per Sentiment Category

### 5. **Statistical Testing**
- ✅ ANOVA test to check significance of PnL variation across sentiment classes

---

## 💡 Key Insights

- Traders had **lower average profits** on days with **Extreme Fear**
- Net PnL was significantly **higher during Neutral and Greed** periods
- ANOVA test confirmed that sentiment differences had **statistically significant** effects on PnL (p < 0.05)
- Suggests that sentiment indicators could inform **timing, risk management, or strategy design**

---

## ▶️ How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/Divyansh8791/fear-greed-vs-trading-performance.git
   cd fear-greed-vs-trading-performance
   ```
2. Place the files inside a data/ folder:
   ```bash
   /data
   ├── fear_greed_index.csv
   └── historical_data.csv
   ```
3. Run the Colab Notebook ( in google colab ):
   ```bash
   Bitcoin_trader_analysis.ipynb
   ```
---
## Feel free to reach out for any questions:
💼 LinkedIn : [Divyansh Dhiman](https://www.linkedin.com/in/divyansh-dhiman)
