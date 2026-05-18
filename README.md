# 📈 TSLA Stock Analysis — End-to-End Data Science Project

End-to-end Data Science project analyzing **Tesla Inc. (TSLA)** daily stock prices from **2021 to 2026** — from raw data to ML predictions and visual dashboards.

---

## 📌 Project Overview

| | |
|---|---|
| **Stock** | Tesla Inc. (TSLA) |
| **Data** | Daily OHLCV prices, 2021–2026 (~1,300 trading days) |
| **Goal** | EDA → Feature Engineering → ML Prediction → Evaluation |
| **Best Model** | Gradient Boosting (highest directional accuracy ~50%) |

---

## 🛠️ Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📊 Steps Covered

1. **Environment Setup** — Library imports and plot configuration
2. **Data Ingestion & Cleaning** — Parsing dates, fixing types, handling nulls
3. **Exploratory Data Analysis** — Monthly/annual returns, volatility, distributions
4. **Feature Engineering** — Moving averages (MA20, MA50, MA200), Bollinger Bands, RSI, MACD
5. **ML Dataset Preparation** — Lag features, train/test split (time-series aware)
6. **Model Training & Evaluation** — Linear Regression, Random Forest, Gradient Boosting
7. **Final Dashboard** — Full summary visualization

---

## 🔍 Key Findings

- TSLA has **~65% annualised volatility** — roughly 3× the S&P 500
- **2022** was the worst year (–65%); **2023** had the strongest recovery (+101.7%)
- **Close price and lag features** dominate feature importance — strong momentum effect
- Directional accuracy hovers near **~50%** — consistent with efficient market behaviour
- **Gradient Boosting** achieved the best directional accuracy among all models

---

## 📉 Model Comparison

| Model | RMSE | Directional Accuracy |
|-------|------|----------------------|
| Linear Regression | ~$11.8 | ~47% |
| Random Forest | ~$15.0 | ~44% |
| Gradient Boosting | ~$15.8 | ~50% ✅ Best |

---

## 📁 Files

| File | Description |
|------|-------------|
| `TSLA_Stock_Analysis.ipynb` | Main project notebook |
| `TSLA.csv` | Raw OHLCV dataset |
| `outputs/step2_raw_data.png` | Price & volume sanity check |
| `outputs/step3a_returns.png` | Monthly & annual returns chart |
| `outputs/step3b_distribution.png` | Return distribution & volatility |
| `outputs/step4_features.png` | Engineered features & correlation heatmap |
| `outputs/step6_evaluation.png` | Model evaluation & feature importances |
| `outputs/step7_dashboard.png` | Final summary dashboard |

---

## 📷 Output Previews

### Raw Price & Volume
![Raw Data](outputs/step2_raw_data.png)

### Returns Analysis
![Returns](outputs/step3a_returns.png)

### Distribution & Volatility
![Distribution](outputs/step3b_distribution.png)

### Engineered Features
![Features](outputs/step4_features.png)

### Model Evaluation
![Evaluation](outputs/step6_evaluation.png)

### Final Dashboard
![Dashboard](outputs/step7_dashboard.png)

---

## ⚙️ Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/your-username/TSLA-Stock-Analysis.git
cd TSLA-Stock-Analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook TSLA_Stock_Analysis.ipynb
```

---

## ⚠️ Limitations

- No sentiment or news data included
- Models use close price as a feature — requires care in live deployment
- No transaction cost or slippage modelling

---

## 🚀 Next Steps

- Add NLP sentiment scores from news/social media
- Implement LSTM for sequence-aware predictions
- Backtest a moving-average crossover strategy

---

## 📄 License
MIT
