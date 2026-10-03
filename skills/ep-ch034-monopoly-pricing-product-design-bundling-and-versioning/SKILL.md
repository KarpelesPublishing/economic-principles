---
name: ep-ch034-monopoly-pricing-product-design-bundling-and-versioning
description: Apply Chapter 34 of The Encyclopedia of Economic Principals (Monopoly Pricing, Product Design, Bundling, and Versioning) to the user's own numbers. Use when someone designs a membership fee plus usage price for different customers, decides how much to strip from a basic product tier, asks whether bundling two products beats separate prices, or reads a markup with the Lerner rule.
---

# Chapter 34: Monopoly Pricing, Product Design, Bundling, and Versioning

Choose tariffs, menus and packages for a seller with market power, and read the markup against demand elasticity.

Notebook with the worked examples and figures: `../../notebooks/ch034-monopoly-pricing-product-design-bundling-and-versioning.ipynb`

## 1. Two-part tariff (two-part-tariff)

When to use it: a fee plus a per-use price, with buyers of different demand.

    F=\frac{1}{2}(12-p)^2
    2F+(p-4)[(20-p)+(12-p)]=16+16p-p^2

Ask the user for: each type's inverse demand, marginal cost per use.

Steps:
1. Set the fee to the low type's surplus at price p (book: p = 8 gives F = 8).
2. Profit = 2F + (p - c)(total uses) (book: 16 + 64 = 80).
3. Compare with serving only the high type at full extraction (book: 128).

Watch for: outside options and congestion change both margins.

## 2. Versioning (versioning)

    50-2q_L-\frac{q_L^2}{2}
    18+2q_L-\frac{q_L^2}{2}

Ask the user for: the two types' valuations of quality, the quality cost.

Steps:
1. Write profit as thetaH^2/2 + (2 thetaL - thetaH) q_L - q_L^2/2 for cost q^2/2.
2. q_L = max(0, 2 thetaL - thetaH) (book: 0 when thetaH = 10, 2 when thetaH = 6).
3. Payments t_L = thetaL q_L and t_H = thetaH^2 - (thetaH - thetaL) q_L (book: 8 and 32, profit 20).

Watch for: the result needs single crossing and known type shares.

## 3. Bundling (bundling)

    90+90=\$180
    120(2)=\$240

Ask the user for: each buyer's value for each product, marginal cost.

Steps:
1. Best separate revenue (book: 90 + 90 = 180).
2. Each buyer's package value and the bundle revenue at a candidate price (book: 120 x 2 = 240).
3. Bundle only if it beats separate pricing (aligned values: 180 against 180, a tie).

Watch for: a buyer who wants only one product can be lost by pure bundling.

## 4. Lerner inverse-elasticity pricing rule (lerner-inverse-elasticity-pricing-rule)

    L=\frac{60-20}{60}=\frac{2}{3}
    \varepsilon=\frac{dQ}{dP}\frac{P}{Q}=(-2)\frac{60}{80}=-1.5

Ask the user for: residual demand, marginal cost.

Steps:
1. Set MR = MC (book: 100 - Q = 20, Q = 80, P = 60).
2. L = (P - MC)/P (book: 2/3).
3. Check against 1/|epsilon| (book: 1/1.5 = 2/3).

Watch for: a binding price ceiling breaks the link between margin and elasticity.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
