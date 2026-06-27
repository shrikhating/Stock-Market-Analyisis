# 📈 NSE Stock Market Terminal — Multi-Module Python Trading Intelligence Platform

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**9-Module NSE Market Intelligence Platform for Indian Equity Markets**  
_Scanner · Signals · Mutual Funds · Options Analytics · Backtesting · Institutional · Portfolio · Heatmaps_

![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Quantitative%20Finance%20%7C%20NSE-blue?style=flat-square)
![Truthfulness](https://img.shields.io/badge/AI%20Policy-Zero%20Fabrication-red?style=flat-square)

</div>

---

## 📋 Overview

The **NSE Stock Market Terminal** is a comprehensive multi-module Python/Streamlit platform for analysing Indian equity markets (NSE). It consolidates 9 distinct analytical domains — from stock scanning and technical signal generation to options analytics, institutional flow detection, portfolio optimization, and market heatmaps — into a unified dark-themed web application.

A core design principle is the **Truthfulness Contract**: every AI-derived column is prefixed with `★AI_`, raw source data is always displayed alongside for verification, and no values are randomly generated or fabricated. All indicators are computed from real market data.

---

## 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                NSE Stock Market Terminal — Module Architecture                │
└─────────────────────────────────────────────────────────────────────────────┘

  ┌──────────────────────────────────────────┐
  │         DATA ACQUISITION LAYER           │
  │  ─ NSE market data feeds                 │
  │  ─ Historical OHLCV data                 │
  │  ─ Options chain data                    │
  │  ─ FII/DII institutional flow data       │
  │  ─ Mutual fund NAV and holdings          │
  └──────────────────┬───────────────────────┘
                     │
                     ▼
  ┌──────────────────────────────────────────┐
  │         COMPUTATION ENGINE               │
  │  ─ Pandas: time-series manipulation      │
  │  ─ NumPy: statistical computations       │
  │  ─ Technical indicator library           │
  │    (45+ indicators)                      │
  └──────────────────┬───────────────────────┘
                     │
                     ▼
  ┌──────────────────────────────────────────────────────────────────────────┐
  │                         9 ANALYTICAL MODULES                              │
  │                                                                            │
  │  ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────────────────┐│
  │  │  Scanner   │ │  Signals   │ │  Mutual    │ │  Options Analytics     ││
  │  │  Module    │ │  Engine    │ │  Funds     │ │  (OI, PCR, Greeks)     ││
  │  └────────────┘ └────────────┘ └────────────┘ └────────────────────────┘│
  │  ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────────────────┐│
  │  │Backtesting │ │Institutional│ │ Portfolio  │ │  Market Heatmaps      ││
  │  │  Engine    │ │  Detection │ │ Optimizer  │ │  (Sector / Index)      ││
  │  └────────────┘ └────────────┘ └────────────┘ └────────────────────────┘│
  │                              ┌────────────┐                               │
  │                              │  AI Insights│                               │
  │                              │  (Ollama)  │                               │
  │                              └────────────┘                               │
  └──────────────────────────────────┬───────────────────────────────────────┘
                                     │
                                     ▼
  ┌──────────────────────────────────────────┐
  │    STREAMLIT MULTI-MODULE DASHBOARD       │
  │    GitHub Dark Theme · Professional UI   │
  │                                          │
  │   ★AI_ prefix enforcement on all         │
  │   AI-derived columns (Truthfulness       │
  │   Contract — zero fabrication policy)    │
  └──────────────────────────────────────────┘
```

---

## 🛠️ Technology Stack

| Component | Technology | Purpose |
|---|---|---|
| **Language** | Python | Core application logic across all modules |
| **UI Framework** | Streamlit | Multi-module web dashboard |
| **Data Layer** | Pandas | OHLCV time-series, indicator computation, portfolio math |
| **Numerics** | NumPy | Statistical computations, matrix operations |
| **Visualization** | Plotly | Interactive candlestick charts, heatmaps, indicator overlays |
| **AI Layer** | Ollama (local LLM) | AI-derived signal commentary and insights |
| **Theme** | GitHub Dark | Professional dark UI theme redesign |

---

## ✨ Module Details

### 1️⃣ Stock Scanner Module
- Multi-criteria screening across NSE-listed equities
- Filter by volume surge, price breakout, gap-up/gap-down, 52-week high/low proximity
- Results sorted by composite signal strength
- Raw screener output always shown; AI commentary in `★AI_` prefixed columns only

### 2️⃣ Technical Signal Engine
- **45+ technical indicators** computed natively:
  - Trend: SMA, EMA, DEMA, WMA, HMA, VWAP
  - Momentum: RSI, MACD, Stochastic, Williams %R, CCI, MFI
  - Volatility: Bollinger Bands, ATR, Keltner Channels, Donchian Channels
  - Volume: OBV, VWAP, Volume SMA, Accumulation/Distribution
  - Pattern: Pivot Points (Classical, Fibonacci, Camarilla)
- Multi-timeframe signal alignment
- Signal confluence scoring

### 3️⃣ Mutual Fund Analysis
- NAV tracking and performance comparison across fund categories
- Holdings overlap analysis between funds
- Sector allocation visualization
- Rolling return comparison (1M, 3M, 6M, 1Y, 3Y, 5Y)

### 4️⃣ Options Analytics
- Live options chain visualization for NSE derivatives
- Open Interest (OI) analysis — OI buildup and unwinding detection
- Put-Call Ratio (PCR) computation
- Max Pain level calculation
- Greeks display: Delta, Gamma, Theta, Vega

### 5️⃣ Backtesting Engine
- Historical strategy backtesting against NSE OHLCV data
- Configurable entry/exit rules based on technical conditions
- Performance metrics: CAGR, Sharpe Ratio, Max Drawdown, Win Rate
- Equity curve visualization with trade markers

### 6️⃣ Institutional Flow Detection
- FII (Foreign Institutional Investor) net buy/sell tracking
- DII (Domestic Institutional Investor) flow data
- Correlation of institutional flows with price movement
- Historical accumulation/distribution pattern detection

### 7️⃣ Portfolio Optimizer
- Multi-asset portfolio weight optimization
- Efficient Frontier computation (Modern Portfolio Theory)
- Sharpe Ratio maximization
- Risk contribution analysis per holding
- Correlation matrix heatmap

### 8️⃣ Market Heatmaps
- Sector-level performance heatmap (NSE sectors)
- Index constituent performance (Nifty 50, Nifty 500)
- Color-coded by % change, volume, or momentum
- Drill-down from sector → stock level

### 9️⃣ AI Insights (Ollama — Local)
- LLM-generated market commentary and signal narratives
- Strictly enforces `★AI_` prefix on all AI-derived output columns
- Raw computed values always displayed alongside AI commentary
- Offline inference — no API keys, no cloud dependency

---

## ⚖️ Truthfulness Contract

> This platform enforces a **zero-fabrication policy** on all data and AI outputs.

| Rule | Implementation |
|---|---|
| **★AI_ prefix** | Every column derived by the LLM is prefixed `★AI_` — never mixed with raw data columns |
| **Raw data always shown** | Source OHLCV and computed indicator values are always visible alongside AI commentary |
| **No random values** | Zero use of `random.random()`, `uuid`, or fabricated placeholders anywhere in the codebase |
| **Placeholder marking** | If a data source is unavailable, the column is explicitly marked `[DATA UNAVAILABLE]` — never filled with estimates |
| **No hallucinated signals** | AI commentary is grounded only in the data returned by the computation engine for that specific ticker and timeframe |

---

## 🔄 Data Flow Workflow

```
Step 1 — DATA FETCH
  └─ NSE market data pulled per module requirement
  └─ Cached with timestamp to avoid redundant API calls

Step 2 — COMPUTATION ENGINE
  └─ Pandas/NumPy compute all 45+ indicators
  └─ All values derived deterministically from raw OHLCV

Step 3 — AI ENRICHMENT (Optional)
  └─ Ollama receives computed indicator values as structured context
  └─ Generates commentary — output stored ONLY in ★AI_ prefixed columns
  └─ Raw computed values remain unchanged in source columns

Step 4 — VISUALIZATION
  └─ Streamlit renders module UI
  └─ Plotly charts: candlesticks, indicator overlays, heatmaps
  └─ Tables: raw columns + ★AI_ columns always side-by-side

Step 5 — USER INTERACTION
  └─ Parameter adjustment via Streamlit sidebar
  └─ Module navigation via top-level tabs
  └─ Download: filtered results as CSV
```

---

## 📁 Project Structure

```
nse_terminal/
├── app.py                         # Streamlit entry point + navigation
├── modules/
│   ├── scanner.py                 # Stock screening module
│   ├── signals.py                 # Technical indicator computation (45+)
│   ├── mutual_funds.py            # Mutual fund analysis
│   ├── options.py                 # Options chain + OI + Greeks
│   ├── backtesting.py             # Strategy backtesting engine
│   ├── institutional.py           # FII/DII flow detection
│   ├── portfolio.py               # Portfolio optimization (Efficient Frontier)
│   ├── heatmaps.py                # Sector/index heatmap rendering
│   └── ai_insights.py             # Ollama integration with ★AI_ enforcement
├── data/
│   ├── fetcher.py                 # Market data acquisition layer
│   └── cache.py                   # Timestamped data cache
├── theme/
│   └── dark_theme.css             # GitHub Dark theme overrides
├── config/
│   └── settings.yaml              # Module config externalized from code
└── requirements.txt
```

---

## ⚙️ Configuration (`config/settings.yaml`)

```yaml
data:
  default_period: "1y"
  default_interval: "1d"
  cache_ttl_minutes: 15

indicators:
  rsi_period: 14
  macd_fast: 12
  macd_slow: 26
  macd_signal: 9
  bollinger_period: 20
  bollinger_std: 2

portfolio:
  optimization_method: "sharpe"  # sharpe | min_variance | max_return
  risk_free_rate: 0.065           # 6.5% (Indian repo rate proxy)

ollama:
  model: "llama3.1:8b"
  endpoint: "http://localhost:11434"
  ai_column_prefix: "★AI_"       # Enforced on all LLM-derived columns
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- Ollama with model pulled (for AI Insights module)
- NSE data feed access

### Installation

```bash
git clone https://github.com/shrikhating/nse-terminal.git
cd nse-terminal
pip install -r requirements.txt
```

### Run

```bash
streamlit run app.py
```

---

## 👤 Author

**Shrikant Khating**  
Senior BI Developer | Quantitative Analyst | Python Developer  
📧 shri.khating@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/shrikant-khating) · [GitHub](https://github.com/shrikhating)

> *Built as a solo personal innovation lab project — no team, no budget, production-grade engineering.*
