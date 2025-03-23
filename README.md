# Bitcoin Price Volatility Analysis

This project analyzes the historical volatility of Bitcoin (BTC) using statistical and exploratory methods in R. It investigates whether BTC price swings are statistically significant, how trading volume impacts volatility, and whether seasonal (quarterly) trends affect trading behavior.

---

## 📊 Project Summary

- **Goal:** Assess volatility patterns in Bitcoin daily trading data and test if volume or quarterly trends explain fluctuations.
- **Dataset:** Binance BTC/USDT daily trading data (2,600+ rows from 2017 to 2024), sourced via [CryptoDataDownload](https://www.cryptodatadownload.com/).
- **Tools Used:** R, `tidyverse`, `ggplot2`, `dplyr`, `lubridate`, `scales`
- **Key Output:** Statistical tests, visualizations, and trading insights for crypto analysts and financial modelers.

---

## 📁 Project Structure

```
bitcoin-volatility-analysis/
├── bitcoin-volatility-analysis.Rmd     # R Markdown file with full analysis
├── data/
│   └── Binance_BTCUSDT.csv             # Daily BTC/USDT dataset
```

---

## 📈 Key Analyses

- **Exploratory Data Analysis (EDA)**  
  - Distribution plots of BTC price, volume, and daily price changes  
  - Time series trend charts for BTC closing price and trading volume

- **Volatility Tests**
  - `Wilcoxon Signed-Rank` test for price change deviation from zero
  - `Mann-Whitney U` test comparing high vs. low volume volatility
  - `Fisher’s Exact` test on volume category vs. price movement direction
  - `Paired t-test` comparing Q1 vs. Q4 trading volume

---

## 🔑 Findings

- Bitcoin exhibits **volatility clustering**, with large swings tending to follow other large swings.
- No statistically significant difference in volatility between **high- and low-volume days**.
- **Quarterly patterns** (Q1 vs Q4) do not show significant changes in trading volume.
- Volume is not a strong standalone predictor of BTC price direction.

---

## 📌 Recommendations

- Use **volatility-aware risk management** (e.g., stop-losses, adjusted position sizing).
- Apply **non-parametric models** due to non-normal return distributions.
- Incorporate **external data** (macroeconomic indicators, social sentiment) for better prediction.

---

## 🧠 Future Enhancements

- Extend analysis with machine learning models (e.g., GARCH, ARIMA, LSTM).
- Include data from other exchanges or alternative cryptocurrencies.
- Integrate sentiment analysis from news or social platforms.

---

## 📜 Author

**Jordon Abrams**  
M.S. Data Science (in progress)  
University of Denver

---