---
name: ep-ch098-austrian-institutional-and-evolutionary-political-economy
description: Apply the principles of Chapter 98 of The Encyclopedia of Economic Principals (Austrian, Institutional, and Evolutionary Political Economy) to the user's own numbers. Use when checking how a lower interest rate favors long projects, what an arbitrage opportunity earns before and after imitation, how much a price saves over an equal-assignment rule when costs are private, or who bears the first-round price effect of new money.
---

# Chapter 98: Austrian, Institutional, and Evolutionary Political Economy

These principles are mostly argued in words; the chapter's worked examples reduce them to discounting, spreads, merit order and first-round prices. The numbers are hypothetical.

Notebook with the worked examples and figures: `../../notebooks/ch098-austrian-institutional-and-evolutionary-political-economy.ipynb`

## 1. Austrian malinvestment cycle (austrian-malinvestment-cycle)

When to use it: seeing how credit terms change which projects look viable.

Inequality as the chapter writes it:

    i_m<R_j<i_n

Ask the user for: each project's cost, payoff and horizon, and the rates to compare.

Steps:
1. PV = payoff / (1 + r)^T (book: 112 / 1.10 = 101.82; 140 / 1.10^4 = 95.62).
2. Repeat at the lower rate (book: 105.66 and 110.89 at 6 percent).
3. Ask whether saving, not only credit, supports the projects started.

Watch for: a low rate backed by real saving does not create the same inconsistency.

## 2. Entrepreneurial discovery (entrepreneurial-discovery)

When to use it: valuing a newly noticed price gap and its erosion by imitation.

Equations as the chapter writes them:

    \pi=q(p-c)-f,
    800(0.95-0.40)-320=120

Ask the user for: quantity, buying and selling prices, fixed route cost.

Steps:
1. Spread q (p - c) (book: 800 x 0.80 = 640) and profit (640 - 400 = 240).
2. Gains to each side (book: growers 160 over disposal).
3. After imitation (book: 800 x 0.55 - 320 = 120).

Watch for: entry costs above expected profit stop discovery.

## 3. Dispersed-knowledge problem (dispersed-knowledge-problem)

When to use it: comparing a posted price with an assigned quota when costs are private.

Calculations as the chapter writes them:

    4(20)+2(50)=180
    2(20)+2(50)+2(90)=320

Ask the user for: each unit's cost and capacity, and the amount needed.

Steps:
1. Fill the need cheapest first (book: 4 from A, 2 from B, cost 180).
2. Cost of the rule (book: 2 each, cost 320).
3. The difference is the value of eliciting private costs (book: 140).

Watch for: with verified costs, an operator could assign the same cheap plan.

## 4. Cantillon effects (cantillon-effects)

When to use it: tracing whose prices move first when new money arrives.

Ask the user for: the fixed quantities and spending in each market, the injection and its first recipients.

Steps:
1. First-round price = (spending + injection) / quantity (book: land 11,000 / 100 = 110).
2. Or, if households receive it, food 11,000 / 1,000 = 11.
3. Nonrecipient loss = 1 - old price / new price (book: 9.1 percent).

Watch for: elastic supply absorbs part of each shock in quantities.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
