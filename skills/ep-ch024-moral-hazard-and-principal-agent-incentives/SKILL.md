---
name: ep-ch024-moral-hazard-and-principal-agent-incentives
description: Apply the principles of Chapter 24 of The Encyclopedia of Economic Principals (Moral Hazard and Principal-Agent Incentives) to the user's own numbers. Use when splitting revenue between partners whose efforts are hidden, pricing a bonus under a wage floor, sizing an insurance deductible so the insured still takes care, or designing a base plus bonus contract that induces effort and is accepted.
---

# Chapter 24: Moral Hazard and Principal-Agent Incentives

These principles tell the user what pay or coverage scheme gets hidden effort supplied, and what it costs.

Notebook with the worked examples and figures: `../../notebooks/ch024-moral-hazard-and-principal-agent-incentives.ipynb`

## 1. Double moral hazard (double-moral-hazard)

When to use it: two parties share revenue and both contribute effort nobody can verify.

Equations as the chapter writes them:

    R(e,m)=40e+40m
    30=20e,  10=20m
    10(1.5^2+0.5^2)=25

Ask the user for: marginal revenue of each effort, each effort's cost curve, the share alpha.

Steps:
1. Each party sets its share of marginal revenue equal to its marginal cost (book: 0.75 x 40 = 20e gives e = 1.5; 0.25 x 40 = 20m gives m = 0.5).
2. Compute revenue, cost and surplus (book: 80 - 25 = 55).
3. Compare with the efficient efforts and with other shares (book: an even split gives 60; efficient 80).

Watch for: no linear split reaches the efficient surplus; that needs verifiable effort.

## 2. Limited-liability information rents (limited-liability-information-rents)

When to use it: a bonus must induce effort but the agent cannot be charged on failure.

Equations as the chapter writes them:

    (0.70-0.30)w_H >= 12
    0.70(21)+0.30(-9)=$12

Ask the user for: effort cost, success probability with and without effort, value of success, the wage floor.

Steps:
1. Spread = cost / (p1 - p0) (book: 12 / 0.40 = 30).
2. With a zero floor, w_H = spread and the expected wage is p1 x w_H (book: 0.70 x 30 = 21).
3. Rent = expected wage - cost (book: 21 - 12 = 9); company keeps p1 x value - wage (book: 70 - 21 = 49).

Watch for: at the minimal bonus the agent is indifferent; the chapter breaks the tie toward high effort.

## 3. Moral hazard (moral-hazard)

When to use it: insurance blunts the incentive to take care.

Equations as the chapter writes them:

    (0.10-0.02)($2,000)=$160
    $80+0.02($2,000)=$120
    (0.10-0.02)($1,500)=$120

Ask the user for: care cost, accident probabilities with and without care, loss, deductible.

Steps:
1. Private saving = (p0 - p1) x deductible (book: 0.08 x 1,500 = 120).
2. Care is taken when saving exceeds care cost (book: 120 > 80).
3. Smallest deductible restoring care = care cost / (p0 - p1) (book: 80 / 0.08 = 1,000, an exact tie).

Watch for: a larger deductible restores care but shifts more risk onto the insured.

## 4. Principal-agent problem (principal-agent)

When to use it: designing base plus bonus pay for an agent whose effort is hidden.

Equations as the chapter writes them:

    $15,000+0.20($22,000)=$19,400
    0.50($100,000)-$26,000=$24,000

Ask the user for: outside option, effort cost, success probabilities, value of success, base and bonus.

Steps:
1. Low effort pay = base + p0 x bonus (book: 15,000 + 0.20 x 22,000 = 19,400).
2. High effort net = base + p1 x bonus - cost (book: 15,000 + 11,000 - 6,000 = 20,000).
3. Check the higher net clears the outside option, then profit = p x value - expected pay (book: 50,000 - 26,000 = 24,000).

Watch for: risk aversion and noise add an insurance cost the book example leaves out.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
