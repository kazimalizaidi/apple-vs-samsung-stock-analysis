# 📈 Apple vs Samsung Stock Performance Analysis (2021–2026)

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-4C72B0)
![SciPy](https://img.shields.io/badge/SciPy-Statistical%20Analysis-8CAAE6?logo=scipy)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?logo=googlecolab)

---

# 📖 Project Overview

This project presents a comprehensive comparative analysis of the historical stock performance of **Apple Inc. (AAPL)** and **Samsung Electronics** using monthly stock market data from **January 2021 to January 2026**.

The objective of this project is to apply **Business Analytics** and **Financial Data Analysis** techniques to evaluate the performance, growth, volatility, and investment potential of two of the world's largest technology companies.

The analysis was performed entirely in **Python** using **Google Colab**, demonstrating practical applications of data analytics, financial analysis, visualization, and statistical testing.

This project includes:

- 📈 Stock Performance
- 💹 Monthly Returns
- 📊 Moving Averages
- ⚡ Volatility
- 📦 Trading Volume
- 📉 Risk vs Return
- 📐 Sharpe Ratio (Risk-Adjusted Return)
- 📈 Compound Annual Growth Rate (CAGR)
- 📉 Maximum Drawdown
- 📊 Statistical Testing

---

## 📂 Dataset

| Feature | Details |
|---------|---------|
| Companies | Apple & Samsung |
| Period | Jan 2021 – Jan 2026 |
| Frequency | Monthly |
| Records | 60+ Months |
| Variables | Price, Open, High, Low, Volume, Change % |

The dataset was cleaned and validated before performing the analysis.

**Note:** Apple's price is denominated in USD and Samsung's in KRW. Raw price levels (max/min/mean) are not directly comparable across the two companies - only percentage-based metrics (returns, CAGR, volatility, Sharpe Ratio, drawdown) should be compared directly.

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|----------|
| 🐍 Python | Programming |
| 🐼 Pandas | Data Analysis |
| 🔢 NumPy | Numerical Computing |
| 📊 Matplotlib | Visualization |
| 🎨 Seaborn | Statistical Charts |
| 📚 SciPy | Statistical Testing |
| ☁️ Google Colab | Development |

---

## 📸 Key Visualizations

### 📈 Normalized Stock Performance (Base = 100)

![Normalized Stock Performance](images/Normalized_Stock_Performance.png)

Apple maintained a consistently higher indexed value for most of the period, while Samsung stayed range-bound until a sharp late-2025 surge closed much of the performance gap.

---

### 📊 Moving Averages - Trend Confirmation

<table>
<tr>
<td><img src="images/Moving_Average_for_Apple.png" alt="Apple Moving Average" width="100%"/></td>
<td><img src="images/Moving_Average_for_Samsung.png" alt="Samsung Moving Average" width="100%"/></td>
</tr>
</table>

Apple's price tracks its 6- and 12-month moving averages in a smoother, steadier uptrend. Samsung shows a similar late-cycle breakout, but with a choppier run-up.

---

### 📉 Risk vs Return

![Risk vs Return](images/Risk_vs_Return_Analysis.png)

Samsung sits in the higher-risk, higher-return quadrant (~9.5% monthly volatility, ~1.58% average return) versus Apple's lower-risk, lower-return profile (~7.1% volatility, ~1.35% return) - the clearest single chart summarizing the risk/return trade-off between the two stocks.

---

### 💹 Monthly Return Distribution

![Distribution of Monthly Returns](images/Outlier_Analysis.png)

The side-by-side boxplot highlights Samsung's wider interquartile range and several extreme positive outliers (20–34% months), versus Apple's tighter, more contained spread - visual confirmation of Samsung's higher volatility.

---

### ⚡ Rolling Volatility

<table>
<tr>
<td><img src="images/Volatility_Analysis_for_Apple.png" alt="Apple Rolling Volatility" width="100%"/></td>
<td><img src="images/Volatility_Analysis_for_Samsung.png" alt="Samsung Rolling Volatility" width="100%"/></td>
</tr>
</table>

Apple's volatility spiked in 2022 before settling into a lower, calmer band. Samsung's volatility climbs sharply into 2026, aligning with its late-period rally.

---

### 🔗 Correlation Matrix

![Correlation Matrix](images/Correlation_&_Correlation_Matrix.png)

A correlation of just **0.25** between Apple and Samsung monthly returns indicates the two stocks move largely independently - supporting the case for diversification.

---

# 📌 Key Findings

- Apple and Samsung delivered nearly identical annualized growth (Apple CAGR: 14.48%, Samsung CAGR: 14.38%) - long-term growth alone doesn't meaningfully separate the two stocks.
- The real difference between the two is risk, not return. Samsung experienced greater price volatility and larger monthly swings than Apple.
- Apple produced more consistent monthly returns and a smoother, steadier moving-average trend.
- Samsung's Maximum Drawdown (-37.54%) was substantially deeper than Apple's (-26.83%), highlighting its greater downside risk.
- Apple's Sharpe Ratio (0.19) edged out Samsung's (0.16), meaning Apple delivered a similar return per unit of risk taken - slightly more efficiently.
- A correlation of just 0.25 between Apple and Samsung monthly returns indicates the two stocks move largely independently, supporting a modest diversification benefit from holding both.
- A t-test on average monthly returns produced a p-value of 0.90 - the difference in average returns between the two stocks is not statistically significant.
- Diversification between both companies may help reduce portfolio-level risk even though their long-term growth rates are similar.

---

# 💡 Recommendations

Based on the findings:

- Apple is the more risk-efficient choice: its growth (14.48% CAGR) is essentially tied with Samsung's (14.38%), but it comes with a much shallower maximum drawdown and a higher Sharpe Ratio.
- Samsung does not show a return advantage over this period to justify its higher volatility - its added risk isn't currently being compensated by higher return.
- Lower-risk-tolerance investors should prefer Apple, since it offers comparable growth with a smaller downside.
- Investors holding or considering Samsung should size the position with its deeper drawdown risk in mind, rather than expecting a return premium to offset it.
- Given the return correlation between the two stocks is only 0.25, combining both may still offer diversification benefits.
- Investment decisions should also account for macroeconomic conditions, technological developments, company fundamentals, and the reminder that the observed average-return difference here (p = 0.90) is not statistically reliable.

---

## 📂 Repository Structure

```text
├── data/
│   ├── Apple Stock Price History.csv
│   ├── Samsung Electronics Co Stock Price History.csv
│   └── Samsung_Apple_Stock_Analysis.xlsx
├── images/
│   ├── Correlation_&_Correlation_Matrix.png
│   ├── Monthly_Return_Analysis_for_Apple.png
│   ├── Monthly_Return_Analysis_for_Samsung.png
│   ├── Moving_Average_for_Apple.png
│   ├── Moving_Average_for_Samsung.png
│   ├── Normalized_Stock_Performance.png
│   ├── Outlier_Analysis.png
│   ├── Return_Distribution_Analysis_for_Apple.png
│   ├── Return_Distribution_Analysis_for_Samsung.png
│   ├── Risk_vs_Return_Analysis.png
│   ├── Scatter_Plot_Analysis.png
│   ├── Volatility_Analysis_for_Apple.png
│   ├── Volatility_Analysis_for_Samsung.png
│   ├── Volume_Analysis_for_Apple.png
│   └── Volume_Analysis_for_Samsung.png
├── notebook/
│   └── Apple&Samsung_StockPrice_DataAnalysis.ipynb
└── README.md
```

---

# 🚀 How to Run the Project

1. Clone this repository.

```bash
git clone https://github.com/yourusername/apple-vs-samsung-stock-analysis.git
```

2. Install the required libraries.

```bash
pip install -r requirements.txt
```

3. Open the Jupyter Notebook or upload the notebook to Google Colab.

4. Run all cells sequentially.

---

# 📌 Future Improvements

Potential enhancements include:

- Daily stock price analysis
- Forecasting using ARIMA or Prophet
- Machine Learning-based stock prediction
- Interactive dashboards using Plotly
- Streamlit web application
- Integration with live financial APIs

---

# 📚 References & Data Sources

- **Historical Stock Data:** Investing.com & Yahoo Finance!

---

# 🎧 Project Soundtrack

*This track was on loop while working on this project*

[if it's real then i'll stay - bonjr](https://open.spotify.com/track/6MIouIaP6WqE6o9Uo25gdO?si=1ba1cf60b9c54ee1)

**Star this repository if you found it interesting!** ⭐

made with ❤️ by **kazim**





























#
