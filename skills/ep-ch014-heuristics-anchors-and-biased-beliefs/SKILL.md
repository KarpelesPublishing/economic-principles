---
name: ep-ch014-heuristics-anchors-and-biased-beliefs
description: Apply Chapter 14 of The Encyclopedia of Economic Principals (Heuristics, Anchors, and Biased Beliefs) to the user's own numbers. Use when someone judges a candidate or case by how typical it looks, values something after seeing an asking price, finds a group more divided after reviewing the same evidence, or forecasts a compounding balance or debt.
---

# Chapter 14: Heuristics, Anchors, and Biased Beliefs

Put back what a shortcut leaves out: the base rate, the anchor weight, the weight on unwelcome evidence and the compounding.

Notebook with the worked examples and figures: `../../notebooks/ch014-heuristics-anchors-and-biased-beliefs.ipynb`

## 1. Representativeness heuristic (representativeness-heuristic)

When to use it: a profile, label or test result "looks like" a winner and the user is about to act on it.

Equation as the chapter writes it:

    P(H|E) = P(E|H)P(H) / [P(E|H)P(H) + P(E|not H)P(not H)]

Ask the user for: the base rate, how often the signal appears among true cases and among the rest, the payoff from a true case and the cost of acting.

Steps:
1. Numerator and denominator (book: 0.80 x 0.10 = 0.08; 0.08 + 0.30 x 0.90 = 0.35).
2. Posterior (book: 0.08 / 0.35 = 0.228571; the book rounds it to 0.229).
3. Expected net value (book: 150,000 x 0.08 / 0.35 - 50,000 = -15,714.29; the book prints -15,650 from the rounded posterior).
4. Compare with the value if the likelihood is used as the posterior (book: 0.80 x 150,000 - 50,000 = 70,000), and state the break-even probability cost / value (book: 0.3333).

Watch for: graded scores and partial value from other hires change the payoffs.

## 2. Anchoring and insufficient adjustment (anchoring-and-insufficient-adjustment)

When to use it: a valuation or offer was formed after seeing an asking price or another arbitrary number.

Equation as the chapter writes it:

    J = (1 - lambda) m(I) + lambda a,   0 < lambda < 1

Ask the user for: their evidence-based estimate m(I), the anchor a, and a guess of the residual weight lambda (say it is an assumption).

Steps:
1. Judgment after each anchor (book: 0.75 x 24,000 + 0.25 x 32,000 = 26,000 and 0.75 x 24,000 + 0.25 x 20,000 = 23,000).
2. Gap = lambda x (a_H - a_L) (book: 0.25 x 12,000 = 3,000).
3. Bids (book: 0.95 x 26,000 = 24,700 and 0.95 x 23,000 = 21,850); with lambda = 0 both are 22,800.

Watch for: an implausibly extreme anchor may get no weight, so lambda is not one fixed number.

## 3. Confirmation bias (confirmation-bias)

When to use it: two parties saw the same evidence and grew further apart.

Equation as the chapter writes it:

    log O_{t+1} = log O_t + w(s_t, p_t) log LR(s_t)

Ask the user for: each party's prior, the likelihood ratio of each signal, and the weights on confirming and contradicting evidence.

Steps:
1. Final odds (book: Ava 3 x 3 x (1/3)^0.5 = 5.1962; Ben (1/3) x (1/3) x 3^0.5 = 0.1925).
2. Posteriors odds / (1 + odds) (book: 0.8386 and 0.1614).
3. Gap after against gap before (book: 0.6772 against 0.50; the book says about 0.678, the difference of its rounded posteriors). With equal weights the signals cancel.

Watch for: the initial disagreement remains even when the weights are equal.

## 4. Exponential-growth bias (exponential-growth-bias)

When to use it: forecasting a saving balance, a debt or any proportional growth over many periods.

Equations as the chapter writes them:

    B_T = P(1 + r)^T,   B~_T = P(1 + rT)

Ask the user for: principal, rate per period, number of periods, and any threshold the decision depends on.

Steps:
1. Linear forecast (book: 10,000 + 30 x 700 = 31,000).
2. Compound balance (book: 10,000 x 1.07^30 = 76,123).
3. Compare both with the threshold (book: 60,000: linear rejects, compound accepts).

Watch for: payments, withdrawals, fees and changing rates need a cash-flow schedule, not the one-deposit formula.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
