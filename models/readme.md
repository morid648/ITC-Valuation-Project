# models

One master Excel file. Thirteen sheets.
All valuation, analysis, and financial modeling lives here.

---

## File
itc_master_model.xlsx

---

## Sheet Guide

| Sheet               | Purpose                                           |
|--------------------|---------------------------------------------------|
| Historical FS       | P&L, Balance Sheet, Cash Flow — FY16 to FY25     |
| Ratio Analysis      | Margins, ROCE, ROE, turnover ratios               |
| Forecast            | Revenue, EBITDA, EPS projections                  |
| WACC                | Peer beta, capital structure, cost of capital     |
| Intrinsic Growth    | ROIC, reinvestment rate, growth rate              |
| DCF                 | FCFF, terminal value, equity value per share      |
| Relative Valuation  | 10 FMCG peers — EV/Revenue, EV/EBITDA, PE        |
| SOTP                | 6 segments × segment-specific peer multiples      |
| Football Field      | All methods in one valuation range chart          |
| Altman Z-Score      | Financial distress scoring — FY16 to FY25         |
| DuPont              | ROE = margin × turnover × leverage                |
| VAR Historical      | Return distribution, VaR at 95/99/99.5%           |
| Segment Data        | Segment revenue and EBIT — FY18 to FY25           |

---

## Data Inputs

| Sheet          | Reads From                      |
|---------------|----------------------------------|
| VAR Historical | itc_daily_prices_1996_2026.csv  |
| WACC           | peer_beta_fundamentals.csv      |
| WACC           | peer_tax_rates.csv              |
| SOTP           | segment_peer_ev_ebit.csv        |

---

## Note

Do not rename any sheet.
Cross-sheet formulas depend on exact sheet names.
