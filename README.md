# Onyx Accounting Group — Annual Budget 2026

`Firm_Budget_Forecast_2026.xlsx` — **four tabs, one live page.**

| Tab | What it is |
|---|---|
| **Budget** | The whole model. Annual P&L on the left, every driver on the right, all on one screen. |
| **Benefits** | Angle rate card, contribution policy, cost by tier, and the Questco PEO quote. |
| **Bill Rates** | Client rate card — reference only. |
| **Owner Earnings** | Salary, K-1 and the tax that follows. |

Deleted: Assumptions, Staff P&L, Monthly Capacity, Growth & Hiring, Budget P&L, Forecast 2026,
Guide. Ten tabs became four.

## The Budget page

Freeze is set at row 6, so the headline strip stays on screen while you scroll. Change a yellow
cell in any block on the right and the P&L on the left moves.

| Block | Where | What it drives |
|---|---|---|
| 1. Annual P&L | A–D | The output. Annual, per month, % of revenue. |
| 2. Staff, capacity and cost | F–W, rows 7–14 | Pay, utilization, billable hours, revenue, burden, COGS split, gross profit per person. |
| 3. Capacity, rates and employer tax | F–H, rows 19–39 | Working days, the 35-hour goal, bill rates, payroll tax rates and wage bases. |
| 4. Benefits by person | M–U, rows 19–33 | Tier, plan, medical, 401(k), PEO — per person. |
| 5. Utilization check | F–M, rows 43–50 | The provided rates against billable hours a week and % of paid hours. |
| 6. Discretionary bonus | F–J, rows 56–63 | Target % and payout factor per person. |

## 2026 at the baseline

| | Annual | Per month | % rev |
|---|---:|---:|---:|
| Revenue | **$1,198,722** | $99,893 | |
| Cost of goods sold | $605,443 | $50,454 | 50.5% |
| **Gross profit** | **$593,279** | $49,440 | **49.5%** |
| Operating expenses | $363,983 | $30,332 | 30.4% |
| **NET INCOME** | **$229,296** | $19,108 | **19.1%** |

7,651 billable hours a year at a $156.67 blended rate.

**Against the file you sent back** ($1,219,372 revenue, $261,832 net income):

| | |
|---|---:|
| Revenue, from rebuilding capacity on an annual basis | −$20,650 |
| PEO cost, now charged per person | −$10,886 |
| PEO implementation, one-time | −$1,000 |
| **Net income** | **−$32,536** |

## PEO cost per person — the gap you spotted

You were right. The PEO was sitting behind a switch that was off, and nothing allocated it to
people. It is now charged to **every W-2 employee, medical or not**:

| | Per employee /mo |
|---|---:|
| Questco admin fee | $117.00 |
| Group cover — workers' comp & EPLI, basic life, LTD ÷ 5 | $64.44 |
| **PEO per W-2 employee** | **$181.44** |

**Josephine now costs $181.44 a month with no medical at all** — $2,177 a year. Valentina, a
Bulgaria contractor, is not a worksite employee and carries none of it.

Total benefits: **$41,371/yr** — medical $30,485 + PEO $10,886, plus $1,000 of implementation in
operating expenses. Cyber and short-term disability are declined; flip them to Yes on the
Benefits tab if that changes. The 401(k) match is at **0%** where you left it.

## COGS allocation — confirmed, and you were right

Your reading of my reasoning was exactly right, and the reasoning was wrong. I was splitting each
person's cost by their **billable mix** — billable hours ÷ hours worked — so Lisa sat at 83.5%,
Jessica 91.0%, Christine 81.7%, Valentina 89.3%, and their admin time landed in overhead.

The allocation you provided is the **delivery allocation** column of your own utilization model:
100% for delivery staff, 50% for Steven, 0% for Josephine. Those are different columns of the
same sheet and I used the wrong one.

