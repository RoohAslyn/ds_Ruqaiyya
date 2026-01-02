# 📊 Trader Behavior vs Market Sentiment Analysis

## 📌 Project Overview
This project analyzes the relationship between **cryptocurrency trader behavior** and **market sentiment (Fear & Greed Index)** using historical trading data from Hyperliquid.  
The objective is to determine whether traders **align with market psychology or diverge from it**, and to uncover **behavioral patterns and hidden signals** that can guide smarter, risk-aware trading strategies.

---

## 🎯 Objectives
- Analyze how **profitability, volume, risk, and leverage behavior** vary across Fear and Greed regimes
- Identify **contrarian opportunities** during extreme sentiment conditions
- Detect **risk traps** caused by overconfidence during market euphoria
- Provide **explainable insights** instead of black-box predictions

---

## 📂 Repository Structure
ds_rooh_aslyn/
├── notebook_1.ipynb
├── csv_files/
│ ├── historical_data.csv
│ ├── fear_greed_index.csv
│ └── merged_trader_sentiment.csv
├── outputs/
│ ├── pnl_vs_sentiment.png
│ └── risk_vs_sentiment.png
├── ds_report.pdf
└── README.md


## 📁 Datasets Used
1. **Historical Trader Data (Hyperliquid)**  
   - Includes timestamps, trade size (USD), direction, and closed PnL

2. **Bitcoin Fear & Greed Index**  
   - Daily sentiment score (0–100) and classification (Fear / Greed)

---

## 🧠 Methodology

### 1️⃣ Data Preparation
- Parsed trade timestamps and aligned them to daily granularity
- Merged trader behavior with daily market sentiment

### 2️⃣ Feature Engineering
Daily behavioral metrics computed:
- **Daily PnL** – total profit or loss per day  
- **Trading Volume** – total USD traded  
- **Trade Count** – activity level  
- **PnL Volatility** – risk and emotional trading indicator  
- **Leverage / Exposure Proxy** – relative aggressiveness based on trade sizing  

### 3️⃣ Sentiment Alignment Analysis
- Correlation analysis between market sentiment and trading behavior
- Evaluation of alignment vs divergence from crowd psychology

### 4️⃣ Signal Identification
Rule-based behavioral signals:
- **BUY Signal (Fear Buying):**  
  Extreme Fear combined with high trading activity
- **SELL Signal (Greed Trap):**  
  Extreme Greed combined with negative profitability

### 5️⃣ Explainable Machine Learning
- Applied a **Random Forest Regressor** to assess feature importance
- Focused on understanding **what drives profitability**, not prediction accuracy

---

## 📊 Visualizations

### 🔹 Trading Performance vs Market Sentiment
- Compares daily PnL against the Fear & Greed Index
- Highlights BUY and SELL signals
- Shows divergence between sentiment extremes and profitability

### 🔹 Risk Exposure vs Market Sentiment
- Plots trader exposure against sentiment levels
- Colored by daily PnL
- Reveals over-leveraging during Greed and disciplined behavior during Fear

---

## 🔍 Key Insights
- Traders tend to **increase risk during Greed**, often without improved returns
- **Extreme Greed frequently coincides with losses**, indicating overconfidence
- **Fear regimes provide better risk-adjusted opportunities**
- Market sentiment is most effective as a **risk management signal**, not a directional predictor

---

## 🏁 Conclusion
The analysis highlights strong behavioral biases in crypto trading.  
Optimal performance emerges when traders **diverge from crowd emotion**, emphasizing contrarian positioning, disciplined risk management, and sentiment-aware decision-making.

---

## 🔗 Google Colab Notebook
📎 Colab Link: **https://colab.research.google.com/drive/1Paqm-maNduBE0_SM8mxGBi0gKXfENhvp?usp=sharing**
 Access: **Anyone with the link can view**

---

## 🚀 Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy
- Scikit-learn
- Google Colab

---
