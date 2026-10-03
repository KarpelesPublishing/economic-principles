---
name: ep-ch064-institutions-state-formation-and-long-run-development
description: Apply the principles of Chapter 64 of The Encyclopedia of Economic Principals (Institutions, State Formation, and Long-Run Development) to the user's own numbers. Use when judging whether a collective boycott can deter confiscation, whether taxes can carry war or emergency debt, how a persistent growth gap can reverse an income lead, or how fast a latecomer can catch up and whether an adoption package pays.
---

# Chapter 64: Institutions, State Formation, and Long-Run Development

These principles turn institutional stories into checkable payoffs: commitment values, debt paths, compounding growth and catch-up arithmetic. The chapter's numbers are constructed teaching numbers, not historical data.

Notebook with the worked examples and figures: `../../notebooks/ch064-institutions-state-formation-and-long-run-development.ipynb`

## 1. Merchant-guild commitment mechanism (merchant-guild-commitment-mechanism)

When to use it: deciding whether a collective sanction makes a powerful party keep its promise.

Equations as the chapter writes them:

    V_H=\frac{24-6}{1-0.75}=72
    V_P(m)=55+72(1-m)
    m\geq\frac{55}{72}\approx0.764

Ask the user for: yearly revenue from cooperation, its cost, the discount factor, the one-time gain from defecting, and the share of future business the sanction removes.

Steps:
1. Cooperate value V_H = (revenue - cost) / (1 - delta) (book: 18 / 0.25 = 72).
2. Defect value V_P = gain + (1 - m) V_H (book, m = 0.25: 55 + 72 x 0.75 = 109).
3. Threshold m* = gain / V_H (book: 55 / 72 = 0.764). The sanction deters only if m is at least m*. If m* exceeds 1 (an impatient ruler, for example delta = 0.60 gives 55 / 45 = 1.222), no sanction can deter.

Watch for: the sanction must also be enforced on the members themselves (book: 3 / 0.25 = 12 > 9).

## 2. Fiscal-military state (fiscal-military-state)

When to use it: checking how much a state must borrow in a high-spending year and whether later surpluses repay it.

Equations as the chapter writes them:

    D_{t+1}=1.05(240)+60+90-120=282
    D_{t+2}=1.05(282)+60+35-120=271.10

Ask the user for: starting debt, interest rate, civilian and emergency spending, tax revenue.

Steps:
1. D_t+1 = (1 + r) D_t + G + M - T (book: 252 + 150 - 120 = 282; borrowing 42).
2. Repeat for the next year with the new spending (book: 296.10 + 95 - 120 = 271.10).
3. Compare the primary surplus with interest (book: 25 against 14.10, debt falls 10.90).

Watch for: the model ignores maturity, inflation and collection cost.

## 3. Reversal of fortune (reversal-of-fortune)

When to use it: asking whether a persistent growth gap can overturn an initial income lead, and when.

Equations as the chapter writes them:

    J=1-0.60P
    g=0.008+0.025J

Ask the user for: two starting incomes, two growth rates (or the indices that set them), a horizon.

Steps:
1. Growth rates (book: 0.008 + 0.025 x 0.46 = 0.0195 and 0.008 + 0.025 x 0.82 = 0.0285).
2. Compound: Y = Y0 (1 + g)^T (book: 150 x 1.0195^60 = 477.89; 100 x 1.0285^60 = 539.83).
3. Ratio and crossover (book: 0.8853, so A ends about 11.5 percent poorer; still ahead at 40 years).

Watch for: the indices and equations are invented; they estimate nothing about real colonies.

## 4. Advantage of backwardness (advantage-of-backwardness)

When to use it: estimating catch-up growth from a productivity gap and testing an adoption package.

Equations as the chapter writes them:

    A_1=35+0.25(100-35)=51.25
    PV=20\left(\frac{1-(1.08)^{-5}}{0.08}\right)\approx79.85

Ask the user for: frontier and starting productivity, the share of the gap closed, and the package's cost, yearly benefit, life and discount rate.

Steps:
1. A_1 = A_0 + theta (A* - A_0) (book: 35 + 0.25 x 65 = 51.25).
2. Growth = A_1 / A_0 - 1 (book: 46.43 percent; from 75 only 8.33 percent).
3. NPV = benefit x annuity factor - cost (book: 79.85 - 72 = 7.85).

Watch for: the catch-up share depends on institutions that can finance and absorb adoption; financing a package is not proof it is efficient.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market or historical case.
