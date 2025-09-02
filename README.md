# Saving Dollars with Diversion💵

**A financial story of campus waste streams.**  
Interactive dashboard that translates diversion (recycling, compost, reuse) into concrete dollar savings — front-loaded KPIs, monthly & cumulative charts, and an exploratory toolkit for understanding: *How much did diversion save us, and where can we do better?*

**Live demo:** https://suhaas15.github.io/SavingDollarsWithDiversion/

---

## Table of contents
- [Quick summary](#quick-summary)
- [Live demo](#live-demo)
- [Tech stack](#tech-stack)
- [Run locally](#run-locally)
- [Project structure](#project-structure)
- [Data format / schema](#data-format--schema)
- [How to present / demo](#how-to-present--demo)
- [Placeholders for screenshots](#placeholders-for-screenshots)
- [Potential extensions](#potential-extensions)
- [License](#license)
- [Contact](#contact)

---

## Quick summary
This dashboard converts campus waste diversion into dollar metrics you can act on:
- **Total savings** vs a hypothetical all-landfill baseline
- **Monthly and cumulative savings** to reveal trends and long-term impact
- **Stream-level cost breakdowns** (Landfill / Recycling / Compost / Reuse)

The UI follows a data-story flow: **Snapshot → Detail → Outcome** so decision-makers see the headline numbers first, then drill into the drivers.

---

## Live demo
Explore the interactive dashboard here:

https://suhaas15.github.io/SavingDollarsWithDiversion/

Use the date slider and legend toggles to focus on particular months or waste streams.

---

## Tech stack
- Static site (HTML / CSS / JS)
- Client-side charts (D3, Plotly, or similar)
- Hosted with GitHub Pages

If your repo uses any build tools (npm, webpack, parcel), add a `package.json` and build instructions.

---

## Run locally
1. Clone the repo
```bash
git clone https://github.com/suhaas15/SavingDollarsWithDiversion.git
cd SavingDollarsWithDiversion
```

2. Serve locally (Python 3):
```bash
python -m http.server 8000
# open http://localhost:8000
```

Or use VS Code Live Server or `npx serve` / `http-server`.

---

## Project structure (example)
```
/SavingDollarsWithDiversion
├─ index.html
├─ css/
│  └─ styles.css
├─ js/
│  └─ main.js
├─ data/
│  └─ waste_costs.csv
├─ assets/
│  └─ screenshot-1.png
└─ README.md
```

Adjust names if your repo differs — these are suggested conventions for clarity.

---

## Data format / schema
Typical CSV/JSON columns expected by the dashboard:
- `date` — ISO date (YYYY-MM-DD)
- `stream` — Landfill | Recycling | Compost | Reuse
- `cost` — numeric (dollars)
- `quantity` — optional (lbs or kg)

Example CSV header:
```
date,stream,cost,quantity
2024-01-15,Recycling,12.34,150
```

If your `main.js` references a different filename or field names, update the schema or rename your data file accordingly.

---

## How to present / demo
1. **Open with the KPI panel** — call out Total Savings vs Hypothetical Cost.
2. **Show monthly time series** — highlight seasonality or spikes (move-outs, events).
3. **Toggle streams in the stacked breakdown** — demonstrate which streams drive costs.
4. **Finish with cumulative net benefit** — emphasize long-term ROI.

A short 30–60s elevator pitch: _“This dashboard turns diversion into dollars. It shows how recycling and composting reduce our campus waste bill over time and where additional diversion would deliver the most savings.”_

---

## Potential extensions
- Per-building drilldowns and filters
- Cost-per-weight (cost per lb/kg) metrics
- Scenario simulator (e.g., what-if: increase recycling rate by X%)
- Automated ETL to refresh data periodically

---


## Contact
Suhaas — https://github.com/suhaas15

