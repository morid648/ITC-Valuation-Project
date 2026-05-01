# data

All financial datasets used in this project.
Every file is either fetched by a Python script
or calculated from fetched data.
Nothing here is manually entered.

---

## Structure
data/
├── raw/ ← Direct output of scripts/ — never edit manually
└── processed/ ← Calculated outputs ready for the Excel model

---

## File Map

| File                             | Source                    | Used In                  |
|---------------------------------|---------------------------|--------------------------|
| itc_daily_prices_1996_2026.csv  | fetch_itc_prices.py       | VAR Historical           |
| peer_beta_fundamentals.csv      | fetch_peer_beta_data.py   | WACC                     |
| peer_tax_rates.csv              | fetch_peer_tax_rates.py   | WACC                     |
| segment_peers_list.csv          | segment_peers_list.py     | fetch_segment_tickers.py |
| segment_peers_with_tickers.csv  | fetch_segment_tickers.py  | fetch_segment_raw.py     |
| segment_raw.csv                 | fetch_segment_raw.py      | calc_ev_ebit_final.py    |
| segment_peer_ev_ebit.csv        | calc_ev_ebit_final.py     | SOTP Sheet               |

---

## Rule

- Never edit anything in `raw/` manually
- `processed/` holds calculated outputs — not fetched data
- Rerun the relevant script if any file needs refreshing
