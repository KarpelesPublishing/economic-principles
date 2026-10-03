---
name: ep-ch059-exchange-rates-capital-flows-crises-and-open-economy-policy
description: Apply the principles of Chapter 59 of The Encyclopedia of Economic Principals (Exchange Rates, Capital Flows, Crises, and Open-Economy Policy) to the user's own numbers. Use when the user asks how an interest-rate cut moves the exchange rate, whether a forward quote leaves a covered arbitrage, why productivity growth raises a country's price level, or why a depreciation first worsens the trade balance.
---

# Chapter 59: Exchange Rates, Capital Flows, Crises, and Open-Economy Policy

These principles turn interest rates, forward quotes, productivity and trade volumes into exchange-rate paths, arbitrage profits, price levels and trade balances.

Notebook with the worked examples and figures: `../../notebooks/ch059-exchange-rates-capital-flows-crises-and-open-economy-policy.ipynb`

## 1. Dornbusch overshooting (dornbusch-overshooting)

When to use it: a monetary shock lowers the domestic rate while goods prices are sticky.

Equation as the chapter writes it:

    1+i=(1+i^*)\frac{E_tS_{t+1}}{S_t}

Ask the user for: impact spot rate S_t, domestic rate i, foreign rate i*, long-run rate.

Steps:
1. Expected rate E S = S_t (1 + i) / (1 + i*) (book: 1.15 x 1.01 / 1.05 = 1.1062).
2. Expected change E S / S_t - 1 (book: -3.81 percent, an appreciation).
3. Overshoot = impact rate minus long-run rate (book: 1.15 - 1.10 = 5 points). Overshooting needs i < i*, so that an expected appreciation back toward the long-run rate exists.

Watch for: the model takes the impact rate as given; exact uncovered parity rarely holds in data.

## 2. Covered interest parity (covered-interest-parity)

When to use it: comparing a quoted forward rate with interest rates in two currencies.

Equations as the chapter writes them:

    1+i_d=\frac{F}{S}(1+i_f)
    F=1.20\left(\frac{1.05}{1.02}\right)\approx1.2353

Ask the user for: spot S, domestic rate i_d, foreign rate i_f, quoted forward F.

Steps:
1. Parity forward S (1 + i_d) / (1 + i_f) (book: 1.2353).
2. Foreign route (1 / S)(1 + i_f) F (book at F = 1.26: 0.85 x 1.26 = 1.071).
3. Profit = foreign route - (1 + i_d) (book: 1.071 - 1.05 = 0.021); a negative value means the reverse trade.

Watch for: spreads, collateral and capital charges larger than the gap remove the arbitrage.

## 3. Balassa-Samuelson effect (balassa-samuelson-effect)

When to use it: explaining higher price levels in countries with productive traded sectors.

Equations as the chapter writes them:

    w=P_TA_T=P_NA_N
    P=P_T^{\alpha}P_N^{1-\alpha}
    P_{N,0}=\frac{w_0}{A_N}=\frac{20}{10}=2

Ask the user for: traded price P_T, traded and service productivity A_T and A_N, expenditure share.

Steps:
1. Wage w = P_T A_T (book: 1 x 30 = 30).
2. Service price P_N = w / A_N (book: 30 / 10 = 3).
3. Index P = P_T^0.5 P_N^0.5 (book: sqrt(3) = 1.732, up 22.5 percent from 1.414); real exchange rate change P0 / P1 - 1 (book: -18.4 percent).

Watch for: it assumes mobile labor and a fixed world traded price.

## 4. J-curve effect (j-curve-effect)

When to use it: tracking the trade balance in the quarters after a depreciation.

Equations as the chapter writes them:

    TB=P_XX-EP_M^*M
    TB_1=100(10)-100(12)=-200

Ask the user for: export and import volumes and prices before, just after and some quarters after.

Steps:
1. TB = export price x export volume - import price x import volume at each date.
2. Just after: volumes fixed, import price up (book: 1,000 - 1,200 = -200).
3. Later: volumes respond (book: 125 x 11 - 70 x 12 = 1,375 - 840 = 535; weak case 20).

Watch for: a J is not guaranteed; small volume responses leave the balance negative.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
