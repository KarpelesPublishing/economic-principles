---
name: ep-ch044-asset-pricing-models-factors-and-empirical-puzzles
description: Apply Chapter 44 of The Encyclopedia of Economic Principals (Asset Pricing Models, Factors, and Empirical Puzzles) to the user's own numbers. Use when someone asks how much equity premium consumption risk can justify, whether price swings exceed what cash flows warrant, why a losing trader keeps betting to get back to even, or whether a size or value return spread survives a CAPM risk charge and trading costs.
---

# Chapter 44: Asset Pricing Models, Factors, and Empirical Puzzles

Test a return against the risk that should explain it, and check what is left after costs.

Notebook with the worked examples and figures: `../../notebooks/ch044-asset-pricing-models-factors-and-empirical-puzzles.ipynb`

## 1. Equity-premium puzzle (equity-premium-puzzle)

When to use it: judging whether consumption risk can explain an observed equity premium.

    m_{t+1} = beta (C_{t+1}/C_t)^(-gamma);  R^f = 1/E[m];  premium = -Cov(m, R^e)/E[m]

Ask the user for: consumption growth and equity return in each state, state probabilities, beta and gamma.

Steps:
1. m in each state (book: 1.02^(-2) = 0.96117 and 1).
2. E[m] and R^f = 1/E[m] (book: 0.98058, 1.01980).
3. Cov(m, R^e) = E[mR^e] - E[m]E[R^e] (book: 1.04476 - 0.98058 x 1.07 = -0.004466).
4. Premium = 0.004466/0.98058 = 0.004554, about 0.46 percentage point, against a stipulated 5 points: 4.54 unexplained.

Watch for: the 0.46 gap between state returns (1.30 minus 0.84) is not the 0.46 point premium. A gamma large enough to close the gap (near 25 here) also implies a safe rate far above the data.

## 2. Excess-volatility puzzle (excess-volatility-puzzle)

When to use it: prices move while expected cash flows do not.

    P* = 5/0.05 = 100 dollars;  variance = ((70 - 100)^2 + (130 - 100)^2)/2 = 900

Steps: value the cash flows at a constant rate (book: 100); compute price variance (book: 900 against 0); find the rate that justifies each price, d/P (book: 5/70 = 7.14%, 5/130 = 3.85%).

Watch for: the test is conditional on a constant discount rate.

## 3. Break-even effect (break-even-effect)

When to use it: deciding whether to take a bet after a loss.

    v(z) = sqrt(z) for z >= 0, -2 sqrt(-z) for z < 0;  U(gamble | L) = sum p_i v(L + x_i)

Steps: score the gamble alone (book: 0.5 sqrt(60) - 0.5(2 sqrt(70)) = -4.49, reject); after a loss L compare v(L) (book: -15.49) with 0.5 v(L + win) + 0.5 v(L + loss) (book: -11.40); report the expected final position (book: -65 against -60).

Watch for: the value function is illustrative; the point is that the odds did not improve.

## 4. Size and value effects (size-and-value-effects)

When to use it: evaluating a factor portfolio's excess return.

    R_f + beta(R_M - R_f) = 2% + 1.0(6%) = 8%;  11% - 8% = 3%;  3% - 4% = -1%

Steps: CAPM required return; alpha = return minus CAPM (book: 3%); subtract implementation costs (book: -1%).

Watch for: one period proves nothing about persistence or about risk versus mispricing.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
