---
name: ep-ch084-labor-supply-participation-and-household-insurance
description: Apply the principles of Chapter 84 of The Encyclopedia of Economic Principals (Labor Supply, Participation, and Household Insurance) to the user's own numbers. Use when deciding whether job search is worth its cost and how exits from search move the unemployment rate, tracing a parent's earnings loss to uncovered care hours, judging whether a fixed wage insures a worker, or reading sector pay averages when workers self-select.
---

# Chapter 84: Labor Supply, Participation, and Household Insurance

These principles turn participation, care and pay decisions into checkable comparisons. The chapter's numbers are hypothetical teaching values.

Notebook with the worked examples and figures: `../../notebooks/ch084-labor-supply-participation-and-household-insurance.ipynb`

## 1. Discouraged-worker effect (discouraged-worker-effect)

When to use it: deciding whether a jobless person keeps searching, and reading the unemployment rate when searchers quit.

Equations as the chapter writes them:

    pJ\geq k.
    u=\frac{U}{E+U}.

Ask the user for: perceived job-finding probability, the gain from an acceptable offer, search cost; employment and active unemployment.

Steps:
1. Expected gain pJ (book: 0.10 x 2,000 = 200).
2. Search if pJ >= k (book: 200 > 120; at p = 0.04, 80 < 120, search stops).
3. Rate before and after exits (book: 100 / 1,000 = 10 percent; 80 / 980 = 8.2 percent).

Watch for: a falling rate can mean exits from search, not hiring.

## 2. Child penalty (child-penalty)

When to use it: tracing a parent's earnings drop after a birth to uncovered care hours and who covers them.

Equations as the chapter writes them:

    t_m+t_f+t_{paid}\geq C.
    \frac{\$1{,}200-\$600}{\$1{,}200}=50\%.

Ask the user for: care need, help from relatives and formal care, each parent's hours and wage, how uncovered hours are split.

Steps:
1. Uncovered hours = need - relatives - formal (book: 50 - 10 - 20 = 20).
2. Subtract them from paid hours of whoever covers them (book: mother 40 - 20 = 20 hours, 600 dollars).
3. Penalty = lost earnings / earnings without the child (book: 600 / 1,200 = 50 percent; equal split 25 percent each).

Watch for: later wage losses from lost experience are a separate dynamic channel (book: 27 dollars an hour, 10 percent).

## 3. Implicit-contract smoothing (implicit-contract-smoothing)

When to use it: checking whether a stable wage acts as insurance and what it costs the firm.

Equations as the chapter writes them:

    w_s^{spot}=p_sF'(n_s).
    \frac{\sqrt{40}+\sqrt{16}}{2}\approx5.16.
    \sqrt{27}\approx5.20,

Ask the user for: revenue per worker in each state and its probability, the fixed wage, the worker's utility function.

Steps:
1. Expected utility of spot pay (book: (sqrt 40 + sqrt 16) / 2 = 5.16).
2. Utility of the fixed wage (book: sqrt 27 = 5.20, preferred).
3. Firm margins by state and on average (book: +13 and -11, average +1).

Watch for: in a deep slump the firm may keep the wage and cut employment instead.

## 4. Roy self-selection model (roy-self-selection-model)

When to use it: reading sector pay averages when people choose the sector that pays them most.

Equations as the chapter writes them:

    j_i^*=\arg\max_j\{p_jq_{ij}-c_{ij}\}.
    \frac{77+66+44}{3}\approx62.3,

Ask the user for: each person's potential pay in each sector and any entry costs.

Steps:
1. Each person's net payoff in each sector; pick the highest.
2. Observed mean pay per sector over those who chose it (book: coding 65, sales 60).
3. Recompute after a price change or new cost (book: +10 percent coding and Dev's 12 licence: coding mean 62.3).

Watch for: the cross-sector gap is not the gain any one person would get from switching.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market or person.
