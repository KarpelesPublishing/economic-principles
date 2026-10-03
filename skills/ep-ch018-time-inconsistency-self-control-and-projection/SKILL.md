---
name: ep-ch018-time-inconsistency-self-control-and-projection
description: Apply the principles of Chapter 18 of The Encyclopedia of Economic Principals (Time Inconsistency, Self-Control, and Projection) to the user's own numbers. Use when a plan to wait reverses once a reward becomes immediate, when a calm-state forecast underestimates a later craving, when removing a tempting option might be worth paying for, or when a purchase is made in a temporary state such as hunger.
---

# Chapter 18: Time Inconsistency, Self-Control, and Projection

These principles let the user price a commitment device, measure the cost of a cold-state forecast error, value a smaller menu, and correct an order placed in a passing state.

Notebook with the worked examples and figures: `../../notebooks/ch018-time-inconsistency-self-control-and-projection.ipynb`

## 1. Present bias (present-bias)

When to use it: a person plans to wait for a larger later reward but takes the smaller one once it is immediate.

Equations as the chapter writes them:

    V_{50}=0.70(0.98)(50)=34.30
    V_{60}=0.70(0.98)^2(60)=40.3368.
    0.70(0.98)(60)=41.16.

Ask the user for: the two amounts, their delays, beta and delta.

Steps:
1. Value both rewards in advance: beta x delta^t x amount (book: 0.70 x 0.98 x 50 = 34.30 and 0.70 x 0.9604 x 60 = 40.3368).
2. Value them on the day: the sooner reward at face, the later at beta x delta x amount (book: 50 against 41.16).
3. If the ranking flips, the commitment device is worth at most the advance gap (book: 40.3368 - 34.30 = 6.0368). With no reversal (beta = 1) commitment is worth nothing. Name near ties (an added comparison: beta = 0.85 gives 49.98 against 50).

Watch for: the commitment value treats the earlier self's evaluation as the welfare benchmark.

## 2. Hot-cold empathy gap (hot-cold-empathy-gap)

When to use it: an advance decision is made in a cold state about a hot-state need.

Equations as the chapter writes them:

    20-15=5.
    20-6=14.
    14-5=9.

Ask the user for: the forecast value, the actual later value, the advance cost and the later spot price.

Steps:
1. The plan acts in advance only if the forecast exceeds the advance cost (book: 5 < 6, so nothing is packed).
2. Realized surplus is the best action left later (book: 20 - 15 = 5).
3. Best surplus under an accurate forecast (book: 20 - 6 = 14); the error cost is the difference (book: 14 - 5 = 9).

Watch for: the later value must not depend on the plan itself.

## 3. Temptation and self-control preferences (temptation-and-self-control-preferences)

When to use it: deciding whether removing an option is worth paying for even if it would not be chosen.

Equation as the chapter writes it:

    W(A)=\max_{x\in A}\{u(x)+v(x)\}-\max_{y\in A}v(y).

Ask the user for: normative value u and temptation v of each option.

Steps:
1. The chosen item maximizes u + v (book: fruit 10, cake 4 + 5 = 9, so fruit).
2. Welfare subtracts the strongest temptation (book: 10 - 5 = 5, against 10 for the fruit-only menu).
3. If temptation rises past the gap, the person yields (book: v(c) = 8 gives 12 - 8 = 4).

Watch for: a restricted choice made for other reasons (allergy, missing information) does not reveal temptation.

## 4. Projection bias (projection-bias)

When to use it: a purchase for later is made in a temporary state.

Equation as the chapter writes it:

    \widehat u=(1-0.50)(2)+0.50(8)=5.

Ask the user for: the true later value, the current value and the projection weight alpha.

Steps:
1. Predicted value = (1 - alpha) x true + alpha x current (book: 0.5 x 2 + 0.5 x 8 = 5).
2. Order if the prediction exceeds the price (book: 5 > 4, two desserts).
3. Realized gain = quantity x (true value - price) (book: 2(2) - 2(4) = -4).

Watch for: a single alpha is a simplification; cheap cancellation is the practical fix.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
