# BatterySure AI — Pilot MVP v0.1

A browser-based EV valuation and battery-assessment workflow prototype for the India-first pilot.

## Run locally

1. Extract the ZIP file.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox or Safari).
3. Start with **Valuation** and enter a vehicle.
4. Save the assessment. It appears in Overview, Inventory and Reports.
5. Use **Print / Save PDF** to create a report.

No build step, server or API key is required for this prototype.

## Included

- Dashboard with assessment and inventory metrics
- Vehicle valuation form for electric 2W, 3W and 4W
- Transparent preliminary valuation heuristic
- Optional manually entered battery SOH and evidence classification
- Local inventory register
- Printable assessment report
- JSON export/import of local workspace data
- Responsive desktop/mobile layout

## Important limitations

This is a functional front-end pilot, not a production SaaS service. Data is stored only in the current browser using localStorage. It is not backed up or shared across devices. There is no authentication, multi-tenant separation, cloud database, payment processing, diagnostic hardware integration, OEM/VAHAN/auction data feed, API, server-side audit trail or production security review.

Valuations are indicative heuristics, not market quotations, certified appraisals or lending decisions. The model uses user-entered original price, age, odometer, condition and optional SOH. SOH must come from supported BMS diagnostics or independent testing; it must never be inferred from a photo or registration number. Do not use this prototype for lending, collateral, purchase or insurance decisions without independent inspection and calibration against verified transactions.

## Next production milestones

1. Validate the workflow and pricing with 10–15 Bengaluru dealers/fleet operators/NBFC users.
2. Build a secure backend (PostgreSQL + API), authentication, roles, tenant isolation and audit logs.
3. Obtain lawful, licensed data sources and verified completed transaction data; calibrate valuation by model/city/year.
4. Integrate supported battery diagnostic devices/BMS data and preserve evidence provenance.
5. Add payment gateway, subscriptions, report signing, monitoring, backups and security testing.
6. Pilot with paid customers before international rollout.
