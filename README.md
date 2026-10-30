# Onyx Accounting Group — Budget 2027

`Firm_Budget_Forecast_2026.xlsx` — a four-sheet chain. Each sheet feeds the next.

```
Bill Rates  →  Staff P&L  →  Monthly Capacity  →  Budget 2027
```

| Sheet | What it does | Feeds |
|---|---|---|
| **Bill Rates** | Client card. Simple and weighted averages by role; a one-cell method selector. | The bill rate per role → Staff P&L column T |
| **Staff P&L** | Pay, employer tax, benefits (medical tier, PEO, 401k), loaded cost, COGS %, revenue and gross profit by person. Tax rates and the Angle / Questco figures sit in blocks B and C on the same sheet. | Cost, burden and COGS split → Budget 2027 |
| **Monthly Capacity** | 2027 calendar — weekdays, holidays, working hours by month. PTO. Editable utilization per person with the Apr–Aug 2026 history beside it. Billable hours, revenue and pay by month. | Revenue and pay by month → Budget 2027 |
| **Budget 2027** | Monthly P&L, QuickBooks layout, twelve months plus total. Operating expenses typed once in the Annual-input column. | — |
| Owner Earnings | Salary, K-1 and the tax that follows, off the 2027 budget. | — |
| Assumptions | **Pending deletion.** A one-screen index of where each former item now lives. | — |

Benefits, Growth & Hiring, Guide, Budget P&L and Forecast 2026 are deleted. No forecast.

## Bill rates — weighted, not simple

The weighted average is the more accurate of the two: each client's card rate is weighted by the
hours the firm actually puts into that client, so the clients that drive the hours drive the rate.
The simple average lets a one-hour client count as much as a 218-hour client.

| Role | Simple | **Weighted (used)** | Realised Jun–Aug |
|---|---:|---:|---:|
| CFO | $248.12 | **$249.62** | $248.90 |
| Controller | $155.42 | **$156.95** | $146.70 |
| Staff | $96.04 | **$96.32** | $97.17 |

`Bill Rates!C68` picks the method: 1 simple, 2 weighted, 3 realised. The realised Controller
rate sits $10 under the card — write-downs and clients billed below card, worth knowing.

## Staff P&L

| Person | Basis | Base comp | Medical | Benefits $/yr | Fully loaded | COGS % | Bill rate | Hrs/yr | Revenue | Gross profit |
|---|---|---:|---|---:|---:|---:|---:|---:|---:|---:|
| Steven Nikolov | Salary | $184,500 | FAM | $12,339 | $211,106 | 50% | $249.62 | 821 | $205,038 | $99,485 |
| Lisa Danforth | Salary | $176,000 | EE | $5,455 | $195,072 | 100% | $249.62 | 1,636 | $408,462 | $213,390 |
| Jessica Bumphus | Hourly $60 | $125,280 | FAM | $12,339 | $147,356 | 100% | $156.95 | 1,608 | $252,391 | $105,035 |
| Christine Johnson | Hourly $40 | $83,520 | ES | $9,061 | $101,821 | 100% | $96.32 | 1,615 | $155,590 | $53,769 |
| Valentina Dikova | Contractor | $50,400 | — | — | $50,400 | 100% | $96.32 | 1,705 | $164,259 | $113,859 |
| Josephine Mack | Salary | $80,000 | waived | $2,177 | $104,813 | 5% | $96.32 | 271 | $26,150 | $20,909 |
| **Firm** | | **$699,700** | | **$41,371** | **$810,569** | | $158.25 | **7,658** | **$1,211,890** | **$606,447** |

**Benefits are on this sheet** (block C). Angle ANG TRAD 1000/2000: Onyx pays 50% of the premium,
never less than Angle's $219.52 minimum — $273.17 employee-only, $573.65 employee + spouse, $846.81
family. The Questco PEO is $181.44 per W-2 employee a month ($117 admin + the group cover ÷ 5),
charged to everyone on payroll, medical or not. The 401(k) match is at 0%.

Elections as you set them: Jessica Family, Christine employee + spouse, Lisa employee only.
**Steven is Family and Josephine is waiving — carried from the Questco census, not confirmed.**

Employer payroll tax (block B) is computed on base comp plus bonus, wage base by wage base, with
2026 parameters. Update the Social Security base when SSA publishes 2027.

## Monthly Capacity — 2027

261 weekdays, 7 handbook holidays, **254 working days**, 2,088 paid hours. Billable capacity at the
35-hour goal is 7 hours per working day — 1,778 hours per full-time person before PTO.

Utilization is one editable cell per person, with the Apr–Aug 2026 figure beside it:

| Person | Delivery allocation | Historical | Used | Billable hrs/wk | % of paid hours |
|---|---:|---:|---:|---:|---:|
| Steven | 50% | 96.6% | 96.6% | 16.2 | 39% |
| Lisa | 100% | 96.2% | 96.2% | 32.2 | 78% |
| Jessica | 100% | 94.5% * | 94.5% | 31.7 | 77% |
| Christine | 100% | 95.0% | 95.0% | 31.8 | 77% |
| Valentina | 100% | 99.8% | 99.8% | 33.6 | 82% |
| Josephine | 100% | 16.0% | 16.0% | 5.3 | 13% |

\* Cindi Campbell's history. Historical rates measure against the 35-hour goal after time off,
which is why they read high; "% of paid hours" is the everyday meaning of utilization.

PTO is 11 days for US staff and 10 for Valentina, spread in proportion to working days. Hourly pay
follows paid hours in the month, so March and December cost more than February.

## Budget 2027

| | 2027 | Per month | % rev |
|---|---:|---:|---:|
| Revenue | **$1,211,890** | $100,991 | |
| Cost of goods sold | $605,443 | $50,454 | 50.0% |
| **Gross profit** | **$606,447** | $50,537 | **50.0%** |
| Operating expenses | $362,983 | $30,249 | 30.0% |
| **Net income** | **$243,464** | $20,289 | **20.1%** |

Revenue runs $95,424 in the 20-working-day months and $109,738 in March. Bonuses pay out in March,
June, September and December. Rent is $96,000 — the new office at full run-rate, for which 2027 is
the first full year. Every operating-expense line is a 2026 figure carried forward; type over
column P.

Check row at the bottom of the sheet: labour cost in the budget equals Staff P&L fully-loaded cost
to the cent ($810,569).

## Open

- **Delete Assumptions?** Everything on it has a new home (listed on the tab). Two items were
  dropped outright — the owner-hours residual mode and the bonus scorecard switch.
- **Steven's and Josephine's elections** are carried from the Questco census — confirm.
- **2027 tax parameters**: Social Security wage base, standard deduction, brackets are 2026 figures.
- **December holidays**: Christmas falls on a Saturday in 2027. Two days are budgeted; pick which.

> Yellow = input · Green = from another sheet · Black = formula · Grey = reference only.
