---
name: ep-ch072-redistribution-social-insurance-giving-and-patronage
description: Apply Chapter 72 of The Encyclopedia of Economic Principals (Redistribution, Social Insurance, Giving, and Patronage) to the user's own numbers. Use when someone asks what a linear tax and equal transfer gives the median voter, whether disaster relief discourages preparation, how much of a raise a household keeps under a benefit phaseout, or whether a distorting tax-financed transfer raises welfare under stated weights.
---

# Chapter 72: Redistribution, Social Insurance, Giving, and Patronage

Work out who gains from a transfer, how people respond to it, and how its losses are weighed.

Notebook with the worked examples and figures: `../../notebooks/ch072-redistribution-social-insurance-giving-and-patronage.ipynb`

## 1. Meltzer-Richard redistribution mechanism (meltzer-richard-redistribution-mechanism)

When to use it: judging how much a median voter gains from a linear tax returned as an equal transfer.

    y_i(t) = (1 - 0.1t) z_i;  b(t) = t x mean taxable earnings;  c_m(t) = (1 - t) y_m + b(t)

Ask the user for: everyone's baseline earnings, the tax rate and the earnings response (default 0.1 per unit of t, as in the chapter; say so).

Steps:
1. Mean and median earnings (book: (18 + 28 + 38 + 58 + 108) / 5 = 50; median 38).
2. Response factor and taxable mean (book: 1 - 0.1 x 0.20 = 0.98; 0.98 x 50 = 49).
3. Transfer (book: 0.20 x 49 = 9.80).
4. Median voter's resources (book: 0.80 x 37.24 + 9.80 = 39.592, above 38).
5. A wider mean-median gap raises the return (book: top 158 gives b = 11.76 and c_m = 41.552).

Watch for: this is a mechanical comparison; it ignores the value of leisure and does not find the voter's best rate.

## 2. Samaritan's dilemma (samaritans-dilemma)

When to use it: checking whether relief coverage removes the private reason to prepare.

    J_N = (1 - c) x loss without preparation;  J_P = preparation cost + (1 - c) x loss with preparation

Steps:
1. Own costs (book at c = 0.75: J_N = 0.25 x 120 = 30; J_P = 24 + 0.25 x 50 = 36.50).
2. The household prepares only if J_P < J_N (book: 30 < 36.50, so it does not).
3. Resource comparison (book: 120 against 24 + 50 = 74, a saving of 46).
4. The coverage that flips the choice (book: at 0.50, J_N = 60 and J_P = 49, so it prepares).

Watch for: liquidity, inequality and catastrophic risk also bear on the right coverage.

## 3. Welfare economics, redistribution, and subsidies (welfare-redistribution)

When to use it: how much of extra earnings a household keeps as a means-tested benefit phases out.

    T(e) = max(0, B - p e);  disposable income = e + T(e)

Steps:
1. Benefits at both earnings levels (book: 9,000 - 0.40 x 12,000 = 4,200 and 9,000 - 0.40 x 18,000 = 1,800).
2. Disposable incomes and the gain (book: 16,200 and 19,800, gain 3,600, 60 percent kept).
3. Repeat at another rate (book p = 0.20: 18,600 and 23,400, gain 4,800, 80 percent kept, payments up 2,400 and 3,600).

Watch for: the benefit cannot go below zero; past the end of the phaseout the household keeps everything.

## 4. Welfare economics and redistribution (welfare-economics-redistribution)

When to use it: judging a tax-financed transfer with explicit welfare weights.

    Delta W = sum of weighted transfers - D - A

Steps:
1. Prices and quantity with the levy (book: Q_D = 120 - P_b, Q_S = P_s - 20, t = 18: P_s = 61, P_b = 79, Q = 41).
2. Revenue and triangle (book: R = 18 x 41 = 738; D = 0.5 x 18 x 9 = 81).
3. Weighted change (book: 1.4(738) - 738 - 81 - 30 = 184.2; equal weights: 738 - 738 - 81 - 30 = -111).

Watch for: the ranking turns on the normative weight; the distortion and administration are losses under any weight.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
