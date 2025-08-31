# 🌋 LAVA – Liquidity in Africa (Nigeria Stablecoin Case Study)

This repo supports my **Technical Research Analyst** application for **LAVA**, investigating where African payment orchestration companies source liquidity and how efficiently it’s used. A **Nigeria stablecoin adoption** case study grounds the analysis in data, focusing on platforms like Flutterwave and Binance P2P.

## Methodology (Summary)
1. **Map Liquidity Sources**: Trace flows from banks (e.g., Zenith Bank FX lines), mobile money (MTN MoMo), stablecoins (USDT via Binance P2P), remittances (WorldRemit, hawala), and central bank FX auctions (CBN).  
2. **Collect Data**: Onchain (Dune Analytics for USDT/Celo transfers), offchain (World Bank remittances, Google Trends for “crypto”/“dollar rate”), and primary insights (X posts from P2P traders).  
3. **Measure Efficiency**: Analyze cost (e.g., 2–5% P2P fees), speed (crypto vs. T+2 bank transfers), and recycling (USDT-to-Naira reconversion losses).  
4. **Analyze & Visualize**: Time-series (stablecoin surges), correlations (FX volatility), and network maps (wallet flows).  
5. **Deliver**: Dashboard (USDT flow trends), efficiency scorecard (by market/channel), and narrative report (bottlenecks, opportunities).

See `notebooks/liquidity_nigeria_stablecoins.ipynb` for the analysis. Sample output: `outputs/usdt_naira_flows.png` (network map of Binance P2P trades).

## 📂 Repo Structure
- `notebooks/liquidity_nigeria_stablecoins.ipynb`: Main analysis notebook.
- `scripts/`: Data scraping (e.g., Binance P2P API).
- `outputs/`: Visualizations (e.g., flow maps, efficiency charts).
- `requirements.txt`: Dependencies.

## 🚀 Quickstart
```bash
# Use a virtual environment
python -m venv .venv && source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# Set Dune API key (optional for onchain data)
export DUNE_API_KEY="YOUR_KEY"  # Windows: set DUNE_API_KEY=YOUR_KEY

# Run notebook
jupyter lab
```

## 📦 Data Sources
- **World Bank**: Remittances received (`BX.TRF.PWKR.CD.DT`) for Nigeria via API.  
- **Google Trends**: Interest for “USDT,” “Binance,” “P2P” in Nigeria (`pytrends`).  
- **Dune Analytics**: USDT transfers on Ethereum and Celo, filtered for Nigeria via exchange APIs (e.g., Binance P2P).  
- **CBN Reports**: FX auction volumes and parallel market spreads.

## 🧰 Requirements
See `requirements.txt`.

## 📜 License
MIT License – open for collaboration and review.
![Visitors](https://visitor-badge.glitch.me/badge?page_id=FijabiAdekunle.Investigating-Liquidity-in-Africa)


## 🧑‍💻 Author
 **Fijabi J. Adekunle** – Marine engineer turned data scientist
> Navigating Data | Unveiling Insight | Driving Impact
