# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` — driver-based budget model. Change any **yellow input cell**
and the model re-computes.

## What changed in this version

- **Medical rebuilt on the Angle Cost-by-Tier structure** from the CapFi / Questco cost model.
  All three plans priced by tier, 50%-of-premium funding with Angle's minimum-funding floor,
  per-person elections.
- **PEO costs held separate.** Questco's fees are on the tab but excluded from the P&L until a
  single switch says otherwise.
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

## Benefits — Angle Health, funded as a percentage of premium

Onyx funds **50% of whatever plan each person elects**, never less than Angle's minimum funding
($219.51/mo, 50% of the cheapest employee-only rate) and never more than the premium. Switch
`Benefits!C15` to *Fixed dollars* and Onyx pays a flat amount per tier instead, with the employee
absorbing the whole difference between plans.

All three plans are priced for every tier. What Onyx pays if the whole firm takes one plan:

| Plan | HSA | Deductible (ind/fam) | OOP max (ind/fam) | Onyx $/yr | Employee $/yr | Worst case |
|---|:--:|---|---|---:|---:|---:|
| ANG HDHP 3400/5000 | Y | $3,400 / $6,800 | $5,000 / $10,000 | **$24,498** | $24,498 | $59,498 |
| ANG TRAD 2000/4000 | N | $2,000 / $4,000 | $4,000 / $8,000 | $27,460 | $27,460 | $55,460 |
| ANG TRAD 1000/2000 | N | $1,000 / $2,000 | $2,000 / $4,000 | $30,485 | $30,485 | $44,485 |

**Everyone is defaulted to the HDHP 3400/5000**, where the cost model leaves them. Changing a
person's plan is one cell in block 4.

Census: Steven and Jessica Family, Lisa employee-only, Christine employee + spouse, Josephine
waiving, Valentina not on US benefits. Four enrolled.

Employer cost: **$3,665/mo — $43,977/yr** (medical $24,498 + 401(k) match at 3% $19,479).
Effective **1 October**, so three months land in 2026 — $10,994.

### PEO (Questco) — carried, not costed

Block 8 holds the Questco quote: $117 PEPM admin, workers' comp and EPLI, life and LTD elected,
cyber and STD declined — **$907/mo, $10,886/yr recurring**, plus $1,000 implementation. It is
**excluded from the P&L** until `Benefits!B103` is set to Yes. Payroll taxes on the Questco quote
are a pass-through and are not modelled here; the workbook computes them wage base by wage base.

## 2026 base case

| | Jan–Jul actual | Aug–Dec budget | Year |
|---|---:|---:|---:|
| Revenue | $692,433 | $502,249 | **$1,194,682** |
| COGS | $363,778 | $235,083 | $598,861 |
| Gross profit | $328,655 | $267,166 | $595,821 (49.9%) |
| Operating expenses | $58,644 | $165,527 | $224,171 |
| **Net income** | **$270,012** | **$101,639** | **$371,650** (31.1%) |
| **Pro-forma net income** | | | **$222,318** |

Budget P&L, all twelve months budgeted: **$291,867**.

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
| **Benefits** | Angle rate card, contribution policy, cost by tier, elections, 401(k), employer cost summary, and the Questco PEO block (excluded). |
| **Monthly Capacity** | 2026 calendar → billable hours → revenue, per person. Owner residual block and the basis bridge. |
| **Growth & Hiring** | New clients and hires (off in the base case) plus the live office-space block. |
| **Budget P&L** | Pure budget, all 12 months. |
| **Forecast 2026** | Jan–Jul actual, Aug–Dec budget, plus the pro-forma. |
| **Owner Earnings** | Salary, K-1 income and the tax that follows. |

## Open items

- **Which plan.** Everyone is defaulted to the HDHP 3400/5000. Moving the firm to the
  TRAD 1000/2000 costs $30,485/yr instead of $24,498 — but cuts the worst case for employees from
  $59,498 to $44,485. One cell per person.
- **Two errors in the CapFi / Questco cost model.** Its *Cost by Tier* enrolled count is hard-typed
  to 1 for the Family rows when two people hold Family, so its plan totals understate Onyx's cost
  by one family — $8,166 on the HDHP. Its *Elections* tab computes person by person and is right.
  Separately, its FICA figure exceeds 7.65% of the quoted payroll and does not appear to cap Social
  Security at the wage base.
- **Pay figures differ.** The cost model assumes Steven $186,000, Lisa $178,094, Jessica $135,000,
  Christine $79,228. This budget carries $184,500 / $176,000 / $125,280 / $83,520. Reconcile before
  either is quoted externally.
- **Basis mix.** Jan–Jul are cash-basis QuickBooks actuals; Aug–Dec are accrual. The billing analysis shows **$20,110 earned but not invoiced** at 31 August. Converting the actuals to accrual is the last real inconsistency.
- **August is available.** The billing analysis has August earned revenue of $97,452. Pull the August QuickBooks P&L and move the Forecast cut-over from 7 to 8.
- **Still unpriced:** VV1012 LLC and Building & Development Professionals bill real time but aren't on the master card. Four clients were dropped from the master — Foothills Reserve among them, which billed 8.4 hours in the window.
- **Dental and vision** are not quoted. There is an employer-cost input on the Benefits tab that flows straight to the P&L.

## Sources
Rates — *Clients Billing Rates Master Sheet 2026* (Sept) and *Onyx Client Billing Analysis Jun–Aug 2026*.
Utilization — *Onyx Utilization Model Apr–Aug 2026*. Office — *Office Space Cost Estimate*, Aug 2026.
Benefits — *Onyx Angle / Questco Cost Model* and Angle Health quote 400798 via CapFi, underwritten
30 Jul 2026. Actuals — QuickBooks P&L Jan–Jul 2026 (cash).

> Yellow = input · Blue = typed actual · Green = from another tab · Black = formula.
