---
name: ep-ch075-institutional-persistence-path-dependence-and-evolution
description: Apply Chapter 75 of The Encyclopedia of Economic Principals (Institutional Persistence, Path Dependence, and Evolution) to the user's own numbers. Use when someone wants to split a productivity gain into firms improving versus market share shifting, price how much legitimacy saves on enforcement, decide whether a better system is worth its conversion cost over a given horizon, or judge whether a broken allocation rule will trigger collective action.
---

# Chapter 75: Institutional Persistence, Path Dependence, and Evolution

Separate search from selection, value legitimacy in enforcement dollars, test lock-in against the decision horizon, and check whether a grievance crosses a mobilization threshold.

Notebook with the worked examples and figures: `../../notebooks/ch075-institutional-persistence-path-dependence-and-evolution.ipynb`

## 1. Evolutionary routines (evolutionary-routines)

When to use it: an industry average improved and the user wants to know how much came from new routines versus reallocation.

    A_bar = sum(w_i A_i) / sum(w_i)

Ask for: productivity of each routine, how many firms use it before and after search, and market weights after selection.

Steps:
1. Initial average with equal shares (book: (9 x 9 + 3 x 13) / 12 = 10).
2. Average after search, still equal shares (book: (7 x 9 + 4 x 13 + 1 x 7) / 12 = 122 / 12 = 10.17).
3. Average after selection with weights (book: N weight 2, D exits: (7 x 9 + 8 x 13) / 15 = 167 / 15 = 11.13).
4. Search gain = step 2 minus step 1; selection gain = step 3 minus step 2 (book: 0.1667 and 0.9667).

Watch for: failed experiments (the defective variant) lower the post-search average; do not count all search as improvement.

## 2. Legitimacy as political capital (legitimacy-as-capital)

When to use it: comparing enforcement budgets across authorities, or judging a reform meant to raise accepted authority.

    c = 0.42 + 0.025L + 0.06e

Ask for: required compliance, a compliance rule (or use the chapter's, and say so), the legitimacy stock, and the cost per effort unit.

Steps:
1. Effort e = (target - base - slope_L x L) / slope_e (book: (0.84 - 0.42 - 0.025 x 2) / 0.06 = 6.17).
2. Cost = e x cost per unit (book: 0.37 x 90,000 / 0.06 = $555,000).
3. Repeat at the post-reform L (book L = 6: 4.5 units, $405,000), saving $150,000 a year.
4. Net of reform over its life (book: 3 x $150,000 - $180,000 = $270,000).

Watch for: if the reform raises compliance through material incentives, the saving is not all legitimacy.

## 3. Path dependence and institutional lock-in (path-dependence-institutional-lock-in)

When to use it: a better system exists but switching has a one-time cost.

    PV_T = gain x (1 - (1 + r)^-T) / r

Ask for: annual gain, conversion cost, discount rate, and the decision maker's horizon.

Steps:
1. Annual gain (book: 18,000 x (11 - 7) + (90,000 - 55,000) = $107,000).
2. PV over the horizon (book T = 3: $291,388; T = 4: $379,417).
3. Switch when PV exceeds the conversion cost (book: $291,388 < $320,000, retain; with a standard cutting cost to $180,000, PV_2 = $198,957 is enough).

Watch for: a subsidy that only reimburses the cost changes the agency's threshold but not the social conversion cost.

## 4. Moral economy (moral-economy)

When to use it: predicting protest over a scarce good, and how the seller will respond.

    willing > threshold;  expected defiance cost = p x disruption cost + reputation loss

Ask for: how many are willing to act, the coordination threshold, disruption cost and probability, reputational loss, and the cost of conceding.

Steps:
1. Compare willing with threshold (book: 45 > 36 under secret diversion; 22 and 25 do not mobilize).
2. Expected defiance cost (book: 0.60 x $3,200 + $500 = $2,420).
3. Concede when concession costs less (book: $900 < $2,420).

Watch for: willingness counts are the chapter's assumptions; real thresholds must be estimated.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real institution.