The model now runs on your figures — delivery staff at **100%**, Steven at 50%, Josephine at 5%.
Admin time for delivery staff is a cost of delivery, not overhead. That moves about $56,000 of
cost from operating expenses into COGS; net income is unchanged by it, gross margin falls.

## Utilization — confirmed

The rates are **exactly** column I of the Summary tab of *Onyx Utilization Model Apr–Aug 2026*,
"Utilization % at capacity" — capped so overtime cannot read above 100%.

| Person | Provided rate | Delivery allocation | Used here | Billable hrs/wk | % of paid hours | Actual hrs/mo Apr–Aug |
|---|---:|---:|---:|---:|---:|---:|
| Steven Nikolov | 96.6% | 50% | 48.3% | 16.9 | 39% | 85.5 |
| Lisa Danforth | 96.2% | 100% | 96.2% | 33.7 | 78% | 139.5 |
| Jessica Bumphus | 94.5% * | 100% | 94.5% | 33.1 | 77% | 134.9 |
| Christine Johnson | 95.0% | 100% | 95.0% | 33.3 | 77% | 141.5 |
| Valentina Dikova | 99.8% | 100% | 99.8% | 34.9 | 81% | 131.0 |
| Josephine Mack | 16.0% | 100% | 16.0% | 5.6 | 13% | 23.7 |

\* Cindi Campbell's history as the Controller proxy.

**Why they read high:** they divide billable hours by the **35-hour-a-week goal** after holidays
and time off — not by paid hours. 96.2% of goal is 33.7 billable hours a week, which is 78% of
paid time. The "% of paid hours" column is the number most people mean by utilization.

Uncapped, the same model reads Steven 115.2%, Lisa 99.6%, Cindi 108.3%, Christine 95.4%,
Valentina 104.0% — several people billed **above** the goal. The rates are not inflated; the
denominator is a goal, not a year.

Steven's 96.6% is against his 50% delivery allocation, so the model carries 48.3% — 16.9 billable
hours a week, close to the 85.5 hours a month he actually logged.

**One number worth a look:** Valentina at 99.8% with 11 PTO days gives 1,698 hours a year. She
actually averaged 131 hours a month across Jun–Aug, which annualises to about 1,572. The model
runs about 8% hot on her.

## What changed from the driver-based model

- **Annual, not monthly.** One column, at the baseline assumptions. No 12-month calendar, no
  Jan–Jul actuals blended with an Aug–Dec budget.
- **Capacity is annual too**: 261 weekdays − 7 holidays − 11 PTO days = 243 working days ×
  7 billable hours at goal = **1,701 hours of billable capacity** per full-time person.
- **Growth & Hiring is gone.** It was zeroed anyway, so nothing moved.
- **Bill rates are direct inputs** — $250 CFO (yours), $146.70 Controller, $97.17 Staff — with
  the Jun–Aug actuals shown beside them in grey.

Staff fully-loaded cost ties to the P&L to the cent: **$810,569**, split $605,443 into COGS and
$205,126 into operating expenses.

## Open items

- **Valentina's hours** run about 8% above what she actually billed. Consider 92% or giving her
  PTO days.
- **Rent at $96,000** is the full office run-rate for twelve months. The lease starts in October,
  so a 2026 cash budget would carry three months.
- **Angle plan choice.** Everyone is on the TRAD 1000/2000 where you left them — $30,485/yr
  against $24,498 on the HDHP 3400/5000. Block 3 of the Benefits tab prices all three.
- **401(k) is at zero.** Questco prices safe-harbor basic at about $26,300/yr, 3% non-elective at
  about $19,750.
- **Two errors in the CapFi / Questco cost model** are not reproduced here: its Cost by Tier
  enrolled count is hard-typed to 1 on the Family rows when two people hold Family, and its FICA
  figure exceeds 7.65% of the quoted payroll without capping Social Security at the wage base.

> Yellow = input · Green = from another tab · Black = formula · Grey = reference only.
