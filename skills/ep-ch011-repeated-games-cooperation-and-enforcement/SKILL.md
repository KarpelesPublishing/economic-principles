---
name: ep-ch011-repeated-games-cooperation-and-enforcement
description: Apply Chapter 11 of The Encyclopedia of Economic Principals (Repeated Games, Cooperation, and Enforcement) to the user's own payoffs. Use when someone sizes a penalty that ends a prisoners dilemma, asks how often a shared task nobody owns gets done, compares a fixed-term relationship with an open-ended one, or works out how long a punishment must last to deter defection.
---

# Chapter 11: Repeated Games, Cooperation, and Enforcement

Cooperation lasts when the future it protects is worth more than one defection.

Notebook with the worked examples and figures: `../../notebooks/ch011-repeated-games-cooperation-and-enforcement.ipynb`

## 1. Prisoner's dilemma (prisoners-dilemma)

    T = 8 > R = 6 > P = 3 > S = 1,   6 > 5 and 1 > 0.

Steps:
1. Compare defecting with cooperating against each rival action (book: 8 > 6 and 3 > 1, defect dominates).
2. A charge f on defection flips both comparisons when f exceeds T - R and P - S (book: f = 3 gives 6 > 5 and 1 > 0).
3. At the exact boundary report the tie (constructed check: f = 2 leaves every profile an equilibrium).

## 2. Volunteer's dilemma (volunteers-dilemma)

    p* = 1 - (30/120)^(1/3) = 1 - 0.25^(1/3) approx 0.370,   (1 - p*)^4 approx 0.630^4 approx 0.157

Steps:
1. p* = 1 - (C/B)^(1/(n - 1)) (book: 0.370).
2. Failure (1 - p*)^n (book: 0.157; with C = 7.5, 0.025).
3. Larger groups fail more often; cut C or name one person.

## 3. Finite-horizon unraveling (finite-horizon-unraveling)

    V_C = 4/(1 - 0.8) = 20.   V_D = 6 + 0.8(1)/(1 - 0.8) = 10.

Steps:
1. Known last round: defect there, then in every earlier round (book: 1 + 1 + 1 = 3 against 12).
2. Random end with continuation q: compare V_C and V_D (book: 20 against 10).
3. Threshold q = (T - R) / (T - P) (book: 0.4).

## 4. Trigger-strategy enforcement (trigger-strategy-enforcement-in-repeated-games)

    delta >= (10 - 6)/(10 - 2) = 0.5,   V_C = 6/(1 - 0.75) = 24

Steps:
1. V_C = R / (1 - delta).
2. V_D with a k-period punishment = T + P(delta + ... + delta^k) + delta^(k+1) V_C (book: two months 22.75, one month 25).
3. Deterred when V_C >= V_D; report exact ties.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which payoffs are the user's and which are assumptions you added.
- Name ties and indifference instead of forcing a verdict.
- Do not present the book's hypothetical payoffs as facts about real firms.
