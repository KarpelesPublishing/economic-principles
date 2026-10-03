---
name: ep-ch093-agrarian-households-food-demand-and-adaptation
description: Apply the principles of Chapter 93 of The Encyclopedia of Economic Principals (Agrarian Households, Food Demand, and Adaptation) to the user's own numbers. Use when judging whether household preferences affect farm labor because a labor market is missing, where land-use boundaries fall as transport costs change, what share contract induces effort and how much risk it loads on the tenant, or whether a lagged supply cycle converges or explodes.
---

# Chapter 93: Agrarian Households, Food Demand, and Adaptation

These principles turn farm decisions into checkable margins: operative wages, crossing bid rents, effort incentives under sharing, and lagged price cycles. The chapter's numbers are hypothetical teaching values, not data from a real farm or market.

Notebook with the worked examples and figures: `../../notebooks/ch093-agrarian-households-food-demand-and-adaptation.ipynb`

## 1. Agricultural-household nonseparability (agricultural-household-nonseparability)

When to use it: deciding whether a transfer or preference change should move farm production.

Equations as the chapter writes them:

    pf_L=\frac{U_{\ell}}{U_c}=w^s.
    MR(L_f)=102-10L_f.

Ask the user for: the marginal revenue product schedule, the market wage, whether labor can be bought and sold, and the household's shadow wage.

Steps:
1. Operative wage = market wage if the market works, else the shadow wage.
2. Solve MR(L) = operative wage (book: 102 - 10L = 42 gives 6; shadow 22 gives 8; shadow 32 gives 7).

Watch for: a lower labor response among transfer recipients may also reflect health, childcare or crop shocks.

## 2. Von Thünen land-use rings (von-thunen-land-use-rings)

When to use it: locating the boundary between competing land uses and how it moves with transport cost.

Equations as the chapter writes them:

    R_v(d)=1{,}080-110d,
    R_g(d)=620-20d,

Ask the user for: each use's bid at the market and its fall per unit of distance.

Steps:
1. Boundary d = (a1 - a2) / (t1 - t2) (book: 460 / 90 = 5.11).
2. Outer margin where the outer bid is zero (book: 620 / 20 = 31).
3. Repeat with the new slope (book: slope 55 gives 460 / 35 = 13.14; at d = 10 vegetables bid 530 against grain 420).

Watch for: routes, not radial distance, matter when access improves only along some roads.

## 3. Stiglitz sharecropping tradeoff (stiglitz-sharecropping-tradeoff)

When to use it: choosing a revenue share that balances incentives and risk.

Equation as the chapter writes it:

    s\Delta Y=0.50(48)=24.

Ask the user for: output in good and bad states, the output gain from effort, the effort cost, and the share.

Steps:
1. Private gain = s x gain; effort is high if it covers the cost (book: 0.50 x 48 = 24 < 27, low; 0.65 x 48 = 31.2, high).
2. Risk borne = s x (good - bad) (book: 40 at one half, 52 at 0.65, 80 under fixed rent).
3. Minimum share = cost / gain.

Watch for: insurance from other sources changes the best share and may create new hidden-action problems.

## 4. Cobweb theorem (cobweb-theorem)

When to use it: predicting whether a cycle in a market with lagged supply settles or grows.

Equations as the chapter writes them:

    a-bP_t=c+dP_{t-1}.
    P_t-P^*=-\frac{d}{b}(P_{t-1}-P^*).

Ask the user for: the demand and supply schedules and last period's price.

Steps:
1. P* = (a - c) / (b + d) (book: 84 / 3 = 28).
2. Iterate P_t = (a - c - d P_(t-1)) / b (book: from 40, 22, 31, 26.5).
3. Deviation ratio -d / b decides convergence (book: -1/2 converges; d = 3 gives -3/2, explodes).

Watch for: forecasting, inventories or same-period supply remove the lag, and an exploding linear cycle soon needs impossible negative prices.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real farm or market.
