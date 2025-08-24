# 🌋 LAVA – Liquidity in Africa (Nigeria Stablecoin Case Study)

This repo supports my task submission for the **Technical Research Analyst** role at **LAVA**.
It pairs **onchain** and **offchain** data to investigate:
- **Where** African payment orchestration companies source liquidity
- **How efficiently** this liquidity is used

A focused **Nigeria stablecoin adoption** case study is included to ground the methodology in concrete data.

## 🧭 Methodology (summary)
1. **Map liquidity sources** (banks, mobile money, stablecoins, remittances, FX auctions).
2. **Collect data** from onchain (Dune) and offchain (World Bank, Google Trends, central bank reports).
3. **Measure efficiency** along cost, speed, and recycling of capital.
4. **Analyze & visualize** time series, correlations, and network flows.
5. **Deliver** a dashboard, efficiency scorecard, and written insights.

See `notebooks/liquidity_nigeria_stablecoins.ipynb` to run the analysis.

## 🚀 Quickstart
```bash
# (Recommended) use a virtual environment
python -m venv .venv && source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# set your Dune API key (optional, only if you want onchain pulls)
export DUNE_API_KEY="YOUR_KEY"   # Windows: set DUNE_API_KEY=YOUR_KEY

# run the notebook
jupyter lab  # or jupyter notebook
```

## 📦 Data Sources (quick-start)
- **World Bank Remittances**: Personal remittances received (indicator `BX.TRF.PWKR.CD.DT`) for `NGA` via the World Bank API.
- **Google Trends (Nigeria)**: Interest-over-time for queries like `"USDT"`, `"crypto"`, `"binance"`, `"p2p"`, `"dollar rate"` using `pytrends`.
- **Dune Analytics (optional)**: Stablecoin transfers (e.g., USDT contract `0xdAC17F958D2ee523a2206206994597C13D831ec7`) aggregated by day; join with offchain proxies to contextualize Nigeria.

## 🧰 Requirements
See `requirements.txt`.

## 🧑‍💻 Author
Fijabi J. Adekunle — *Marine engineering background turned data scientist.*
