---
name: ep-ch063-demography-poverty-traps-and-unified-growth
description: Apply the principles of Chapter 63 of The Encyclopedia of Economic Principals (Demography, Poverty Traps, and Unified Growth) to the user's own numbers. Use when weighing the cost of more children against more investment per child, splitting income per head into productivity, employment and age structure, or checking whether a training program or a group of investments only pays once enough others join.
---

# Chapter 63: Demography, Poverty Traps, and Unified Growth

These principles show when family size, age structure or coordination holds income down, and what it would take to move it.

Notebook with the worked examples and figures: `../../notebooks/ch063-demography-poverty-traps-and-unified-growth.ipynb`

## 1. Quantity-quality tradeoff in children (quantity-quality-tradeoff-in-children)

When to use it: the cost of children depends on both their number and the investment each receives.

Equation as the chapter writes it:

    18(3)+3(20)+2(3)(20)=54+60+120=234.
    P_n=18+2(20)=58,

Ask the user for: cost coefficients a, b, d; number of children n; investment per child q; resources.

Steps:
1. Cost C = a n + b q + d n q (book: 18(2) + 3(50) + 2(2)(50) = 386, leaving 420 - 386 = 34).
2. Shadow price of a child P_n = a + d q (book: 18 + 2(50) = 118, up from 58 at q = 20).
3. Shadow price of quality P_q = b + d n (book: 3 + 2(3) = 9).
4. State which bundles are affordable and how the standard changes the price of another child.

Watch for: without a utility function the costs do not show which bundle is optimal.

## 2. Demographic dividend (demographic-dividend)

When to use it: income per head changes while the age structure is shifting.

Equation as the chapter writes it:

    \frac{Y}{N}=50(0.70)(0.45)=15.75.

Ask the user for: output per worker, employment rate, working-age share before and after.

Steps:
1. Y/N = (Y/E)(E/W)(W/N) (book: 50(0.70)(0.60) = 21, up one third from 15.75).
2. Recompute with the old share and the new other factors (book: 54(0.75)(0.45) = 18.225).
3. The difference is the age-share contribution (book: 24.30 - 18.225 = 6.075).

Watch for: the gain reverses when the large cohort retires; this is accounting, not a forecast.

## 3. Threshold-externality poverty trap (threshold-externality-poverty-trap)

When to use it: the return to an investment jumps once enough others make it.

Equation as the chapter writes it:

    R_0-c=7-10=-3
    R_1-c=15-10=5

Ask the user for: cost, low and high returns, the threshold, expected participation.

Steps:
1. Compare expected participation with the threshold (book: 47 is below 48).
2. Net per participant R - c (book: 7 - 10 = -3 below, 15 - 10 = 5 at or above).
3. Group payoff n (R - c) (book: 48(5) = 240; 47(-3) = -141).
4. State how many binding commitments are needed to cross the threshold.

Watch for: show the threshold is real before designing a program around it.

## 4. Big-push coordination failure (big-push-coordination-failure)

When to use it: each project's demand depends on how many complementary projects start.

Equation as the chapter writes it:

    \pi(m)=105+20m-150.

Ask the user for: base revenue, cost, spillover per other project, number of projects.

Steps:
1. Profit with m others pi(m) = base + spill m - cost (book: pi(0) = -45, pi(3) = 15).
2. Check each coalition size (book: pi(2) = -5, so three plants unravel).
3. State the smallest coalition with nonnegative profit and the subsidy a lone project would need.

Watch for: the spillover must be genuine new demand, not displaced purchases.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market or history.
