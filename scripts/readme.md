# scripts/

Python data pipeline for the ITC valuation project.
Each script does one job — fetch, search, or calculate.
No valuation logic lives here. Only data collection.

---

## Run Order

```bash
# Step 1 — ITC price history (used for VaR)
python fetch_itc_prices.py

# Step 2 — Peer data (used for WACC)
python fetch_peer_beta_data.py
python fetch_peer_tax_rates.py

# Step 3 — Segment peers (used for SOTP)
# Must run in this exact order
python segment_peers_list.py
python fetch_segment_tickers.py
python fetch_segment_raw.py
python calc_ev_ebit_final.py
```

---

## Script Map

| Script                    | Input                          | Output                         |
|--------------------------|--------------------------------|--------------------------------|
| fetch_itc_prices.py       | —                              | itc_daily_prices_1996_2026.csv |
| fetch_peer_beta_data.py   | —                              | peer_beta_fundamentals.csv     |
| fetch_peer_tax_rates.py   | —                              | peer_tax_rates.csv             |
| segment_peers_list.py     | —                              | segment_peers_list.csv         |
| fetch_segment_tickers.py  | segment_peers_list.csv         | segment_peers_with_tickers.csv |
| fetch_segment_raw.py      | segment_peers_with_tickers.csv | segment_raw.csv                |
| calc_ev_ebit_final.py     | segment_raw.csv                | segment_peer_ev_ebit.csv       |

---

## Requirements

```bash
pip install yfinance pandas
```
