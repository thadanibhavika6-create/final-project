# final-project
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:36BCF7,50:8E2DE2,100:f857a6&height=200&section=header&text=Stock%20Market%20Analyzer&fontSize=48&fontColor=ffffff&fontAlignY=32&desc=Simulate%20%7C%20Analyze%20%7C%20Visualize&descAlignY=52&descSize=20&animation=twinkling&fontFamily=Poppins" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=8E2DE2&center=true&vCenter=true&width=600&lines=Built+with+Python+%F0%9F%90%8D;Powered+by+Pandas+%2B+NumPy;Charts+by+Matplotlib+%2B+Seaborn" alt="Typing SVG" />

<br/>

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4C72B0?style=for-the-badge)

![GitHub repo size](https://img.shields.io/github/repo-size/your-username/stock-market-analyzer?style=flat-square&color=orange)
![GitHub last commit](https://img.shields.io/github/last-commit/your-username/stock-market-analyzer?style=flat-square&color=green)
![GitHub issues](https://img.shields.io/github/issues/your-username/stock-market-analyzer?style=flat-square&color=red)
![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)
![Stars](https://img.shields.io/github/stars/your-username/stock-market-analyzer?style=flat-square&color=blueviolet)
![Forks](https://img.shields.io/github/forks/your-username/stock-market-analyzer?style=flat-square&color=blue)
![Maintained](https://img.shields.io/badge/Maintained%3F-yes-brightgreen.svg?style=flat-square)

</div>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#️-tech-stack)
- [Project Structure](#️-project-structure)
- [Installation](#️-installation)
- [Usage](#-usage)
- [How It Works](#-how-it-works)
- [Indicators Calculated](#-indicators-calculated)
- [Output Preview](#-output-preview)
- [Roadmap](#️-roadmap)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:36BCF7,100:8E2DE2&height=120&section=header&text=About%20The%20Project&fontSize=34&fontColor=ffffff&fontAlignY=35&desc=Know%20what%20this%20project%20is%20all%20about&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 📖 About The Project

**Stock Market Analyzer** is a Python-based data analysis project that generates a realistic simulated OHLCV (Open, High, Low, Close, Volume) dataset for a stock — by default **RELIANCE.NS** — and runs it through a complete technical analysis and visualization pipeline.

Using **NumPy** for random-walk price simulation and statistics, **Pandas** for time-series manipulation, and **Matplotlib** + **Seaborn** for charting, the project computes moving averages, volatility, and return distributions, then visualizes them through clean, publication-ready plots.

It's built as a hands-on demonstration of core quantitative finance and data analysis concepts — a great reference for anyone learning how `pandas`, `numpy`, `matplotlib`, and `seaborn` come together in a real time-series workflow.

> 💡 No API keys, no external data downloads required — the dataset is simulated locally using a reproducible random seed, so results are consistent every run.

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:150458,100:6A11CB&height=120&section=header&text=Features&fontSize=34&fontColor=ffffff&fontAlignY=35&desc=Everything%20this%20tool%20can%20do%20for%20you&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## ✨ Features

| Feature | Description |
|---|---|
| 🎲 **Simulated OHLCV Data** | Generates realistic Open, High, Low, Close, and Volume data using a NumPy random-walk model with a fixed seed for reproducibility |
| 📅 **Custom Date Range** | Configurable ticker, start date, and end date for the simulated business-day time series |
| 📈 **Moving Averages** | 20-day & 50-day Simple Moving Averages (SMA) and a 20-day Exponential Moving Average (EMA) |
| 📉 **Daily Returns** | Percentage daily returns computed from closing prices |
| 🌪️ **Rolling Volatility** | 20-day rolling standard deviation of daily returns |
| 📊 **Annualized Volatility** | Full-period volatility annualized using the √252 trading-day scaling factor |
| 🖼️ **Price Chart** | Closing price plotted alongside SMA-20 and SMA-50 trend lines |
| 📊 **Volume Chart** | Bar chart of trading volume over the full date range |
| 🔔 **Returns Distribution** | Histogram + KDE of daily returns to visualize the return profile |
| 🔥 **Correlation Heatmap** | Seaborn heatmap showing correlation between Close, Volume, Returns, SMAs, and Volatility |

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:013243,100:2193b0&height=120&section=header&text=Tech%20Stack&fontSize=34&fontColor=ffffff&fontAlignY=35&desc=Built%20with%20these%20powerful%20tools&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 🖥️ Tech Stack

<div align="center">

| Library | Purpose |
|---|---|
| ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) | Core programming language |
| ![Pandas](https://img.shields.io/badge/-Pandas-150458?style=flat-square&logo=pandas&logoColor=white) | Time-series indexing, rolling windows, indicator calculations |
| ![NumPy](https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white) | Random-walk price simulation and statistical calculations |
| ![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?style=flat-square) | Price, volume, and distribution plots |
| ![Seaborn](https://img.shields.io/badge/-Seaborn-4C72B0?style=flat-square) | Styled histograms and the correlation heatmap |

</div>

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:11557C,100:38ef7d&height=120&section=header&text=Project%20Structure&fontSize=32&fontColor=ffffff&fontAlignY=35&desc=How%20the%20codebase%20is%20organized&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 🗂️ Project Structure

```
stock-market-analyzer/
│
├── stock_analyzer.py       # Main script — data simulation, indicators & plots
├── assets/                 # Saved chart screenshots
├── requirements.txt        # Python dependencies
└── README.md                # You are here
```

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:4C72B0,100:00c6ff&height=120&section=header&text=Installation&fontSize=34&fontColor=ffffff&fontAlignY=35&desc=Get%20up%20and%20running%20in%20minutes&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## ⚙️ Installation

**1. Clone the repository**

```bash
git clone https://github.com/your-username/stock-market-analyzer.git
cd stock-market-analyzer
```

**2. (Optional but recommended) Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```

**3. Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn
```

Or, if a `requirements.txt` is present:

```bash
pip install -r requirements.txt
```

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:36BCF7,100:f857a6&height=120&section=header&text=Usage&fontSize=36&fontColor=ffffff&fontAlignY=35&desc=A%20step-by-step%20walkthrough&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 🚀 Usage

Run the script (or notebook cells) in order:

```bash
python stock_analyzer.py
```

The pipeline runs through these stages automatically:

1. 🎲 **Data simulation** — a reproducible OHLCV dataset is generated for `TICKER` between `START_DATE` and `END_DATE`
2. 🧮 **Indicator calculations** — SMA-20, SMA-50, EMA-20, daily returns, 20-day rolling volatility, and annualized volatility are computed and printed
3. 📈 **Price chart** — Close price plotted with SMA-20 and SMA-50 overlays
4. 📊 **Volume chart** — trading volume bar chart across the full period
5. 🔔 **Returns distribution** — histogram + KDE of daily returns
6. 🔥 **Correlation heatmap** — relationships between price, volume, returns, and volatility

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:150458,100:ff512f&height=120&section=header&text=How%20It%20Works&fontSize=32&fontColor=ffffff&fontAlignY=35&desc=A%20peek%20under%20the%20hood&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 🧠 How It Works

The script flows through a straightforward simulate → calculate → visualize pipeline:

```python
# 1. Simulate OHLCV data with a NumPy random walk
df = simulate_ohlcv(TICKER, START_DATE, END_DATE, seed=42)

# 2. Calculate technical indicators
df["SMA_20"] = df["Close"].rolling(20).mean()
df["SMA_50"] = df["Close"].rolling(50).mean()
df["EMA_20"] = df["Close"].ewm(span=20, adjust=False).mean()
df["Daily_Return"] = df["Close"].pct_change() * 100
df["Volatility_20"] = df["Daily_Return"].rolling(20).std()

# 3. Visualize
plot_price_with_moving_averages(df)
plot_volume(df)
plot_returns_distribution(df)
plot_correlation_heatmap(df)
```

Each stage is independent, so indicators or charts can be swapped out or extended without touching the rest of the pipeline.

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:013243,100:00b09b&height=120&section=header&text=Indicators%20Calculated&fontSize=30&fontColor=ffffff&fontAlignY=35&desc=What%20the%20numbers%20mean&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 📁 Indicators Calculated

| Indicator | Formula / Method | Purpose |
|---|---|---|
| **SMA (20 / 50)** | Rolling mean of `Close` over N days | Identify short & medium-term trend direction |
| **EMA (20)** | Exponentially weighted mean of `Close` | Trend line that reacts faster to recent prices |
| **Daily Return (%)** | `Close.pct_change() * 100` | Day-over-day percentage price change |
| **Volatility (20-day)** | Rolling std. dev. of daily returns | Short-term measure of price fluctuation |
| **Annualized Volatility** | `std(returns) * sqrt(252)` | Full-period volatility scaled to a trading year |

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:11557C,100:a18cd1&height=120&section=header&text=Output%20Preview&fontSize=32&fontColor=ffffff&fontAlignY=35&desc=A%20glimpse%20of%20the%20generated%20charts&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 📸 Output Preview

<div align="center">

| Price Chart | Volume Chart | Heatmap |
|---|---|---|
| 📈 Close + SMA-20 + SMA-50 | 📊 Trading Volume Over Time | 🔥 Correlation Matrix |

</div>

> Add your own generated chart screenshots inside an `assets/` folder, then reference them like:
> `![Price Chart](assets/price_chart.png)`

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:4C72B0,100:f7971e&height=120&section=header&text=Roadmap&fontSize=36&fontColor=ffffff&fontAlignY=35&desc=What%27s%20coming%20up%20next&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 🗺️ Roadmap

- [ ] Fetch real historical data via `yfinance` as an alternative to simulation
- [ ] Add RSI and MACD indicators
- [ ] Export summary statistics and charts as a PDF report
- [ ] Add a simple web dashboard (Streamlit)
- [ ] Add unit tests for indicator calculations
- [ ] Support multiple tickers in a single run

Feel free to open an issue if you'd like to suggest a feature!

---

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:36BCF7,100:11998e&height=120&section=header&text=Contributing&fontSize=34&fontColor=ffffff&fontAlignY=35&desc=Help%20make%20this%20project%20even%20better&descAlignY=58&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn and grow. Any contributions you make are **greatly appreciated**.

1. Fork the project
2. Create your feature branch  
   `git checkout -b feature/AmazingFeature`
3. Commit your changes  
   `git commit -m 'Add some AmazingFeature'`
4. Push to the branch  
   `git push origin feature/AmazingFeature`
5. Open a Pull Request

---

## 📜 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

# 👩‍💻 Author
Bhavika Thadani
📍 Ahmedabad

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

<img src="https://raw.githubusercontent.com/platane/platane/output/github-contribution-grid-snake.svg" width="100%" alt="snake animation"/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:36BCF7,100:8E2DE2&height=180&section=footer&text=Thanks%20For%20Visiting!&fontSize=32&fontColor=ffffff&fontAlignY=70&desc=Star%20the%20repo%20if%20you%20liked%20it%20%E2%AD%90&descAlignY=85&descSize=16&animation=twinkling&fontFamily=Poppins" width="100%"/>

Made with ❤️ using Python

</div>
