# 📈 AdEase Time-Series Forecasting

This repository contains a complete time-series analysis and forecasting pipeline built for the **AdEase dataset**.  
It covers both **Exploratory Data Analysis (EDA)** and **Modeling** stages, leveraging statistical and machine learning approaches for multi-language Wikipedia traffic prediction.

---

## 🧩 Project Overview

The goal of this project is to analyze time-series traffic data from multiple Wikipedia pages (in various languages) and forecast future trends using three modeling approaches:
- **ARIMA** — Autoregressive Integrated Moving Average
- **SARIMAX** — Seasonal ARIMA with Exogenous Factors
- **Prophet** — Facebook’s additive model for trend and seasonality

---

## 📊 Notebooks

| Stage | Description | Colab Link |
|:------|:-------------|:-----------|
| 🧠 **EDA Notebook** | Data cleaning, visualization, and initial time-series decomposition for all representative pages. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1es8O-Ty2oBzPK6wwC4UDU3b68bC9VzM9?usp=sharing) |
| 🔮 **Modeling Notebook** | Stationarity checks, ARIMA/SARIMAX/Prophet modeling, evaluation (MAPE), and model comparison across languages. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13y0h8tMvqw8_c0UUnRJQ2YTZoyvXWODq?usp=sharing) |

---

## 🧠 Key Highlights

- ✅ Automated stationarity checks and differencing  
- ✅ Decomposition of trend, seasonality, and residuals  
- ✅ Unified multi-series pipeline across languages  
- ✅ Model comparison using 30-day MAPE  
- ✅ Insights on best-performing model per page & per language  

---

## 📑 Insights Summary

- **Prophet** achieved the lowest average MAPE across all representative series.  
- **ARIMA** showed stable performance and dominated by count (best on 21 out of 39 pages).  
- **SARIMAX** showed improvement on some series but overall aligned closely with ARIMA.  
- Cross-language behavior revealed unique seasonalities (especially in EN, FR, and JA pages).  

---

## ⚙️ Requirements

- Python 3.8+
- pandas, numpy, statsmodels, prophet, matplotlib, seaborn
- tqdm, pmdarima (for auto-ARIMA)

To install dependencies:
```bash
pip install pandas numpy statsmodels prophet matplotlib seaborn tqdm pmdarima
