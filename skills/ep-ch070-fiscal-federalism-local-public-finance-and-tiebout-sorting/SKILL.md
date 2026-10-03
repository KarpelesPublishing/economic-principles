---
name: ep-ch070-fiscal-federalism-local-public-finance-and-tiebout-sorting
description: Apply Chapter 70 of The Encyclopedia of Economic Principals (Fiscal Federalism, Local Public Finance, and Tiebout Sorting) to the user's own numbers. Use when someone asks whether a service should be set locally or centrally, which town a household should choose given taxes, services, rents and moving costs, how a local tax change should move house prices, or whether public spending is growing faster than income.
---

# Chapter 70: Fiscal Federalism, Local Public Finance, and Tiebout Sorting

Decide where a service belongs, how households sort across towns, how fiscal packages are priced into houses, and whether government grows faster than income.

Notebook with the worked examples and figures: `../../notebooks/ch070-fiscal-federalism-local-public-finance-and-tiebout-sorting.ipynb`

## 1. Oates decentralization theorem (oates-decentralization-theorem)

When to use it: comparing locally chosen service levels with one uniform level.

    W^D=49+49+49=147;  W^U=40+49+40=129

Ask for: each district's preferred level and surplus curve, any spillover per unit.

Steps:
1. Tailored welfare: each district at its peak (book: 147).
2. Uniform welfare at the mean peak (book: q = 4 gives 40 + 49 + 40 = 129), gain 18.
3. With spillover s, District 1's best q = peak + s/2 (book s = 2: q = 2, contribution 52 against 51).

Watch for: spillovers and scale economies can reverse the ranking.

## 2. Tiebout sorting (tiebout-sorting)

When to use it: comparing towns' tax and service packages.

    (12-5)-(3-2)-m=6-m

Steps: net value per town = service value - tax - rent premium (book: high 12 - 5 = 7 vs 3 - 2 = 1); move if the gain 6 - m (less any rent) is positive (book m = 7 blocks it; rent 4 leaves 7 - 4 = 3).

Watch for: limited homes and rents can capture the package value.

## 3. Oates capitalization effect (oates-capitalization-effect)

When to use it: predicting a house price response to a tax or service change.

    Delta f=1,500-2,400=-900;  Delta P=-900/0.045=-20,000

Steps: annual net change Delta f (book: -900); perpetual Delta P = Delta f / r (book: -20,000); for n years Delta f x (1 - (1 + r)^-n)/r (book 10 years: -7,121); new price (book: 340,000).

Watch for: supply, risk and amenity changes also move prices.

## 4. Wagner's law (wagners-law)

When to use it: projecting public spending as income grows.

    G_1=96(1,200/800)^1.25=96(1.5)^1.25 approx 159.36

Steps: G_1 = G_0 (Y_1/Y_0)^eps (book: 159.36); share G_1/Y_1 (book: 13.28% vs 12%); the strong form needs eps > 1 (book eps 0.75: 130.12, share 10.84%).

Watch for: rising spending alone does not confirm the strong form.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
