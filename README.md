# Intesa Sanpaolo (ISP.MI) — Equity Research Report

> **Full sell-side style equity research on one of Europe's largest banks, built entirely in Python.**

---

## Rating & Price Target

| | |
|---|---|
| **Recommendation** | **HOLD** |
| **Price Target (Base)** | EUR 4.99 |
| **Current Price** | EUR 4.52 (May 2026) |
| **Upside** | +10.4% |
| **Dividend Yield (fwd)** | ~8.9% |
| **Total Return (12M)** | ~19.3% |
| **Price Target (Bull)** | EUR 6.64 |
| **Price Target (Bear)** | EUR 3.81 |

---

## Project Overview

This repository contains a complete, professional-grade equity research project on **Intesa Sanpaolo S.p.A. (ISP.MI)**, Italy's largest bank and one of the top-10 European banks by market cap (~EUR 78.5 billion).

The analysis was built from scratch using Python, following the methodology of a professional sell-side equity research report:

1. **Data extraction** via `yfinance` API (financials, balance sheet, cash flow)
2. **KPI analysis** — NIM, ROTE, CIR, NPL ratio, CET1 (2022–2025)
3. **Forward model** — Base / Bull / Bear scenarios for 2026–2028
4. **6-method valuation** — DDM, P/BV, P/E, Excess Return, SOTP, Peer Comps
5. **Football field chart** — visualising the valuation range
6. **Peer benchmarking** — vs. UCG.MI, BNP.PA, SAN.MC, INGA.AS, GLE.PA
7. **Risk register** — 11 risks with probability, impact, severity, mitigation
8. **Investment thesis** — written thesis, rating, price target, catalysts

---

## Repository Structure

```
intesa_sanpalolo/
│
├── Intesa_sanpaolo.ipynb          # Main analysis notebook (10 cells)
├── ISP_Analysis.xlsx              # Full Excel model (7 sheets)
├── intesa_sanpaolo_analisi.docx   # Italian Word report (9 sections + Sintesi)
│
├── chart/
│   ├── ISP_forward_model.png              # Scenario projections chart
│   ├── ISP_valuation_football_field.png   # Valuation football field
│   ├── linkedin_chart1_revenue_growth.png
│   ├── linkedin_chart2_kpi_evolution.png
│   ├── linkedin_chart3_scenario_projections.png
│   ├── linkedin_chart4_peer_comparison.png
│   └── linkedin_chart5_football_field.png
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Notebook Cell Structure

| Cell | Content |
|------|---------|
| 0 | Data extraction via yfinance — ISP.MI financials 2022–2025 |
| 1 | KPI Dashboard — NIM, ROTE, CIR, NPL, CET1 |
| 2 | Excel export — Income Statement, Balance Sheet, Cash Flow, KPIs |
| 3 | Forward Model — Base/Bull/Bear 2026–2028 |
| 4 | Export Forward Model to Excel |
| 5 | Valuation — 6 methods + Football Field chart |
| 6 | Export Valuation to Excel |
| 7 | Risk Register — 11 risks + Excel export |
| 8 | Investment Thesis — HOLD rating, PT EUR 4.99 + Excel export |
| 9 | LinkedIn Charts — 5 dark-theme charts for social media |

---

## Excel Model — 7 Sheets

1. **Income Statement** — P&L 2022–2025 with all line items
2. **Balance Sheet** — Assets, liabilities, equity 2022–2025
3. **KPI Dashboard** — NIM, ROTE, CIR, NPL, CET1, EPS, DPS
4. **Forward Model** — Base/Bull/Bear 2026–2028 projections
5. **Valuation** — 6-method valuation with price targets and assumptions
6. **Risk Register** — 11 risks with severity colour-coding
7. **Investment Thesis** — Summary table of rating, PT, catalysts, risks

---

## Key Financial Metrics (2025A)

| Metric | Value |
|--------|-------|
| Net Income | EUR 9.19 billion (+11% YoY) |
| NIM | 1.80% |
| ROTE | 16.9% (vs. Ke 10.1%) |
| CIR | 40.0% (best-in-class EU) |
| CET1 Ratio | ~13.5% |
| NPL Ratio (net) | 0.9% |
| EPS | EUR 0.529 |
| DPS | EUR 0.404 |

---

## Valuation Summary

| Method | Bear | Base | Bull | Weight |
|--------|------|------|------|--------|
| DDM | EUR 3.75 | EUR 4.80 | EUR 6.30 | 25% |
| P/BV | EUR 3.85 | EUR 4.72 | EUR 5.80 | 20% |
| P/E | EUR 3.65 | EUR 4.90 | EUR 6.75 | 20% |
| Excess Return | EUR 4.05 | EUR 5.25 | EUR 6.85 | 20% |
| SOTP | EUR 3.70 | EUR 5.10 | EUR 6.55 | 10% |
| Peer Comps | EUR 3.80 | EUR 5.20 | EUR 6.75 | 5% |
| **Weighted Avg** | **EUR 3.81** | **EUR 4.99** | **EUR 6.64** | 100% |

---

## Setup

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/intesa-sanpaolo-equity-research.git
cd intesa-sanpaolo-equity-research

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook Intesa_sanpaolo.ipynb
```

> **Note:** Cell 0 requires a live internet connection to fetch data from Yahoo Finance (`yfinance`). All subsequent cells can run with the fetched data in memory.

---

## Methodology Notes

- **NIM** = Net Interest Income / Average Total Assets
- **ROTE** = Net Income / Tangible Book Value
- **CIR** = Operating Expenses / Total Revenue
- **CAPM**: Ke = rf (3.8%) + β (1.15) × ERP (5.5%) = **10.1%**
- **DDM**: P = DPS / (Ke − g), g = 2.5%
- **Tax Rate**: 27% (IRES 24% + IRAP ~3%)
- **Payout Ratio**: 70% (ISP Piano d'Impresa target)

---

## Disclaimer

> This report is for **educational and personal research purposes only**. It does not constitute financial advice or a solicitation to invest. The author does not hold positions in ISP.MI. Past performance is not indicative of future results. Always conduct your own due diligence before making investment decisions.

---

## Author

**Ali Akbar** | [ali123akbar12@gmail.com](mailto:ali123akbar12@gmail.com)

*Equity Research Project — May 2026*
