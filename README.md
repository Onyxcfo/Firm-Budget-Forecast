# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` — driver-based budget model. Change any **yellow input cell**
and the model re-computes.

## What changed in this version

- **Angle replaces Insperity.** The Benefits tab is rebuilt around the Angle Health
  ANG TRAD 1000/2000 plan. Every column of the quote is an editable input.
- **One more PTO day for US staff** — 88 hours a year, up from 80. Valentina is unchanged.
- **A $70,014 labour-cost leak is closed.** See below; it is the largest number on this page.

## The labour-cost leak

Setting each person's COGS share to their billable mix put only that share of Lisa's,
Jessica's, Christine's and Valentina's cost into cost of goods sold. Nothing picked up the
rest, and the employer tax on the bonus was nowhere at all. **$70,014 of real labour cost
reached neither side of the Budget P&L.** The calibration check on Monthly Capacity had been
flagging it as a 281-hour discrepancy.

The operating-expense lines now absorb every person's non-COGS share:

| Line | Was | Now |
|---|---|---|
| Admin & Non-billable Labor | Josephine only — $80,000 | $140,992 |
| Admin & Non-billable Payroll Taxes | Steven + Josephine — $13,407 | $17,727 |
| Admin & Non-billable Benefits | Steven + Josephine | all staff — $18,569 |

Staff P&L fully-loaded cost now ties to the Budget P&L to the cent ($824,076.53), and the
calibration check reads **OK — formula reproduces the plan**.

## Benefits — Angle Health ANG TRAD 1000/2000

Onyx pays a fixed dollar amount per tier; the employee pays the balance of the premium.

| Tier | Premium | Onyx pays | Employee pays | Onyx share | Deductible | OOP max | Worst case to employee |
|---|---:|---:|---:|---:|---:|---:|---:|
| Employee only | $546.33 | $275.00 | $271.33 | 50.3% | $1,000 | $2,000 | $5,256 |
| Employee + spouse | $1,147.29 | $600.00 | $547.29 | 52.3% | $2,000 | $4,000 | $10,567 |
| Family | $1,693.61 | $900.00 | $793.61 | 53.1% | $2,000 | $4,000 | $13,523 |

Employer cost, current census: **$4,573/mo — $54,879/yr** (medical $35,400, 401(k) match at 3%
$19,479). The Insperity proposal was $8,106/mo — **$42,389 a year cheaper**, and employees pay
less too ($271 / $547 / $794 against $338 / $676 / $1,014), because the underlying premium is
lower rather than because Onyx absorbed more of it.

Gone with Insperity: the $183/employee/month HR admin fee, 0.17% workers' comp and EPLI,
the 0.233% payroll-tax allocation, and the $2,824.61 enrollment fee.

**Two things to set**: the real effective month (`Benefits!B43` still carries the old Insperity
date of November) and each person's actual tier — the elections reproduce the census in total
but guess who holds which.

## 2026 base case

| | Jan–Jul actual | Aug–Dec budget | Year |
|---|---:|---:|---:|
| Revenue | $692,433 | $502,249 | **$1,194,682** |
| COGS | $363,778 | $233,415 | $597,193 |
| Gross profit | $328,655 | $268,833 | $597,489 (50.0%) |
| Operating expenses | $58,644 | $165,347 | $223,991 |
| **Net income** | **$270,012** | **$103,486** | **$373,498** (31.3%) |
| **Pro-forma net income** | | | **$211,416** |

Budget P&L, all twelve months budgeted: **$280,965**.

Growth (new clients, new hires) is **switched off** so the base case is real. Turn it on in the
Growth & Hiring tab.

## The model still reproduces reality

| | Model | Jun–Aug actual | |
|---|---:|---:|---|
| Billable hours / month | 642.7 | 651.5 | −1.4% |
| Revenue / month | $101,379 | $101,711 | −0.3% |

The extra PTO day costs about 2.3 billable hours a month across the firm.

## Rates — actual, weighted, by role

From the Jun–Aug 2026 billing analysis (1,112 billable entries, $305,132 earned):

