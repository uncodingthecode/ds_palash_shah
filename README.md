# 📈 Trading Behavior vs Market Sentiment — Palash Shah

This project analyzes how trading behavior (profitability, risk, volume, leverage) aligns or diverges from overall **market sentiment** using the **Fear & Greed Index (FGI)**.  
The analysis combines historical trading data with sentiment indicators to uncover hidden trends and insights for smarter trading strategies.

---

## 📂 Repository Structure
```
├── csv_files/
│   ├── fear_greed_index.csv
│   ├── historical_data
│   └── merged_data.csv
├── output/
│   ├── README.md
│   ├── ds_Report.pdf
│   └── notebook_1.ipynb
├── notebook_1.ipynb              # Main Jupyter/Colab notebook with full analysis & EDA
├── trade_fgi_analysis.py          # Script version of the analysis
└── README.md                      # Project overview
```

---

## ⚙️ Features
- **Data Preparation**: Cleaning, timestamp standardization, missing value handling  
- **Exploratory Data Analysis (EDA)**: Summary stats, distributions, correlations  
- **Feature Engineering**: Rolling profit, rolling correlations, risk metrics  
- **Regime Classification**: Market sentiment split into Fear, Neutral, Greed  
- **Performance Analysis**: Sharpe ratio, drawdowns, cumulative P&L  
- **Visualization**: Time-series plots, heatmaps, lagged correlations  

---

## 🚀 Quick Start

### Option A — Run in Google Colab
1. Open [`notebook_1.ipynb`](notebook_1.ipynb) in **Google Colab**.  
2. Upload your trading history CSV and the FGI dataset.  
3. Run all cells to generate outputs and visualizations.  

### Option B — Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/uncodingthecode/ds_palash_shah.git
   cd ds_palash_shah
   ```
2. Create a virtual environment & install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate       # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Run the analysis script:
    ```bash
    python trade_fgi_analysis.py
    ```
    
---

## 📊 Outputs
- Merged Dataset → /outputs/merged_trade_fgi_daily.csv
- Plots & Charts → /outputs/*.png
- Summary Report → /outputs/summary.txt
These outputs provide insights into profitability patterns, sentiment effects, and regime-based performance.

---

## 📌 Notes
- Data is based on a single trader → results may not generalize.
- FGI is daily → not ideal for intraday strategies.
- Validate missing values & currency units before further use.

---

## 👤 Author
Palash Shah
(Currently not accepting any pull request)
