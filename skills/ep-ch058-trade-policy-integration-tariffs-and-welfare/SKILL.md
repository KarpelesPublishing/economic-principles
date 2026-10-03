---
name: ep-ch058-trade-policy-integration-tariffs-and-welfare
description: Apply the principles of Chapter 58 of The Encyclopedia of Economic Principals (Trade Policy, Integration, Tariffs, and Welfare) to the user's own numbers. Use when weighing a tariff by a large importer, judging whether a depreciation will improve the trade balance, evaluating a free trade agreement for creation and diversion, or explaining a price gap between two connected markets.
---

# Chapter 58: Trade Policy, Integration, Tariffs, and Welfare

These principles let the user net the gains and losses of trade policy instead of judging it by trade volumes or prices alone.

Notebook with the worked examples and figures: `../../notebooks/ch058-trade-policy-integration-tariffs-and-welfare.ipynb`

## 1. Optimal-tariff argument (optimal-tariff-argument)

When to use it: a large importer considers a tariff to push down the price foreign suppliers accept.

Equations as the chapter writes them:

    p=(1+t)p^*
    t^*=\frac{1}{\varepsilon_x^*}
    t^*=\frac{1}{8}=0.125
    p=1.125(19.75)=22.21875
    0.25(108)=27
    \frac{1}{2}(12)(2.46875)=14.8125

Ask the user for: initial imports and foreign price, the foreign export-supply elasticity, the tariff, and the expected fall in imports.

Steps:
1. Foreign price cut = import fall / elasticity (book: 10 / 8 = 1.25 percent, so 20 becomes 19.75).
2. Home price = (1 + t) x foreign price (book: 1.125 x 19.75 = 22.21875).
3. Terms-of-trade gain = price cut x remaining imports (book: 0.25 x 108 = 27).
4. Distortion = 0.5 x lost imports x tariff wedge (book: 0.5 x 12 x 2.46875 = 14.8125).
5. Net = gain - distortion (book: 12.1875); say which elasticity would flip the sign.

Watch for: retaliation and administration costs, which the calculation ignores; world welfare falls regardless.

## 2. Marshall-Lerner condition (marshall-lerner-condition)

When to use it: deciding whether a depreciation will improve the trade balance.

Equations as the chapter writes them:

    TB=P_XX-eP_M^*M
    \varepsilon_X+\varepsilon_M>1
    P_XX=5(224)=1{,}120
    eP_M^*M=6(176)=1{,}056

Ask the user for: export and import volumes and prices before and after, and the exchange rates.

Steps:
1. Export receipts = P_X X (book: 5 x 224 = 1,120).
2. Import spending = e P_M* M (book: 6 x 176 = 1,056).
3. TB = receipts - spending (book: 64; weak case 1,030 - 1,164 = -134).
4. Midpoint elasticities and their sum (book: 0.62 + 0.70 = 1.32, above 1).

Watch for: incomplete pass-through and short-run lags (the J-curve).

## 3. Trade creation and trade diversion (trade-creation-and-trade-diversion)

When to use it: judging a free trade agreement product by product.

Equations as the chapter writes them:

    c_H,\qquad c_P+t_P,\qquad c_N+t_N
    12(80)=960
    (13-11.50)(120)=180

Ask the user for: home, partner and outsider costs, the tariff, and quantities per product.

Steps:
1. Find the cheapest delivered source before and after the partner's tariff is removed.
2. Creation: resource saving from leaving costlier home output (book: 1,280 - 960 = 320).
3. Diversion: buyer saving minus lost tariff revenue (book: 180 - 480 = -300).
4. Add across products (book: net 20); name ties in delivered price.

Watch for: fixed quantities; demand responses add consumption gains.

## 4. Commodity arbitrage (commodity-arbitrage-spatial-prices)

When to use it: explaining or trading on a price gap between two places.

Equations as the chapter writes them:

    \pi_{AB}=P_B-P_A-c_{AB}
    P_B-P_A\leq c_{AB}
    c_{AB}=21+8+5+4+3=41
    \pi_{AB}=201-150-41=10
    15+8+5+4+3=35

Ask the user for: both prices and each per-unit transfer cost.

Steps:
1. Transfer cost = sum of per-unit costs (book: 41).
2. Margin = P_B - P_A - cost (book: 201 - 150 - 41 = 10).
3. A positive margin draws shipments until the spread equals the cost (book: 195 - 154 = 41).

Watch for: costs that vary with volume or risk; the equilibrium spread is not zero.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
