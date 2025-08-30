# 📑 Assignment Report: Trader Performance vs Market Sentiment

## 1. Introduction

This project explores the relationship between trader performance and market sentiment using real trading and sentiment data.

* **Dataset:** Includes trade-level data (timestamps, trade side, PnL, size, fees, coin) and sentiment data (Fear & Greed Index).
* **Objective:** *To explore how trader performance varies across different market sentiment conditions (Fear, Greed, Neutral, Extreme Fear, Extreme Greed) and uncover patterns that can guide smarter trading strategies.*

---

## 2. Methodology

### 📂 Data Sources

* `historical_data.csv` → Trade-level data
* `fear_greed_index.csv` → Sentiment index data

###  Data Cleaning

* Checked for missing values → None found 
* Converted timestamps to proper datetime objects
* Extracted dates and merged both datasets on **date**

###  EDA Approach

* Distribution of trades across sentiment phases
* Aggregate trader performance (PnL) by sentiment
* Side-wise (BUY/SELL) profitability analysis
* Trade size & fee comparison across sentiment phases
* Identified top/bottom performing traders
* Analyzed most traded coins

---

## 3. Findings & Insights

###  Sentiment Distribution

* Fear is dominant (781 days) compared to Greed (633 days).
* Extreme Fear & Extreme Greed are rare but influential.

###  Trader Profitability by Sentiment

* **Fear → Most profitable** (PnL ≈ **1.78M**)
* **Extreme Greed → Highly profitable** (PnL ≈ **1.15M**, avg PnL ≈ **205/trade**)
* **Extreme Fear → Very risky** (Longs lose, Shorts barely survive)
* **Neutral → Low activity & minimal returns**

### 📈 Side-Wise Strategy

* In **Fear** → Longs dominate (avg **+210** per trade)
* In **Greed** → Shorts dominate (avg **+89** per trade)
* In **Extreme Greed** → Shorts dominate strongly (avg **+288** per trade)
* In **Extreme Fear** → Only Shorts profitable

 **Rule of Thumb:**

* Fear = Go **Long** ✅
* Greed = Go **Short** ✅
* Extreme Fear = Avoid Longs ⚠️

###  Trade Size & Fees

* Biggest trades in **Fear** (\~\$5.7k avg size, highest fees)
* Traders bet bigger under Fear → higher risk & higher reward

###  Trader Performance

* Top trader earned **1.47M** overall
* Majority of traders earn small or lose small amounts → profits concentrated in few hands

###  Most Traded Coins

* Dominant: **BTC, ETH, @107, kPEPE, kBONK**
* Meme tokens are most active during Greed phases

---

## 4. Hidden Patterns

* Profitability is **sentiment-dependent** (Fear = Longs win, Greed = Shorts win).
* Trade sizes **increase under Fear**, signaling higher confidence in rebounds.
* **Extreme Fear is a trap** → Long traders expect bottoms but usually lose.
* **Few traders dominate profits**, suggesting trading is not evenly rewarding.

---

## 5. Strategic Insights

✅ **Sentiment-driven trading strategy:**

* Fear → Bias towards Long positions
* Greed → Bias towards Short positions
* Avoid heavy longs in Extreme Fear

✅ **Risk Management:**

* Use smaller trade sizes in extreme sentiment conditions

✅ **Trader Profiling:**

* Analyze top performers to replicate successful strategies

✅ **Coin Choice:**

* Stick to BTC & ETH for stability
* Meme tokens only during Greed phases

---

## 6. Conclusion

* Market sentiment plays a **direct role** in trader performance.
* Smarter strategies can be built by aligning trading direction with sentiment.
* **Fear-driven Longs** and **Greed-driven Shorts** are statistically superior.
* **Extreme Fear** is consistently dangerous for Long traders.
