---
name: ep-ch010-dynamic-and-sequential-games
description: Apply Chapter 10 of The Encyclopedia of Economic Principals (Dynamic and Sequential Games) to the user's own payoffs. Use when someone asks whether a rival's threat is credible, how patient firms must be to sustain cooperation under grim trigger, whether to enter against an incumbent of unknown type, or how long and costly a war of attrition will be.
---

# Chapter 10: Dynamic and Sequential Games

Solve from the last move back, and test every threat at the moment it would be carried out.

Notebook with the worked examples and figures: `../../notebooks/ch010-dynamic-and-sequential-games.ipynb`

## 1. Backward induction (backward-induction)

    2 > -1,   3 > 0.   -1 > -3,   0 > -2.

Steps:
1. At each last node, pick the mover's best payoff (book: incumbent 2 > -1, accommodates).
2. Replace the node by that outcome and move back (book: entrant 3 > 0, enters; outcome (3, 2)).
3. A threat is credible only if it is the best choice at its node (book: with Accommodate -3, Fight is credible).

## 2. One-shot deviation principle (one-shot-deviation-principle)

    V_C = 8/(1 - 0.7) = 26.667.   V_D = 12 + 0.7 x 5/(1 - 0.7) = 23.667.

Steps:
1. V_C = R / (1 - delta), V_D = T + delta P / (1 - delta) (book: 26.667 and 23.667).
2. Threshold delta = (T - R) / (T - P) (book: 4/7 = 0.571).
3. Check the punishment state too (book: 16.667 against 13.667).

## 3. Sequential equilibrium (sequential-equilibrium)

    0.30(-1) + 0.70(3) = -0.30 + 2.10 = 1.80 > 0.

Steps:
1. Find each type's optimal action after entry (book: Strong fights, Weak accommodates).
2. Weight the entrant's payoffs by the prior (book: 1.80 at q = 0.30; -0.20 at 0.80).
3. Break-even prior where the expectation is 0 (book: 0.75); report exact ties.

## 4. War-of-attrition game (war-of-attrition-game)

    h = c/V = 3/120 = 0.025 per week.   1/(2h) = 1/0.05 = 20 weeks.

Steps:
1. Hazard h = c / V; expected duration 1 / (2h) (book: 20 weeks).
2. Expected combined cost 2c x duration = V (book: 120).
3. A deadline T caps spending at 2cT (book: 60).

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which payoffs are the user's and which are assumptions you added.
- Name ties and indifference instead of forcing a choice.
- Do not present the book's hypothetical payoffs as facts about real firms.
