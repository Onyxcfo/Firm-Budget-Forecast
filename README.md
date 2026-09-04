# Onyx Accounting Group — Firm Budget & Forecast (2026)

`Firm_Budget_Forecast_2026.xlsx` — driver-based budget model. Change any **yellow input cell**
and the model re-computes.

## The model now reproduces reality

Rates and utilization are set from three months of measured billing rather than a rate card:

| | Model | Jun–Aug actual | |
|---|---:|---:|---|
| Billable hours / month | 645.0 | 651.5 | −1.0% |
| Revenue / month | $101,780 | $101,711 | +0.1% |

## 2026 base case

| | Jan–Jul actual | Aug–Dec budget | Year |
|---|---:|---:|---:|
| Revenue | $692,433 | $504,250 | **$1,196,683** |
| COGS | $363,778 | $236,611 | $600,389 |
| Gross profit | $328,655 | $267,639 | $596,294 (49.8%) |
| Operating expenses | $58,644 | $138,504 | $197,148 |
| **Net income** | **$270,012** | **$129,134** | **$399,146** (33.4%) |
| **Pro-forma net income** | | | **$238,210** |

Growth (new clients, new hires) is **switched off** so the base case is real. Turn it on in the
Growth & Hiring tab.

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
capped so overtime doesn't read above 100%. Each person's **billable mix** now sets how much of
their cost sits in COGS.

| Person | Utilization | COGS share |
|---|---:|---:|
| Steven Nikolov | 96.6% | 50% (policy) |
| Lisa Danforth | 96.2% | 83.5% |
| Jessica Bumphus | 94.5% * | 91.0% |
| Christine Johnson | 95.0% | 81.7% |
| Valentina Dikova | 99.8% | 89.3% |
| Josephine Mack | — | 0% (policy) |

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
| **Benefits** | Insperity 1000-Deductible medical by tier, 401(k) match, PEO fees. |
| **Monthly Capacity** | 2026 calendar → billable hours → revenue, per person. Owner residual block and the basis bridge. |
| **Growth & Hiring** | New clients and hires (off in the base case) plus the live office-space block. |
| **Budget P&L** | Pure budget, all 12 months. |
| **Forecast 2026** | Jan–Jul actual, Aug–Dec budget, plus the pro-forma. |
| **Owner Earnings** | Salary, K-1 income and the tax that follows. |

## Open items

- **Basis mix.** Jan–Jul are cash-basis QuickBooks actuals; Aug–Dec are accrual. The billing analysis shows **$20,110 earned but not invoiced** at 31 August. Converting the actuals to accrual is the last real inconsistency.
- **August is available.** The billing analysis has August earned revenue of $97,452. Pull the August QuickBooks P&L and move the Forecast cut-over from 7 to 8.
- **Still unpriced:** VV1012 LLC and Building & Development Professionals bill real time but aren't on the master card. Four clients were dropped from the master — Foothills Reserve among them, which billed 8.4 hours in the window.
- **Benefit tiers** reproduce the census in total but guess who holds which. The 401(k) can't start retroactively in 2026.

## Sources
Rates — *Clients Billing Rates Master Sheet 2026* (Sept) and *Onyx Client Billing Analysis Jun–Aug 2026*.
Utilization — *Onyx Utilization Model Apr–Aug 2026*. Office — *Office Space Cost Estimate*, Aug 2026.
Benefits — *Insperity HR360 proposal*, 12 Aug 2026. Actuals — QuickBooks P&L Jan–Jul 2026 (cash).

> Yellow = input · Blue = typed actual · Green = from another tab · Black = formula.
