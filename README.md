# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` — driver-based budget model. Change any **yellow input cell**
and the model re-computes.

## Start here — Forecast 2026

The budget for the year. **January–July are the actual figures from the QuickBooks P&L**
(cash basis, typed in blue). **August–December are calculated from the budget** (green
formulas). A band under the month headers labels each column ACTUAL or BUDGET.

**Utilization toggle:** `Assumptions!B15`, mirrored on the Forecast tab. It moves the
**Aug–Dec budget months only** — the Jan–Jul actuals never move.

| Utilization | Net income | Pro-forma net income |
|---|---:|---:|
| 100% | $440,333 | $303,532 |
| 91% | $392,025 | $255,224 |

Jan–Jul actuals imply **90.5%** utilization; the Forecast tab shows that next to the toggle.

**When a month closes:** type its actual figures over that month's column and change the band
label from BUDGET to ACTUAL.

## Tabs

| Tab | What it does |
|-----|--------------|
| **Bill Rates** | 2026 rate per client. Blended average of the 42 priced clients — **$250.00 / $153.21 / $96.31** — drives the model. |
| **Assumptions** | Hours, PTO, utilization, employer tax rates, owner comp. The flat "hours × 4 weeks" block is legacy and feeds nothing. |
| **Staff P&L** | Pay + full labor burden (AZ/US employer tax + PEO) → loaded cost per hour and gross profit per person. |
| **Monthly Capacity** | Real 2026 calendar → working days → billable hours per person per month → revenue. Also drives hourly wage cost. |
| **Budget P&L** | Pure budget, all 12 months at full capacity. Source of the Aug–Dec figures. |
| **Forecast 2026** | The budget: Jan–Jul actual, Aug–Dec calculated. Plus a pro-forma restating the year with all costs expensed. |

## Forecast 2026 (at 100% utilization)

| | Jan–Jul actual | Aug–Dec budget | Total 2026 |
|---|---:|---:|---:|
| Revenue | $692,433 | $536,753 | $1,229,186 |
| COGS | $363,778 | $250,842 | $614,620 |
| Operating expenses | $58,644 | $115,589 | $174,233 |
| **Net income** | **$270,012** | **$170,321** | **$440,333** |

Every Jan–Jul figure ties to the source QuickBooks P&L to the cent.

### Why there are two net income numbers

The Jan–Jul actuals carry **no owner compensation, admin salary, PEO benefits or IT** — those
aren't on the QuickBooks P&L. The Aug–Dec budget months do. The pro-forma block restates the
full year as if every month bore them:

| | |
|---|---:|
| Net income per the forecast | $440,333 |
| Less owner comp, admin salary + burden, PEO, IT for Jan–Jul | ($136,801) |
| **Pro-forma net income** | **$303,532** |

Use $440,333 for cash and distributions; use $303,532 to judge whether pricing and staffing work.

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

> Yellow = input · Blue = typed actual · Green = from another tab · Black = formula.
