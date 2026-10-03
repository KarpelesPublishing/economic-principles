---
name: ep-ch051-banks-monitoring-lending-and-credit-creation
description: Apply the principles of Chapter 51 of The Encyclopedia of Economic Principals (Banks, Monitoring, Lending, and Credit Creation) to the user's own numbers. Use when comparing direct and bank monitoring costs, judging whether a bank's franchise value keeps it safe, pricing a loan with private information about the borrower, or weighing runnable deposit funding against panic risk.
---

# Chapter 51: Banks, Monitoring, Lending, and Credit Creation

These principles let the user decide when a bank lowers the cost of finance, when its owners prefer safety, what an informed lender can charge, and how much run risk deposit funding can bear.

Notebook with the worked examples and figures: `../../notebooks/ch051-banks-monitoring-lending-and-credit-creation.ipynb`

## 1. Delegated monitoring (delegated-monitoring)

When to use it: comparing every investor checking every borrower with one intermediary that monitors and can itself default.

Equation as the chapter writes it:

    \Pr(F\geq3)=1-\sum_{j=0}^{2}\binom{10}{j}(0.1)^j(0.9)^{10-j}\approx0.0701908.

Ask the user for: number of savers and loans, cost per check, loan payoffs in good and bad states, failure probability, the promise to depositors, the cost of a bank default, and whether loan outcomes are independent.

Steps:
1. Direct cost = savers x loans x check cost (book: 100 x 10 x 4,000 = 4,000,000).
2. Find the number of failures at which pool receipts fall below the promise, and its probability (book: F >= 3, 0.0701908).
3. Delegated cost = loans x check cost + Pr(default) x default cost (book: 40,000 + 0.070190826 x 40,000,000 = 40,000 + 2,807,633 = 2,847,633).
4. Compare; redo with perfectly correlated loans (book: 0.1 x 40,000,000 + 40,000 = 4,040,000, the bank loses).

Watch for: the advantage rests on independent loan outcomes.

## 2. Charter-value discipline (charter-value-discipline)

When to use it: deciding whether future rents keep a bank's owners away from a risky portfolio.

Equation as the chapter writes it:

    8+0.98V=11+0.80V.

Ask the user for: each portfolio's payoff now and survival probability, and the charter value V.

Steps:
1. Owner value = payoff now + survival probability x V (book: 8 + 0.98 x 30 = 37.4; 11 + 0.80 x 30 = 35).
2. Pick the larger; name a tie.
3. Threshold V* = payoff gap / survival gap (book: 3 / 0.18 = 16.67).

Watch for: risk-neutral owners and a charter lost in full on failure.

## 3. Relationship lending (relationship-lending)

When to use it: judging whether a lender with private information about a borrower should lend, and at what promise.

Equation as the chapter writes it:

    0.90P^*+0.10(40{,}000)=100{,}000.

Ask the user for: principal, promised repayment, collateral recovery and the lender's success probability.

Steps:
1. Expected repayment = p x promise + (1 - p) x collateral (book: 0.90 x 110,000 + 0.10 x 40,000 = 103,000; outsider 92,500).
2. Lend if it covers the principal.
3. Break-even promise P* = (principal - (1 - p) x collateral) / p (book: 106,666.67, a 6.67 percent rate).

Watch for: the informed lender can charge above P* when outsiders cannot compete.

## 4. Diamond-Rajan liquidity-creation fragility (diamond-rajan-liquidity-creation-fragility)

When to use it: weighing the funding capacity of demandable deposits against the cost of a panic sale.

Equations as the chapter writes them:

    (1-s)(30)+s(-18)=30-48s.
    s<\frac{30}{48}=0.625.

Ask the user for: collection value C, outsider recovery share beta, project cost and the panic probability s.

Steps:
1. Outsider value beta C (book: 0.60 x 120 = 72).
2. Completion net = C - cost (30); panic net = beta C - cost (-18).
3. Expected surplus = (1 - s) x completion + s x panic (book: at s = 0.3, 21 - 5.4 = 15.6).
4. Threshold s* = completion / (C - beta C) (book: 30 / 48 = 0.625).

Watch for: a stylized one-loan bank; the panic probability is an assumption, the book leaves it symbolic.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
