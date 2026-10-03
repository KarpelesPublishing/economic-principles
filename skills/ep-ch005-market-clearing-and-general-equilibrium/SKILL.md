---
name: ep-ch005-market-clearing-and-general-equilibrium
description: Apply Chapter 5 of The Encyclopedia of Economic Principals (Market Clearing and General Equilibrium) to the user's own numbers. Use when someone solves a linear supply and demand market, asks whether a demand or supply shift explains a price and quantity change, measures the shortage under a price ceiling, checks whether a price adjustment rule converges, or asks whether an economy can have several equilibria.
---

# Chapter 5: Market Clearing and General Equilibrium

Find the price where plans meet, read shifts from the direction of price, and check whether an adjustment rule can actually reach the equilibrium.

Notebook with the worked examples and figures: `../../notebooks/ch005-market-clearing-and-general-equilibrium.ipynb`

## 1. Supply-and-demand market clearing (supply-and-demand-market-clearing)

When to use it: a market with linear demand and supply, before and after a shift.

    Q_D = 100 - 2p,   Q_S = 20 + 2p,   120 - 2p = 20 + 2p

Ask the user for: demand intercept and slope, supply intercept and slope, the shift.

Steps:
1. Set demand equal to supply and solve for p (book: 100 - 2p = 20 + 2p, p* = 20, Q* = 60).
2. Re-solve after the shift (book: demand +20 gives p = 25, Q = 70; supply +20 gives p = 15, Q = 70).
3. Price and quantity moving together point to demand; moving apart point to supply.

Watch for: both curves shifting at once, which can leave price unchanged.

## 2. Price controls and black markets (price-controls-and-black-markets)

    Q_D = 120 - 2P,   S = 90 - 50 = 40

Ask the user for: demand, supply, the ceiling, any imports at every price.

Steps:
1. Find the clearing price (book: 25). A ceiling binds only below it.
2. Demand and supply at the ceiling, shortage = demand minus supply (book: 90 - 50 = 40; with imports 20, 20).
3. Compare an illicit seller's net (price minus penalty) with the ceiling (book: 27 - 8 = 19 > 15).

Watch for: quantity sold equals supply, not demand; sales do not show the shortage.

## 3. Walrasian tatonnement (walrasian-tatonnement)

    p^{t+1} - 5 = 0.5(p^t - 5)

Ask the user for: excess demand z(p), adjustment speed alpha, starting price.

Steps:
1. Iterate p(t+1) = p(t) + alpha z(p(t)) (book: z = 10 - 2p, alpha 0.25 from 2 gives 3.5, 4.25, 4.625).
2. For linear z = a - bp the gap factor is 1 - alpha b (book: 0.5; alpha 1 gives -1, a cycle; alpha 1.1 gives -1.2).
3. Converges when the factor has size below 1.

Watch for: an existing equilibrium does not guarantee the rule finds it.

## 4. Sonnenschein-Mantel-Debreu theorem (sonnenschein-mantel-debreu-theorem)

    z_1(p) = -(p-1)(p-2)(p-3),   p z_1(p) + z_2(p) = 0

Ask the user for: an excess demand function and a starting price.

Steps:
1. Find all zeros (book: 1, 2, 3).
2. Evaluate z at the start (book: z(1.5) = -(0.5)(-0.5)(-1.5) = -0.375, so price falls toward 1).
3. Equilibria where z crosses from positive to negative are stable (book: 1 and 3; 2 is unstable).

Watch for: the polynomial is illustrative; uniqueness needs extra structure such as gross substitutes.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and nonbinding cases instead of forcing a result.
- Do not present the book's hypothetical numbers as facts about any real market.
