# Cryptocurrency Market Volatility Analysis

> Can market fundamentals predict cryptocurrency price volatility?

**Authors:** Siddharth Patel, Dylan Kim, Zihan Yu, Weijie Guan  
**Course:** DS3000 - Northeastern University  
**Date:** Fall 2025

---

## 📊 Overview

This project investigates whether market capitalization and trading volume can predict cryptocurrency price volatility using machine learning models.

---

## 🎥 Project Presentation
**[Watch our 6-minute presentation on YouTube](https://www.youtube.com/watch?v=sJCnnZh-ET0)**

---

## 🎯 Research Questions

1. Are larger coins (BTC, ETH) less volatile than smaller coins?
2. Can we predict volatility using market cap and trading volume?

---

## 📁 Repository Structure
```
├── notebooks/                               # Jupyter notebooks
│   ├── Phase_I_Proposal.ipynb               # Data collection & proposal
│   ├── Phase_II_Data_EDA.ipynb              # Data cleaning & visualizations
│   └── Phase_III_ML_Models.ipynb            # Machine learning models
├── CryptocurrencyAnalysisPresentation.pdf   # Presentation slides
├── CryptocurrencyAnalysisFinalReport.pdf    # Complete final report 
└── README.md                                # Project overview
```

---

## 🔬 Methodology

**Data Source:** CoinMarketCap API (3,376 cryptocurrencies)

**Models Implemented:**
1. **Linear Regression** - MSE: 0.518, R²: 0.0144 (1.44%)
2. **Polynomial Regression (degree 4)** - MSE: 0.525, R²: 0.0215 (2.15%)
3. **Polynomial + Interactions** - MSE: 0.524, R²: 0.0236 (2.36%)

**Implementation:** Custom NumPy functions for regression, sklearn for preprocessing

---

## 📈 Key Findings

### ❌ Market fundamentals CANNOT predict crypto volatility
- All models explained **< 2.4%** of variance
- Over **97.6%** of volatility remains unexplained
- Crypto is driven by sentiment, news, and speculation—not fundamentals

### Why Did Models Fail?
- Missing critical features (social media sentiment, regulatory news, macro conditions)
- Wrong model family (need time-series approaches)
- Crypto markets operate differently than traditional assets

---

## 🚀 Technologies

`Python` `NumPy` `Pandas` `Matplotlib` `Seaborn` `scikit-learn` `SciPy`

---

## 🔧 Installation
```bash
git clone https://github.com/apulza/CryptocurrencyAnalysis.git
cd CryptocurrencyAnalysis
```

**API Key Required:** Get free key at [CoinMarketCap API](https://coinmarketcap.com/api/)

---

## 💡 Future Work

- Incorporate sentiment analysis (Twitter, Reddit)
- Implement time-series models (GARCH, LSTM)
- Add macroeconomic indicators (VIX, interest rates)
- Build sector-specific models (DeFi vs meme coins)

---

## ⚠️ Disclaimer

**This is academic research, NOT financial advice.**

Cryptocurrency investments are highly speculative and risky. Our models' poor performance (R² < 2.4%) demonstrates crypto markets are fundamentally unpredictable using simple market metrics. Always consult financial professionals and only invest money you can afford to lose.

---
