---
name: ep-ch057-new-trade-theory-firm-selection-scale-and-geography
description: Apply the principles of Chapter 57 of The Encyclopedia of Economic Principals (New Trade Theory, Firm Selection, Scale, and Geography) to the user's own numbers. Use when someone asks whether a larger market attracts more than its share of an industry, how much integration saves by removing duplicate plants, how much of a productivity gain comes from firms exiting and exporters growing, or how much a cut in trade costs raises bilateral exports.
---

# Chapter 57: New Trade Theory, Firm Selection, Scale, and Geography

Scale economies, firm selection and distance explain trade between similar countries.

Notebook with the worked examples and figures: `../../notebooks/ch057-new-trade-theory-firm-selection-scale-and-geography.ipynb`

## 1. Home-market effect (home-market-effect)

When to use it: a region's share of an industry's production is compared with its share of demand.

    s_E = 900 / (900 + 600) = 0.60;  s_N = 8 / 12 = 0.6667;  8(125) = 1,000

Ask the user for: demand in each region, producer counts (or output), output per producer.

Steps:
1. Demand share s_E (book: 900 / 1,500 = 0.60).
2. Producer share s_N (book: 8 / 12 = 0.6667).
3. Net exports = producers x output each - demand (book: 1,000 - 900 = 100).
4. A home-market effect shows as s_N above s_E with net exports.

Watch for: the producer allocation in the book is assumed, not derived; clustering can also come from inputs, skills or subsidies.

## 2. Scale mechanism (new-trade-theory-scale-mechanism)

When to use it: integration lets each variety be made once instead of in every country.

    C(q) = 90 + 2q;  C(75) = 90 + 2(75) = 240;  C(150) = 90 + 2(150) = 390;  4(390) = 1,560

Ask the user for: fixed cost per plant, marginal cost, varieties, units per market.

Steps:
1. Autarky cost = plants x C(q) (book: 8 x 240 = 1,920).
2. Integrated cost (book: 4 x 390 = 1,560).
3. Saving = duplicated plants x fixed cost (book: 4 x 90 = 360, 18.75 percent).

Watch for: free entry can turn the saving into new varieties instead of lower cost.

## 3. Melitz selection effect (melitz-selection-effect)

When to use it: industry productivity rose after trade opening and you need to know how much is reallocation.

    phi_bar = sum(weight x phi) / 100  (book: 232.5 / 100 = 2.325 before, 319.5 / 100 = 3.195 after)

Ask the user for: firm productivities and sales weights before and after.

Steps:
1. Weighted mean before (book: 2.325).
2. Weighted mean after (book: 3.195).
3. Change and percent (book: 0.870, 37.42 percent), stating that no firm's productivity changed.

Watch for: revenue productivity can rise through markups or quality rather than lower input use.

## 4. Gravity equation of trade (gravity-equation-of-trade)

When to use it: translating a bilateral trade-cost change into an export response.

    X'/X = (t'/t)^(1 - sigma)  (book: (1.22/1.30)^(1-4) = (1.30/1.22)^3 = 1.2099)

Ask the user for: current exports, sigma, old and new trade-cost factor.

Steps:
1. Ratio (book: 1.2099).
2. New exports (book: 160 x 1.2099 = 193.58 million).
3. Compare the cost cut (6.15 percent) with the export rise (20.99 percent).

Watch for: incomes and multilateral resistance are held fixed; diversion from other partners is ignored.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
