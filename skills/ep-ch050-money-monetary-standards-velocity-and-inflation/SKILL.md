---
name: ep-ch050-money-monetary-standards-velocity-and-inflation
description: Apply Chapter 50 of The Encyclopedia of Economic Principals (Money, Monetary Standards, Velocity, and Inflation) to the user's own numbers. Use when someone asks how much a money increase will raise prices given velocity and output, how falling prices change the real burden of a debt, how often to move cash out of an interest-bearing account, or how much an inflation tax takes from existing money holders.
---

# Chapter 50: Money, Monetary Standards, Velocity, and Inflation

Trace a change in money through prices, real debts, cash management and the issuer's revenue.

Notebook with the worked examples and figures: `../../notebooks/ch050-money-monetary-standards-velocity-and-inflation.ipynb`

## 1. Quantity theory of money (quantity-theory-of-money)

When to use it: forecasting the price level after a change in money, velocity or output.

Equation as the chapter writes it:

    P_1=\frac{1{,}250\times4}{2{,}000}=2.5

Ask the user for: money before and after, velocity before and after, real output before and after.

Steps:
1. P0 = M0 V0 / Y0 (book: 1,000 x 4 / 2,000 = 2).
2. P1 = M1 V1 / Y1 (book: 1,250 x 4 / 2,000 = 2.5; with velocity 3.2 it stays 2; with output 2,200 it is 2.2727).
3. Percent change = (P1 - P0) / P0 (book: 25 percent, or 13.64 percent with output 2,200).

Watch for: the identity holds by definition; the forecast is only as good as the assumptions about velocity and output.

## 2. Deflation and monetary contraction (deflation-and-monetary-contraction)

When to use it: judging how a contraction of money or spending changes real debt burdens.

Equations as the chapter writes them:

    P_1=\frac{450\times3.8}{980}\approx1.7449
    M^*=\frac{P_0Y_1}{V_1}=\frac{2\times980}{3.8}\approx515.79

Ask the user for: money, velocity and output before and after, and the nominal debt.

Steps:
1. Compute P0 and P1 (book: 2 and 1.7449, a fall of 12.76 percent).
2. Real debt = nominal debt / P (book: 200 / 2 = 100, then 200 / 1.7449 = 114.62).
3. Money that restores P0 at the new velocity and output: M* = P0 Y1 / V1 (book: 515.79, so 65.79 more).

Watch for: M* is an accounting counterfactual, not a promise that extra money cures insolvency.

## 3. Baumol-Tobin transactions demand for money (baumol-tobin-transactions-demand-for-money)

When to use it: choosing how often to move cash out of an interest-bearing account.

Equation as the chapter writes it:

    n^*=\sqrt{\frac{0.04\times24{,}000}{2\times6}}=\sqrt{80}\approx8.944

Ask the user for: annual spending T (dollars), cost per transfer b (dollars), interest rate i.

Steps:
1. n* = sqrt(i T / (2 b)) (book: sqrt(80) = 8.944).
2. Compare the two neighbouring whole numbers with C(n) = b n + i T / (2n) (book: C(9) = 54 + 53.33 = 107.33; C(8) = C(10) = 108).
3. Optimal average balance = sqrt(b T / (2 i)) (book at 9 percent: 894.43 dollars, with n* = 13.416).

Watch for: the rule assumes even spending and certain payments; uncertain outflows call for an extra buffer.

## 4. Seigniorage and the inflation tax (seigniorage-inflation-tax)

When to use it: measuring what a one-time money issue takes from existing holders.

Equations as the chapter writes them:

    \frac{10{,}000}{1}-\frac{10{,}000}{1.10}=10{,}000-9{,}090.91=909.09
    s=\frac{1{,}000}{1.10}=909.09

Ask the user for: existing holdings, the new issue, and the price index before and after.

Steps:
1. Inflation = P1 / P0 - 1 (book: 10 percent).
2. Exact erosion = holdings / P0 - holdings / P1 (book: 909.09).
3. Compare with the shortcut inflation x beginning balances (book: 1,000, too high by 90.91).
4. Seigniorage = issue / P1 (book: 909.09, equal to the holders' loss).

Watch for: the equality of loss and gain fails with growing output, shifting money demand, interest-bearing money or production costs.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
