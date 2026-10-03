---
name: ep-ch089-norms-identity-social-interaction-and-multipliers
description: Apply the principles of Chapter 89 of The Encyclopedia of Economic Principals (Norms, Identity, Social Interaction, and Multipliers) to the user's own numbers. Use when estimating how peer feedback multiplies a program's direct effect, whether a participation cascade stalls or spreads, whether a few departures can tip a mixed neighborhood, or how expected ownership changes a status buyer's willingness to pay.
---

# Chapter 89: Norms, Identity, Social Interaction, and Multipliers

These principles show how other people's choices amplify, stall or reverse one's own. The chapter's numbers are hypothetical.

Notebook with the worked examples and figures: `../../notebooks/ch089-norms-identity-social-interaction-and-multipliers.ipynb`

## 1. Social multiplier (social-multiplier)

When to use it: scaling a direct program effect by peer feedback.

Equations as the chapter writes them:

    \frac{d\bar y}{dx}=\frac{\beta}{1-\gamma}, \qquad M_s=\frac{1}{1-\gamma}
    \frac{6}{1-0.4}=10

Ask the user for: the direct effect beta and the feedback coefficient gamma.

Steps:
1. Check gamma is below 1; otherwise the linear formula fails.
2. Total = beta / (1 - gamma) (book: 6 / 0.6 = 10; with gamma = -0.2, 6 / 1.2 = 5).
3. Feedback = total - beta (book: 4).

Watch for: capacity limits can shrink or reverse the peer response.

## 2. Threshold model of collective behavior (threshold-model-of-collective-behavior)

When to use it: predicting where a participation cascade stops.

Equations as the chapter writes them:

    (0,1,2,3,4,5,6,7,8,9)
    (0,1,2,4,4,5,6,7,8,9)

Ask the user for: each person's threshold (count of visible participants needed) and any visible seeds.

Steps:
1. Sort thresholds; add everyone whose threshold is at or below the visible count, repeat.
2. The cascade stops at the first gap (book: stalls at 3 with the changed list).
3. Add seeds to the visible count (book: one seed makes 3 + 1 = 4 and all 10 join).

Watch for: reversible choices and misreported counts change the outcome.

## 3. Schelling segregation tipping (schelling-segregation-tipping)

When to use it: checking whether a few departures set off a chain of exits.

Equations as the chapter writes them:

    s_A=\frac{47}{95}\approx49.5\%
    \frac{27}{75}=36\%

Ask the user for: group counts, each subgroup's minimum acceptable share and the initial exits.

Steps:
1. New share after exits, updating both numerator and denominator (book: 47 / 95 = 49.5%).
2. Remove every subgroup whose threshold is above the share and recompute (book: 27 / 75 = 36%).
3. Stop when no subgroup leaves (book: all A households leave; with a 45% threshold no one does).

Watch for: entry into vacancies and moving costs can halt the chain; stability is not welfare.

## 4. Snob effect (snob-effect)

When to use it: judging whether wider ownership loses a status buyer.

Equations as the chapter writes them:

    W=300-2N

Ask the user for: the willingness-to-pay rule, expected owners and price.

Steps:
1. W at the expected count (book: 300 - 80 = 220).
2. Surplus = W - price (book: 40 at $180; she buys).
3. Repeat with a higher count (book: N = 70 gives 160, below 180, so she declines).

Watch for: resale value and quality signals can move demand alongside exclusivity.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real household, group or place.
