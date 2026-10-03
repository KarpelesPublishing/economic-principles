---
name: ep-ch012-coordination-conflict-evolution-and-strategic-networks
description: Apply Chapter 12 of The Encyclopedia of Economic Principals (Coordination, Conflict, Evolution, and Strategic Networks) to the user's own numbers. Use when someone asks how confident they must be before joining a shared project, what mix of aggressive and passive behavior a population sustains, whether adding a road or link can slow a network, or how much selfish routing costs against an optimum.
---

# Chapter 12: Coordination, Conflict, Evolution, and Strategic Networks

When everyone's best move depends on the crowd, beliefs and the network's layout decide the outcome.

Notebook with the worked examples and figures: `../../notebooks/ch012-coordination-conflict-evolution-and-strategic-networks.ipynb`

## 1. Stag-hunt game (stag-hunt-game)

    12p - 2(1 - p) = 14p - 2,   14p - 2 >= 7 <=> p >= 9/14 approx 0.643.

Steps:
1. Expected payoff of the joint action R p + L(1 - p) (book: 7.8 at p = 0.70).
2. Threshold p* = (T - L) / (R - L) (book: 9/14; with a guarantee L = 0, 7/12).
3. Choose the joint action only above the threshold; report exact ties.

## 2. Evolutionarily stable strategy (evolutionarily-stable-strategy)

    U_H = x(-20) + (1 - x)60 = 60 - 80x,   U_D = (1 - x)30 = 30 - 30x.

Steps:
1. Hawk vs Hawk = (V - C) / 2 (book: -20).
2. If C > V, stable Hawk share x* = V / C (book: 0.60, payoff 12); otherwise all Hawk.

## 3. Braess paradox (braess-paradox)

    2,000/100 + 45 = 65 minutes,   4,000/100 + 4,000/100 = 80.

Steps:
1. Travel time without the new link (book: 65 minutes).
2. Equilibrium with the link: does everyone switch? (book: 80, a lone switcher would face 85).
3. Compare total time (book: 320,000 against 260,000 commuter-minutes).

## 4. Price of anarchy (price-of-anarchy)

    C(x) = x^2 + (1 - x),   C'(x) = 2x - 1,   PoA = 1/(3/4) = 4/3 approx 1.333.

Steps:
1. Equilibrium cost (book: all on A, 1).
2. Planner's cost from C'(x) = 0 (book: x = 1/2, cost 3/4).
3. PoA = equilibrium / optimum (book: 4/3).

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and multiple equilibria instead of forcing one outcome.
- Do not present the book's hypothetical numbers as facts about real networks or populations.
