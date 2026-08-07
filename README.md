# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` is a driver-based budget model. Change any **yellow input
cell** and the whole forecast re-computes.

## Tabs

| Tab | What it does |
|-----|--------------|
| **Bill Rates** | 2026 bill rate per client. Blended average of the 42 priced clients — **$250.00 CFO / $153.21 Controller / $96.31 Staff** — drives the model. |
| **Assumptions** | Every lever: hours, PTO, utilization, employer tax rates, owner comp. The flat "hours × 4 weeks" block is legacy and marked as such; Monthly Capacity is the live driver. |
| **Staff P&L** | Pay + full labor burden (AZ/US employer tax + PEO benefits) → **loaded cost per hour** and gross profit per person. |
| **Monthly Capacity** | **New.** Real 2026 calendar → working days → billable hours per person per month → revenue. Also drives hourly-staff wage cost. |
| **Budget P&L** | Monthly P&L in QuickBooks layout. Revenue and hourly wages vary with working days; salaries, taxes and benefits are annual ÷ 12. |
| **Budget vs Actual** | **New.** Paste QuickBooks actuals monthly. YTD variance plus a reconciliation of why actual net income reads higher than budget. |

## The 2026 calendar

| | |
|---|---|
| Weekdays | 261 |
| Company holidays (handbook) | 7 |
| **Working days** | **254** |
| Working hours per FTE @ 8 hrs/day | 2,032 |
| Paid hours per FTE (incl. holidays) | 2,088 |

Working days by month: Jan 21 · Feb 20 · Mar 22 · Apr 22 · May 20 · Jun 22 · Jul 22 ·
Aug 21 · Sep 21 · Oct 22 · Nov 20 · Dec 21.

Holidays are removed **once**, here, so the model never deducts them twice. Billable hours =
(gross working hours − admin hours − PTO for the month) × billable share × utilization.

## Why this changed the budget

The old flat convention — 40 hrs/week × 4 weeks × 12 = 1,920 hrs — assumed a 48-week year and
*also* subtracted holidays that a real calendar already excludes. Together that understated
billable capacity by about **168 hours per FTE per year**, roughly a month of work. Modelled
revenue moved from $1.14M to **$1.30M** at 100% utilization.

## Budget vs actual, Jan–Jul 2026

| | Budget | Actual | Variance |
|---|---:|---:|---:|
| Revenue | $763,218 | $692,433 | ($70,785) |
| COGS | $350,723 | $363,778 | ($13,055) |
| Operating expenses | $161,826 | $58,644 | $103,182 |
| **Net income** | **$250,670** | **$270,012** | **$19,342** |

$136,801 of budgeted cost has no counterpart in the actual P&L — owner comp $53,812, admin
salary $39,667, admin payroll taxes $7,272, PEO benefits $28,000, IT $8,050. That, not
out-performance, is the bulk of the apparent gap.

> ⚠ The loaded actuals are **cash basis** (per the QuickBooks footer); the budget is accrual.

## Key modeling choices

- **Team:** CFO = Steven Nikolov (50% client / 50% admin), Lisa Danforth · Controller = Cindi Campbell · Staff = Christine Johnson, Valentina Dikova (Bulgaria contractor, $4,200/mo) · Admin = Josephine Mack (15% billable).
- **Owner salary:** $184,500 = 2026 Social Security wage-base max; 50% in COGS, 50% below the line.
- **Labor burden:** employer SS (capped), Medicare 1.5%, FUTA, AZ SUTA 1.4%, plus a per-employee PEO input.
- **Utilization** is set to 100%. Jan–Jul actuals imply roughly **91%** — dial `Assumptions!B15` down for a realistic forecast.

## Sources
Bill rates — *Clients Billing Rates Master Sheet 2026*. Pay — *Cost Sheet.xlsx*. PTO (80 hrs)
and 7 paid holidays — *Onyx Handbook*. Actuals — *Onyx Accounting Group LLC Profit and Loss*,
Jan–Jul 2026.

> Yellow = input · Green = from another tab · Black = formula. Benefits are placeholders
> ($800/mo) — replace with your PEO quote.
