# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` — driver-based budget blended with actuals to date.
Change any **yellow input cell** and the model re-computes.

## Start here

**Forecast 2026** is the headline tab: actual months to date plus budget for the balance of
the year, in QuickBooks layout. Each month is labelled **ACTUAL** (green) or **BUDGET** (amber).

**To roll forward each month:** paste the new QuickBooks column into **Budget vs Actual**, then
raise the month counter in `Budget vs Actual!B6` by one. Everything re-blends automatically.

**Utilization toggle:** `Assumptions!B15`. It moves **budget months only** — actual months are
historical fact. YTD actuals imply **≈91%**; the Forecast tab shows the live setting and the
implied figure side by side.

| Utilization | Forecast net income |
|---|---:|
| 100% | $440,333 |
| 91% | $392,025 |

## Tabs

| Tab | What it does |
|-----|--------------|
| **Bill Rates** | 2026 rate per client. Blended average of the 42 priced clients — **$250.00 / $153.21 / $96.31** — drives the model. |
| **Assumptions** | Hours, PTO, utilization, employer tax rates, owner comp. The flat "hours × 4 weeks" block is legacy and feeds nothing. |
| **Staff P&L** | Pay + full labor burden (AZ/US employer tax + PEO) → loaded cost per hour and gross profit per person. |
| **Monthly Capacity** | Real 2026 calendar → working days → billable hours per person per month → revenue. Also drives hourly wage cost. |
| **Budget P&L** | Pure budget, all 12 months, at full capacity. |
| **Budget vs Actual** | Where actuals live. YTD variance and the reconciliation of the net income gap. |
| **Forecast 2026** | Actual + budget blended, plus a pro-forma restating the year with all costs expensed. |

## Forecast 2026 (actual Jan–Jul + budget Aug–Dec, 100% utilization)

| | |
|---|---:|
| Revenue | $1,229,186 |
| COGS | $614,620 |
| Gross profit | $614,566 |
| Operating expenses | $174,233 |
| **Net income** | **$440,333** (35.8%) |
| **Pro-forma net income** | **$303,532** |

The two net income figures differ because the actual months carry **no owner compensation,
admin salary, PEO benefits or IT** — those aren't on the QuickBooks P&L. The pro-forma block
restates the full year as if every month bore them ($136,801 of cost).

> Actuals are **cash basis** per the QuickBooks footer; the budget is accrual. Switch when ready.

## The 2026 calendar

261 weekdays − 7 handbook holidays = **254 working days** → 2,032 working hrs and 2,088 paid
hrs per FTE. By month: Jan 21 · Feb 20 · Mar 22 · Apr 22 · May 20 · Jun 22 · Jul 22 · Aug 21 ·
Sep 21 · Oct 22 · Nov 20 · Dec 21.

Holidays are removed **once**, here, so the model never deducts them twice. Billable hours =
(gross working hours − admin hours − PTO for the month) × billable share × utilization.

## Key modeling choices

- **Team:** CFO = Steven Nikolov (50% client / 50% admin), Lisa Danforth · Controller = Cindi Campbell · Staff = Christine Johnson, Valentina Dikova (Bulgaria contractor, $4,200/mo) · Admin = Josephine Mack (15% billable).
- **Owner salary:** $184,500 = 2026 Social Security wage-base max; 50% COGS, 50% below the line.
- **Labor burden:** employer SS (capped), Medicare 1.5%, FUTA, AZ SUTA 1.4%, plus a per-employee PEO input ($800/mo placeholder).

## Sources
Bill rates — *Clients Billing Rates Master Sheet 2026*. Pay — *Cost Sheet.xlsx*. PTO and
holidays — *Onyx Handbook*. Actuals — *Onyx Accounting Group LLC Profit and Loss*, Jan–Jul 2026
(cash basis).

> Yellow = input · Green = from another tab · Black = formula.