| Role | Hours | Earned | **Weighted rate** |
|---|---:|---:|---:|
| CFO | 619.75 | $154,255 | **$248.90** |
| Controller | 427.25 | $62,678 | **$146.70** |
| Staff | 907.64 | $88,199 | **$97.17** |
| **Blended** | **1,954.64** | **$305,132** | **$156.11** |

`Assumptions!B36 = 4` selects these. Methods 1–3 (simple average, hours-weighted, calibrated card)
remain available.

## Utilization — per person

From the Apr–Aug 2026 utilization model, measured against the 35-billable + 5-admin hour goal and
capped so overtime doesn't read above 100%. Each person's **billable mix** sets how much of their
cost sits in COGS.

| Person | Utilization | COGS share | PTO hrs/yr |
|---|---:|---:|---:|
| Steven Nikolov | 96.6% | 50% (policy) | 88 |
| Lisa Danforth | 96.2% | 83.5% | 88 |
| Jessica Bumphus | 94.5% * | 91.0% | 88 |
| Christine Johnson | 95.0% | 81.7% | 88 |
| Valentina Dikova | 99.8% | 89.3% | — |
| Josephine Mack | — | 0% (policy) | 88 |

\* Cindi's Apr–Aug history as the Controller proxy.

## Office space — from October

$33.50/SF on 2,750 SF = **$7,677/mo**, three months in 2026 ($23,031 against $3,600 of existing
rent). Full run-rate $92,125/yr versus $14,400 today — **$77,725/yr incremental**.

Base rent only. Fit-out, furniture, cabling, moving, signage and deposit are not included, and a
NNN quote would add $8–$12/SF. There's an input row for the one-time cost, currently zero.

## Tabs

| Tab | What it does |
|-----|--------------|
| **Bill Rates** | Rate card per client, plus the actual role-weighted rates that drive the model. |
| **Assumptions** | Hours, PTO, employer tax, owner comp, and the mode switches: rate method (B36), owner hours (B38), bonus source (B40). |
| **Staff P&L** | Pay, labour burden, loaded cost per hour, gross profit per person. Quarterly bonus block, operational scorecard, Josephine's pay options. |
| **Benefits** | Angle medical by tier, elections, 401(k) match, plan start, employer cost summary. |
| **Monthly Capacity** | 2026 calendar → billable hours → revenue, per person. Owner residual block and the basis bridge. |
| **Growth & Hiring** | New clients and hires (off in the base case) plus the live office-space block. |
| **Budget P&L** | Pure budget, all 12 months. |
| **Forecast 2026** | Jan–Jul actual, Aug–Dec budget, plus the pro-forma. |
| **Owner Earnings** | Salary, K-1 income and the tax that follows. |

## Open items

- **Angle effective date.** `Benefits!B43` is still November, carried over from the superseded
  Insperity start. Two months of benefit cost land in 2026 at that setting.
- **Benefit elections** reproduce the census in total but guess who holds which tier.
- **Basis mix.** Jan–Jul are cash-basis QuickBooks actuals; Aug–Dec are accrual. The billing analysis shows **$20,110 earned but not invoiced** at 31 August. Converting the actuals to accrual is the last real inconsistency.
- **August is available.** The billing analysis has August earned revenue of $97,452. Pull the August QuickBooks P&L and move the Forecast cut-over from 7 to 8.
- **Still unpriced:** VV1012 LLC and Building & Development Professionals bill real time but aren't on the master card. Four clients were dropped from the master — Foothills Reserve among them, which billed 8.4 hours in the window.
- **Dental and vision** are not quoted. There is an employer-cost input on the Benefits tab that flows straight to the P&L.

## Sources
Rates — *Clients Billing Rates Master Sheet 2026* (Sept) and *Onyx Client Billing Analysis Jun–Aug 2026*.
Utilization — *Onyx Utilization Model Apr–Aug 2026*. Office — *Office Space Cost Estimate*, Aug 2026.
Benefits — Angle Health ANG TRAD 1000/2000 quote. Actuals — QuickBooks P&L Jan–Jul 2026 (cash).

> Yellow = input · Blue = typed actual · Green = from another tab · Black = formula.
