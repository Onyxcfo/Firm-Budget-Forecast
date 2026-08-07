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
| 100% | $427,064 | $290,263 |
| 91% | $378,756 | $241,955 |

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
| **Owner Earnings** | Steven's salary, K-1 pass-through income and the tax that follows. Every tax parameter is an editable input. |

## Forecast 2026 (at 100% utilization)

| | Jan–Jul actual | Aug–Dec budget | Total 2026 |
|---|---:|---:|---:|
| Revenue | $692,433 | $536,753 | $1,229,186 |
| COGS | $363,778 | $264,110 | $627,888 |
| Operating expenses | $58,644 | $115,589 | $174,233 |
| **Net income** | **$270,012** | **$157,052** | **$427,064** |

Every Jan–Jul figure ties to the source QuickBooks P&L to the cent.

### Why there are two net income numbers

The Jan–Jul actuals carry **no owner compensation, admin salary, PEO benefits or IT** — those
aren't on the QuickBooks P&L. The Aug–Dec budget months do. The pro-forma block restates the
full year as if every month bore them:

| | |
|---|---:|
| Net income per the forecast | $427,064 |
| Less owner comp, admin salary + burden, PEO, IT for Jan–Jul | ($136,801) |
| **Pro-forma net income** | **$290,263** |

Use $427,064 for cash and distributions; use $290,263 to judge whether pricing and staffing work.

> Actuals are **cash basis** per the QuickBooks footer; the budget is accrual. Switch when ready.

## The 2026 calendar

261 weekdays − 7 handbook holidays = **254 working days** → 2,032 working hrs and 2,088 paid
hrs per FTE. By month: Jan 21 · Feb 20 · Mar 22 · Apr 22 · May 20 · Jun 22 · Jul 22 · Aug 21 ·
Sep 21 · Oct 22 · Nov 20 · Dec 21.

Holidays are removed **once**, here, so the model never deducts them twice. Billable hours =
(gross working hours − admin hours − PTO for the month) × billable share × utilization.

## Quarterly discretionary bonus

Defined in a block on **Staff P&L** below the main table. Each person has a target % of base
(5% placeholder); the quarterly amount is target ÷ 4 × that quarter's **payout factor** — the
discretionary lever, set per quarter. Paid in March, June, September and December. **The owner
is excluded** (target 0%).

| | Annual | Employer tax | Total cost |
|---|---:|---:|---:|
| W-2 employees → payroll lines | $22,718 | $1,719 | $24,437 |
| Contractor → cost of labor | $2,520 | — | $2,520 |
| **Total** | **$25,238** | **$1,719** | **$26,957** |

Employer Social Security applies only to bonus dollars still under the wage base after base pay
(Lisa's $8,800 bonus is taxed on $8,500 of headroom); Medicare applies to all of it; FUTA and
SUTA are already maxed by base pay. Bonuses and their tax are folded into each person's
fully-loaded cost, so loaded cost per hour and gross profit already reflect the plan.

On Forecast 2026 only the September and December payments land — March and June sit inside the
Jan–Jul actuals.

## Owner Earnings

Models Steven as an S-corp owner: W-2 salary carries FICA, the remaining profit reaches his 1040
through the K-1 free of FICA.

| | |
|---|---:|
| Firm profit before owner compensation | $509,884 |
| Less salary and its employer tax | ($198,767) |
| **K-1 pass-through income** | **$311,116** |
| Taxable income (after QBI) | $426,255 |
| **Total tax** | **$114,134** (23.0%) |
| **Net after-tax cash to owner** | **$381,482** |

Accounting is a **Specified Service Trade or Business**, so the 20% QBI deduction phases out as
income rises — at this level it is ~60% available, worth $37,161. Every tax parameter (brackets,
standard deduction, thresholds, AZ rate) is an editable input; the shipped figures are estimates,
so verify them before relying on the output.

## Key modeling choices

- **Team:** CFO = Steven Nikolov (50% client / 50% admin), Lisa Danforth · Controller = Cindi Campbell · Staff = Christine Johnson, Valentina Dikova (Bulgaria contractor, $4,200/mo) · Admin = Josephine Mack (15% billable).
- **Owner salary:** $184,500 = 2026 Social Security wage-base max; 50% COGS, 50% below the line.
- **Labor burden:** employer SS (capped), Medicare 1.5%, FUTA, AZ SUTA 1.4%, plus a per-employee PEO input ($800/mo placeholder).

## Sources
Bill rates — *Clients Billing Rates Master Sheet 2026*. Pay — *Cost Sheet.xlsx*. PTO and
holidays — *Onyx Handbook*. Actuals — *Onyx Accounting Group LLC Profit and Loss*, Jan–Jul 2026
(cash basis).

> Yellow = input · Blue = typed actual · Green = from another tab · Black = formula.
