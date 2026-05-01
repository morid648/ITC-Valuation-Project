# 📊 ITC Limited — Equity Valuation & Financial Analysis
### Identifying Mispricing in One of India's Most Debated Large-Cap Stocks

---

## 🧠 Executive Summary

ITC trades at a 60%+ discount to FMCG peers despite zero net debt,
35%+ margins, and consistent cash flows across a decade.

We observe a double discount — tobacco ESG penalty +
conglomerate complexity — both of which are structurally unwinding.

**Key Risk:** Cigarettes carry the overwhelming majority of EBIT.
Any regulatory shock hits consolidated earnings disproportionately.

**Conclusion:** Modestly undervalued at CMP. Clear re-rating path
via hotel demerger (done) and FMCG margin expansion (in progress).

---

## 🏢 Business Context

Six segments — Cigarettes, FMCG, Hotels, Agri, Paperboards, Infotech.
Cigarettes dominate profit. FMCG Others is inflecting toward profitability.
Hotel demerger in FY25 removed a structural margin drag.

---

## 📊 KPI Snapshot

| Metric                  | Value                               |
|------------------------|-------------------------------------|
| Revenue (FY25)          | ₹75,323 Cr — 10.9% YoY             |
| EBITDA Margin (10Y Avg) | 36.5% — stable across cycles        |
| ROIC (FY25)             | 56.5% vs WACC 12.4%                 |
| Net Debt                | Nil — Interest Coverage 537x        |
| Dividend Payout         | 100%+ consistently                  |

---

## 📈 Core Insights

- **Revenue growth** is cigarette-led — diversification is
  revenue-level, not yet profit-level
- **Margins** held 34–39% through COVID and inflation —
  pricing power is real
- **FMCG Others** margin: 1.5% (FY18) → 8.5% (FY24) —
  the key inflection to watch
- **ROIC >> WACC** for 5 consecutive years —
  value creation is consistent, not cyclical

---

## 🧾 Valuation Summary

| Method                   | Implied Value (₹/share) |
|-------------------------|--------------------------|
| DCF — Bear / Base / Bull | 137 — 177 — 340          |
| SOTP                     | ~375                     |
| Peer Comps               | ~769 – 793               |
| **CMP (at analysis)**    | **~308**                 |

SOTP at ₹375 is the most grounded method.
DCF gap vs SOTP traces to one assumption — reinvestment rate.
Peer comps overstate value due to tobacco-free multiples.

![Football Field](outputs/01_football_field_valuation_summary_itc.png)

---

## ⚠️ Key Risks

- Cigarette EBIT concentration — revenue diversification masks it
- 67% of DCF value in terminal value — sensitive to growth assumptions
- Reinvestment ramp assumed in DCF has no historical support

---

## 💡 Strategic View

**Stance: Accumulate on dips. Hold at current levels.**
Quality business. Fair price. Re-rating already underway.
Entry below ₹290 — Exit above ₹420.

---

## 🛠️ Tools & Skills

| Tool         | Application                                       |
|-------------|---------------------------------------------------|
| Python       | Data pipeline — prices, peer betas, segment comps |
| yfinance     | 30 years of market data fetched programmatically  |
| pandas       | Data cleaning, processing, CSV management         |
| Excel        | Full financial model — 13 integrated sheets       |
| Screener.in  | Fundamental data cross-validation                 |

`DCF` `SOTP` `Relative Valuation` `Football Field`
`WACC` `DuPont` `Altman Z-Score` `Historical VaR`
`ROIC` `Segment Margin Decomposition`

---

## 📂 Project Structure
ITC-Valuation-Project/
│
├── data/
│ ├── raw/ ← Python fetch outputs
│ └── processed/ ← Calculated model inputs
│
├── scripts/ ← 7 Python data fetch scripts
│
├── models/
│ └── itc_master_model.xlsx
│
├── outputs/ ← 10 charts + visuals
│
└── README.md

---

## 🔁 How to Reproduce

```bash
pip install yfinance pandas

python scripts/fetch_itc_prices.py
python scripts/fetch_peer_beta_data.py
python scripts/fetch_peer_tax_rates.py
python scripts/segment_peers_list.py
python scripts/fetch_segment_tickers.py
python scripts/fetch_segment_raw.py
python scripts/calc_ev_ebit_final.py
```

Then open `models/itc_master_model.xlsx`

---

## 🎯 Key Takeaways

- 60% peer discount on a zero-debt, 35%+ margin business
  is structural — and structurally unwinding
- ROIC of 56% vs WACC of 12% is among the widest
  value-creation spreads in Indian large-cap equities
- The DCF vs SOTP gap traces to one assumption —
  that single variable drives a ₹198/share difference
- Re-rating catalyst already in motion —
  demerger done, FMCG margins inflecting

---

## 🤝 Open To

Financial Analyst • Equity Research • Data Analytics roles

---

*Data: Yahoo Finance + ITC Annual Reports FY16–FY25.*
*Figures in INR Crores. Not investment advice.*

---
### Author:Anshul Chaudhary | morid648@gmail.com
