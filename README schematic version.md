# Collateral Climate Radar (CCR) — Demo

**Making Climate Risk Visible Across Real Estate Collateral.**

## Open it
Open `index.html` in any modern browser. No server, build step, or API key is needed. The whole demo works offline.

## What is in the app
- **Executive Overview:** five headline metrics, risk distribution, assessment coverage, exposure by emirate, and three findings computed from the data.
- **Climate Risk Map:** a schematic coordinate map with one marker per collateral asset, coloured by risk, unknown, or not assessed. Click a marker to see its property card. Overlapping markers are listed for selection.
- **Collateral Portfolio:** search, emirate and risk filters, paging, a record panel with all 47 source fields, and CSV export (filtered or full).
- **Flood Scenario:** five-level rainfall slider. Exposed count, exposed value, associated loans, and change against the Moderate baseline update live.
- **Risk Analysis:** top assessed risks, a "needs attention" ranking, highest flood, heat, and loan exposure, emirate and category concentration, and data gaps.
- **CCR Intelligence:** a local rule-based assistant in English and Arabic. It answers from the live dataset and says plainly when a question is outside the data.
- **Methodology & Data:** sources, formulas, limitations, CBUAE tiers, NGFS tags, and the regulatory statement.
- **Audit Trail:** the actions performed in your session.
- **Generate Executive Report:** downloads a PNG in Arabic or English with current values. The assistant can also trigger it ("generate a report" / "اعمل لي تقرير").

Arabic is the default (right-to-left). Light and dark modes can be switched. A "Real Estate & Land Only" toggle is available.

## Data
- The app uses the 1,000 synthetic records from the supplied workbook (Main_Data). No records were generated, resampled, or changed.
- Hazard data is attributed to ThinkHazard! — World Bank GFDRR (thinkhazard.org).
- Source tier labels are shown for reference only. They do not match the cutoffs in the workbook's Data_Explanation sheet, and the app discloses this.

## Key rules
- Flood score = 10 × flood intensity × elevation × coast × protection, capped at 100. Heat score = 10 × extreme heat × material, capped at 100.
- Scenario exposure = scenario flood score ≥ 65. Multipliers are 0.60, 0.80, 1.00, 1.20, 1.40.
- Overall risk = 10 × composite hazard score. Demo thresholds: 35–64 Medium, 65–100 High. These are CCR demo thresholds, not regulatory thresholds.
- Implied valuation = exposure ÷ loan-to-value ratio (derived, not an appraisal).
- Expected climate loss is the source-modelled figure. It is shown separately and never added to exposed value.

## Not included
- Satellite imagery. The map is a coordinate plot.
- CSV import, record editing, and Presenter Mode.
- Marker clustering. Overlapping markers are listed on click.

All figures are synthetic. Demo environment only. Confidential — Hackathon Use.
