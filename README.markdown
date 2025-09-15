# 🌍 Liquidity in Africa: Nigeria Stablecoin Case Study

*This repo investigates where African payment orchestration companies source liquidity and how efficiently it’s used, using Nigeria’s stablecoin adoption as a case study.*

The research draws on both `onchain` and `offchain` data, with a focus on how platforms like Binance P2P, Flutterwave, and mobile money providers contribute to liquidity flows in Nigeria.

### 🔎 Methodology (Summary)

**Map Liquidity Sources**
- Banks (e.g., Zenith FX lines), mobile money (MTN MoMo), stablecoins (USDT via Binance P2P), remittances (WorldRemit, hawala), and CBN FX auctions.

**Collect Data**

`Onchain`: USDT transfers on Ethereum/Celo (Dune Analytics).

`Offchain`: World Bank remittances, CBN FX reports, Google Trends for “USDT/crypto/dollar rate.”

**Primary Insights**: P2P trader posts on X/Twitter.

- Measure Efficiency:
Compare cost (2–5% P2P spreads vs 8–9% bank FX), speed (crypto instant vs T+2 bank), and recycling (losses from USDT-to-Naira reconversions).

- Analyze & Visualize

- Time-series: stablecoin surges.

- Correlations: USDT demand vs FX volatility.

- Network maps: wallet flows across P2P.

**Deliverables**

- Dashboard: USDT trend flows.

- Efficiency scorecard: By liquidity channel.

- Narrative report: Bottlenecks & opportunities.

- 👉 See notebooks/liquidity_nigeria_stablecoins.ipynb
 for the full analysis.
- 👉 Sample output: outputs/usdt_naira_flows.png (Binance P2P network map).

### 📂 Repo Structure

- notebooks/liquidity_nigeria_stablecoins.ipynb → Main analysis notebook.

- scripts/ → Scraping utilities (Binance P2P API).

- outputs/ → Charts & visualizations (flow maps, scorecards).

- requirements.txt → Dependencies list.

### 🚀 Quickstart
### Create virtual environment
python -m venv .venv && source .venv/bin/activate  
#### Windows: .venv\Scripts\activate  

#### Install requirements
pip install -r requirements.txt  

#### (Optional) Set Dune API key for onchain queries
export DUNE_API_KEY="YOUR_KEY"  
#### Windows: set DUNE_API_KEY=YOUR_KEY  

#### Launch Jupyter
jupyter lab  

### 📦 Data Sources

- World Bank: Remittances API (BX.TRF.PWKR.CD.DT).

- Google Trends: “USDT,” “Binance,” “P2P” via pytrends.

- Dune Analytics: USDT flows (Ethereum + Celo).

- CBN Reports: FX auctions & parallel market spreads.

- Binance P2P API: Real spreads and liquidity depth.

### 🧰 Requirements

> See requirements.txt
.

### 📜 License

*MIT License — open for collaboration, feedback, and community contributions.*

### 👤 Author

Fijabi J. Adekunle
> Marine engineer ⚓ turned data scientist 📊, exploring how liquidity flows shape Africa’s fintech and Web3 future.

*✨ Note: This project began as part of a VC research task but is now released publicly to contribute to the growing conversation on open financial infrastructure in Africa.*