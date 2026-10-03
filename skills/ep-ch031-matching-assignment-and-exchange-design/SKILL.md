---
name: ep-ch031-matching-assignment-and-exchange-design
description: Apply the principles of Chapter 31 of The Encyclopedia of Economic Principals (Matching, Assignment, and Exchange Design) to the user's own numbers. Use when weighing early offers against waiting for information, deciding how to rank schools under a Boston-style mechanism, judging whether a common market date pays, or diagnosing application congestion against review capacity.
---

# Chapter 31: Matching, Assignment, and Exchange Design

These principles show how timing, market thickness, rules and capacity decide which matches a market can find.

Notebook with the worked examples and figures: `../../notebooks/ch031-matching-assignment-and-exchange-design.ipynb`

## 1. Market unraveling (market-unraveling)

When to use it: deciding whether to sign before match quality is known.

Equations as the chapter writes them:

    110+110=220.
    82.5+82.5=165.
    220-165=55

Ask the user for: match values in each information state, their probabilities, and the total cost of waiting.

Steps:
1. Surplus when waiting picks the best pairs (book: 110 + 110 = 220).
2. Expected surplus of early pairs (book: (110 + 55)/2 = 82.5 each, 165 total).
3. Compare 220 - waiting cost with 165 (book: cost 70 gives 150 < 165, so early wins; breakeven 55).

Watch for: reversible early offers remove the loss.

## 2. Boston-mechanism priority loss (boston-mechanism-priority-loss)

When to use it: ranking choices under a mechanism that fills seats in round one.

Equations as the chapter writes them:

    (1-0.40)(120)+0.40(0)=72.
    (1-0.20)(120)=96,

Ask the user for: values of the favorite and the safe option, and the chance a higher-priority rival takes the favorite.

Steps:
1. Value of listing the favorite first: (1 - q) x favorite (book: 0.6 x 120 = 72).
2. Value of listing the safe option first (book: 85).
3. Pick the larger; indifference at q = 1 - safe/favorite (book: 0.292).

Watch for: under deferred acceptance honest ranking is safe, so no calculation is needed.

## 3. Market thickness (market-thickness)

When to use it: deciding whether to bring all participants to one market date.

Equations as the chapter writes them:

    110+95=205.
    65+75=140
    205-4(18)=133,

Ask the user for: pair values and the waiting cost per participant.

Steps:
1. Best pooled assignment (book: 110 + 95 = 205).
2. Fragmented assignment (book: 65 + 75 = 140).
3. Subtract waiting costs from pooling and compare (book: 205 - 4(18) = 133 < 140; breakeven 65/4 = 16.25).

Watch for: if all pairs are worth the same (book: 80), pooling adds nothing.

## 4. Market congestion (market-congestion)

When to use it: many applications chasing limited review capacity.

Equation as the chapter writes it:

    120(12)=1{,}440,\qquad m_j=\frac{1{,}440}{12}=120.

Ask the user for: number of applicants, applications each, number of reviewers, capacity each, suitable targets per applicant.

Steps:
1. Load per reviewer (book: 1,440/12 = 120).
2. Review probability rho = capacity/load, capped at 1 (book: 40/120).
3. Chance at least one suitable application is read: 1 - (1 - rho)^s (book: 1 - (80/120)^2 = 55.56%).

Watch for: once load is within capacity, capping applications only reduces discovery.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
