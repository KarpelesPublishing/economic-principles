---
name: ep-ch068-public-goods-free-riding-clubs-and-collective-funding
description: Apply Chapter 68 of The Encyclopedia of Economic Principals (Public Goods, Free Riding, Clubs, and Collective Funding) to the user's own numbers. Use when someone asks whether a shared service is worth one more unit, how a quadratic matching fund splits a limited pool, how many members a shared facility should admit, or whether a grant for a discovery with spillovers is justified.
---

# Chapter 68: Public Goods, Free Riding, Clubs, and Collective Funding

Add up shared benefits, fund them without free riding, and size the group that shares them.

Notebook with the worked examples and figures: `../../notebooks/ch068-public-goods-free-riding-clubs-and-collective-funding.ipynb`

## 1. Samuelson condition for public goods (samuelson-condition-for-public-goods)

When to use it: deciding on one more unit of a shared good.

    MB_3 = 22 + 15 + 11 + 8 = 56;  MB_4 = 16 + 12 + 9 + 6 = 43 < 50

Ask the user for: each group's marginal value for the next unit and its marginal cost.

Steps:
1. Sum the marginal values (book: 56).
2. Compare with marginal cost (book: 56 - 50 = 6, passes; fourth unit 43 < 50 fails).
3. Add omitted spillovers (book: 56 + 5 = 61 > 58 when finance raises cost to 58).

Watch for: the test says whether to provide, not who should pay.

## 2. Quadratic funding (quadratic-funding)

When to use it: designing or checking a matching fund.

    F_B = (4 sqrt(36))^2 = (4 x 6)^2 = 576;  M_B = 576 - 144 = 432

Steps: target (sum of square roots of gifts)^2 and match = target - gifts (book: 576 and 432; nine gifts of 16: 1,296 and 1,152); if desired matches exceed the pool, scale by beta = pool/total (book: 600/1,584 = 0.3788, paying 163.64 and 436.36).

Watch for: the arithmetic rewards splitting one donor into many accounts; verify donors are distinct.

## 3. Optimal club size (optimal-club-size)

When to use it: choosing membership for a facility with fixed cost and crowding.

    u(n) = 2,100 - 0.12n^2 - 72,000/n;  0.24n = 72,000/n^2;  n^3 = 300,000

Steps: n* = (C/(2a))^(1/3) (book: 66.94); compare the two neighbouring whole numbers (book: u(66) = 486.37, u(67) = 486.69); check the best u is positive.

Watch for: identical members; a weekend-only member crowds less than a daily one.

## 4. Public goods and knowledge spillovers (public-goods-spillovers)

When to use it: a grant to fund a project whose benefits leak to others.

    P = 6(45,000) = 270,000;  V = 270,000 + 230,000 = 500,000;  C - P = 420,000 - 270,000 = 150,000

Steps: private net P - C (book: -150,000); social net P + spillover - diffusion cost - C (book: 80,000; with 110,000 diffusion cost, -30,000); fund the gap C - P only if social net is positive.

Watch for: the grant moves who pays; it does not create the spillover.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
