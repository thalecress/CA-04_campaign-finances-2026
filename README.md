# CA-04 Campaign Finance & Network Dashboard

An interactive campaign finance visualization and network analysis tool for the California 4th Congressional District (CA-04) election between Eric Jones and Mike Thompson.

## 📌 Features

- **Interactive Network Graph:** Explore relationships between candidates, donor sectors, PACs, and individual contributors using D3.js force-directed topology.
- **Granular Drill-Down:** Filter network flows by candidate, donor sector, entity type, or transaction size.
- **Itemized Ledger:** Search and inspect individual filings with CSV export capabilities.
- **Metric Toggles:** Switch between dollar amounts ($) and percentage breakdown (%) views.

---

## 📊 Campaign Summary

- **Eric Jones (Total: ~$18.40M):** Primarily self-funded through personal loans (~82.4% / $15.16M), with remaining funds coming from Tech, VC/PE, and individual donors (~17.6% / $3.24M).
- **Mike Thompson (Total: ~$5.48M):** Funded through individual donors (~53.7% / $2.95M) and Political Action Committees (~44.5% / $2.44M).

### Mike Thompson Individual Donor Breakdown (~$2.72M Itemized)
- **Agriculture & Wine:** ~$820,000 (30% of individual)
- **Real Estate & Legal Services:** ~$680,000 (25% of individual)
- **Healthcare & Pharmaceuticals:** ~$540,000 (20% of individual)
- **Retirees, Education & Civic:** ~$410,000 (15% of individual)
- **Tech, Energy & Other Services:** ~$270,000 (10% of individual)

---

## 🛠️ Usage & Setup

This is a standalone, client-side web application. No server installation or build steps are required.

1. Clone the repository or download `index.html`.
2. Open `index.html` in any modern web browser.
3. To host publicly via GitHub Pages, go to **Settings > Pages** in your repository and set the source branch to `main`.

---

## 🔍 Data Source & Disclaimers

- **Data Origin:** Compiled from Federal Election Commission (FEC) disclosures (Form 3 and Form 6 / Schedule E reports).
- **Educational Use:** This tool is created strictly for public transparency, educational research, and non-partisan informational purposes. It is not an official FEC system.

