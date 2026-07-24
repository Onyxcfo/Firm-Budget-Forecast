# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` is a driver-based budget model for the firm. Change any
**yellow input cell** and the whole forecast re-computes.

## Tabs

| Tab | What it does |
|-----|--------------|
| **Guide** | Legend, key outputs, and source/policy notes. |
| **Bill Rates** | 2026 bill rate per client (CFO / Controller / Staff). The blended average of the 42 priced clients — **$249.40 / $153.21 / $96.31** — drives the model. |
| **Assumptions** | Every lever: working hours, PTO/holidays, utilization, employer tax rates, owner comp, benefits. |
| **Staff P&L** | Per employee — pay → full labor burden (AZ/US employer tax + PEO benefits) → **loaded cost per hour**, billable hours (net of PTO & holidays), revenue, and **gross profit per staff member**. |
| **Budget P&L** | Monthly P&L in QuickBooks format: revenue, COGS (with benefits plugged in), operating expenses, and **Net Income**. |

## Key modeling choices

- **Team:** CFO = Steven Nikolov (50% client / 50% admin), Lisa Danforth · Controller = Cindi Campbell · Staff = Christine Johnson, Valentina Dikova (Bulgaria contractor) · Admin = Josephine Mack (15% billable, adjustable).
- **Billable hours:** 140 gross/mo − 20 admin = 120, less PTO (80 hrs/yr) and holidays (56 hrs/yr = 7 days) → **≈108.7 billable hrs/mo** at 100% utilization (dial-able).
- **Owner salary:** Steven at **$184,500 = 2026 Social Security wage-base max**; 50% sits in COGS (billable CFO work), 50% below the line as owner compensation.
- **Labor burden:** employer SS (capped), Medicare, FUTA, AZ SUTA, plus a per-employee PEO benefit input ($/mo) — all divided into a loaded cost per hour.
- **Contractor:** Valentina modeled at the Bulgaria all-in cost ($3,892.70/mo); no US payroll tax.

## Sources
- Bill rates — *Clients Billing Rates Master Sheet 2026*.
- Pay — *Cost Sheet.xlsx* (incl. Bulgaria Costs tab).
- PTO (80 hrs) & 7 paid holidays (56 hrs) — *Onyx Handbook*.
- P&L layout & OpEx run-rate defaults — *Onyx Accounting Group LLC P&L Format* (H1 2026).

> Yellow = input · Green = pulled from another tab · Black = formula. Benefit costs are placeholders ($800/mo) — replace with your PEO quote.
