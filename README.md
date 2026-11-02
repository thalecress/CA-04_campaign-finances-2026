# CA-04 Campaign Finance & Network Dashboard

An interactive campaign finance visualization for the California 4th Congressional District (CA-04) election between Eric Jones and Mike Thompson.

**Data as of: November 2, 2026.** Candidate committee totals are through the Oct 14 pre-general report. Later 48-hour notices are included through Oct 31 and are partial. Outside spending reflects notices through about Oct 30.

## 📌 Features

- **Layered Network Graph:** Money flows left to right, from funders to outside groups (Super PACs and hybrid PACs) to campaigns, with one lane per candidate. Line thickness shows dollar amount and arrows show direction.
- **Direct vs. Indirect Links:** Solid lines are reported contributions. Dotted lines are indirect: outside spending for or against a candidate, and donors who fund a candidate through a Super PAC. Indirect links can be toggled off.
- **Node Tracing:** Click any node to highlight its connections and see its direct and indirect links, with amounts and verification status.
- **Dragoneer Network Highlight:** Donors tied to Dragoneer Investment Group (Jones's former firm) are outlined in teal, with the network's share of New Leadership Now's receipts.
- **Verified Ledger:** Every flow is listed with its period, a verification badge (2+ sources, 1 source, derived, or sources differ), source links, and CSV export.

---

## 📊 Campaign Summary

Figures are from reports through Oct 14, 2026, unless noted.

- **Eric Jones (~$18.06M raised):** Self-funded through his own contributions (~$10.06M) and loans (~$4.80M), together 82.3% of receipts. Individual donors gave ~$3.19M (17.6%). No PAC contributions. Another ~$0.90M in 48-hour notices (Oct 16–28, including $900,000 from Jones himself) is not yet in the totals. FEC letter of Oct 25 requests loan documentation; response due Nov 30. It is not a finding of wrongdoing.
- **Mike Thompson (~$5.48M raised):** Individual donors ~$2.95M (53.7%) and PACs ~$2.44M (44.5%). Another ~$0.49M in 48-hour notices (Oct 15–30) is not yet in the totals.

### Donor Geography (individual donors, estimated mailing location)
- **Thompson:** 2,149 identified donors, 43.2% in CA-04 (38.1% of dollars).
- **Jones:** 690 identified donors, 11.6% in CA-04 (4.9% of dollars).

### Outside Spending (reported independent expenditures)
- **For Jones / against Thompson:** ~$5.16M, mostly New Leadership Now ($1.25M for Jones, $3.87M against Thompson). California Leadership Fund adds $33k against Thompson.
- **For Thompson / against Jones:** ~$7.14M. BDA PAC ($1.31M for Thompson, $3.13M against Jones), Article One PAC ($1.29M for, $203k against), Center Forward Committee ($750k), American Hospital Association PAC ($275k), NAR PAC ($115k), Public Integrity Alliance ($63k), and smaller groups.

### New Leadership Now Funding (raised ~$5.77M)
- **Elisa Stad:** $4.25M cumulative (~74%). She is the wife of Dragoneer's founder. About $2.0M was given by May 28.
- **Dragoneer network total:** ~$4.93M (~85%): Elisa Stad, Dan Gillespie ($400k), Gillespie Family Trust ($225k), and Jared Middleman ($50k).
- **Other named donors:** Maurice Duca ($250k) and TPG partners Coulter and Trujillo ($100k each).

---

## ✅ Data Validation Notes

- **Corrections to the previous version:** The earlier dataset was an incomplete sample. It mislabeled the Jones self-funding split, omitted six or more outside groups, and showed California Leadership Fund as pro-Thompson with $1.1M when filings show $33k *opposing* Thompson. It also attributed $3.5M of New Leadership Now's funding to a second donor; filings show it came from Elisa Stad.
- **Removed (could not be verified):** Sector breakdowns (Tech, VC, Agriculture & Wine, Real Estate & Legal, Healthcare, Retirees, etc.) and vendor payments (Red Dog Strategies, Sexton Group, Common Blue Strategies). Common Blue Strategies appears in filings as a *contributor* to New Leadership Now ($76,560), and Red Dog Strategies as a payee of Jones's campaign, not clearly of the PAC.
- **Known gaps:** The FEC had an electronic-filing outage that ended Oct 28. Some committee amendments could not be fully checked. Funders of outside groups other than New Leadership Now are not traced. 48-hour notices omit gifts under $1,000.
- **Source conflicts:** New Leadership Now's spending against Thompson is $3.87M in the Nov 2 tracker and $3.47M in an Oct 26 analysis (different dates and methods). A disputed $266,633.50 purchase is excluded.
- **Indirect links:** Dotted donor-via-PAC links are inferred relationships, not filed transactions. The Gillespie Family Trust link to Dan Gillespie is inferred by reporters, not stated in the filing.

Primary source for most figures: the Napa Valley Register's Nov 2, 2026 tracker, which is built from FEC filings. Key figures are cross-checked against LocalCandidates.org, the Press Democrat, and itemized donor reporting from Davisite, Davis Vanguard, and Judy Tipple's Substack (advocacy outlets that cite FEC records). Full source list is at the bottom of the dashboard. Verify against the FEC before relying on any figure.

---

## 🛠️ Usage & Setup

This is a standalone, client-side web application with no dependencies, server installation or build steps.

1. Clone the repository or download `index.html`.
2. Open `index.html` in any modern web browser.
3. To host publicly via GitHub Pages, go to **Settings > Pages** in your repository and set the source branch to `main`.

---

## 🔍 Data Source & Disclaimers

- **Data Origin:** Compiled from Federal Election Commission (FEC) disclosures (Form 3, Form 6 and Schedule E reports) as reported by the sources listed in the dashboard.
- **Not Official:** Figures are reported filings, not live balances, and amendments can change them.
- **Educational Use:** This tool is created strictly for public transparency, educational research, and non-partisan informational purposes. It is not an official FEC system.
