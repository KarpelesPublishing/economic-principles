---
name: ep-ch056-comparative-advantage-factor-endowments-and-distribution
description: Apply the principles of Chapter 56 of The Encyclopedia of Economic Principals (Comparative Advantage, Factor Endowments, and Distribution) to the user's own numbers. Use when a goods price change must be traced into wages and rentals, when a factor endowment grows at fixed prices, when mobile workers and sector-specific owners gain or lose from a price change, or when trade may equalize factor prices across countries.
---

# Chapter 56: Comparative Advantage, Factor Endowments, and Distribution

These principles let the user see how trade prices and endowments move factor rewards and outputs, and who wins and who loses.

Notebook with the worked examples and figures: `../../notebooks/ch056-comparative-advantage-factor-endowments-and-distribution.ipynb`

## 1. Stolper-Samuelson theorem (stolper-samuelson-theorem)

When to use it: a goods price changes and the user wants the effect on wages and rentals.

Equation as the chapter writes it:

    2w+r=36,\qquad w+2r=30.

Ask the user for: labor and capital per unit of each good, and both goods prices.

Steps:
1. Write price = unit cost for each good (book: 2w + r = 36, w + 2r = 30).
2. Solve the pair (book: 3r = 2 x 30 - 36 = 24, r = 8, w = 14).
3. Compare percent changes with the price change (book: wage +40 percent against cloth +20 percent) and real rewards in each good (book: 14 / 36 = 0.389, 14 / 30 = 0.467).

Watch for: the result needs both goods to be produced; otherwise one equation stops binding.

## 2. Rybczynski theorem (rybczynski-theorem)

When to use it: one factor's endowment grows while goods prices stay fixed.

Equation as the chapter writes it:

    2X+Y=360,\qquad X+2Y=300.

Ask the user for: factor requirements per unit and the two endowments.

Steps:
1. Write full employment for each factor (book: 2X + Y = 360, X + 2Y = 300).
2. Solve (book: 3X = 2 x 360 - 300 = 420, X = 140, Y = 80).
3. Compare with the baseline (book: cloth +40 percent, machines -20 percent, labor +20 percent).

Watch for: a negative solved output means the economy specializes and the formula no longer applies.

## 3. Specific-factors distribution effect (specific-factors-distribution-effect)

When to use it: labor is mobile but each sector has a fixed factor, and one price changes.

Equation as the chapter writes it:

    \frac{7.5}{\sqrt{L_X}}=\frac{5}{\sqrt{L_M}},\qquad L_X+L_M=100.

Ask the user for: workers, prices and the output function of each sector.

Steps:
1. Equate the value of marginal products (book: L_X = 2.25 L_M, so L_M = 30.77, L_X = 69.23).
2. Compute the wage (book: 5 / sqrt(30.77) = 0.9014, +27.5 percent) and the wage in each good (book: 0.9014 / 1.5 = 0.6009, -15.0 percent).
3. Compute each rent (book: R_X = 1.5 x 5 x sqrt(69.23) = 62.40; R_M = 5 x sqrt(30.77) = 27.74).

Watch for: the result is short run; when the specific factors can move, the long-run logic differs.

## 4. Factor-price equalization theorem (factor-price-equalization-theorem)

When to use it: two countries with the same techniques trade goods at common prices.

Equation as the chapter writes it:

    2w+r=30,\qquad w+2r=36,

Ask the user for: common techniques, each country's autarky prices and the trade prices.

Steps:
1. Solve each country's autarky pair (book: A (3, 18), B (13, 10)).
2. Solve the pair at trade prices (book: 3r = 2 x 36 - 30 = 42, r = 14, w = 8).
3. Report each factor's move toward the common point.

Watch for: equality fails if a country stops producing a good or techniques differ.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
