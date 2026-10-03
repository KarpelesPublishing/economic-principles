---
name: ep-ch032-market-structure-competition-and-price-dispersion
description: Apply Chapter 32 of The Encyclopedia of Economic Principals (Market Structure, Competition, and Price Dispersion) to the user's own numbers. Use when someone asks how price comparison changes price spreads and margins, why a zero-profit firm still prices above marginal cost, whether a most-favored-customer clause makes a discount unprofitable, or why small search costs can keep prices high.
---

# Chapter 32: Market Structure, Competition, and Price Dispersion

Work out how search, comparison, entry and contract terms set prices and margins when competition is imperfect.

Notebook with the worked examples and figures: `../../notebooks/ch032-market-structure-competition-and-price-dispersion.ipynb`

## 1. Burdett-Judd price dispersion (burdett-judd-price-dispersion)

When to use it: two sellers of an identical good, some buyers compare both prices.

    p_L=15+60\left(\frac{0.60}{1.40}\right)=\frac{285}{7}\approx\$40.71
    \bar\pi=\frac{(75-15)(0.60)}{2}=\$18

Ask the user for: marginal cost c, buyer value v, share of comparing buyers lambda.

Steps:
1. Lower support p_L = c + (v - c)(1 - lambda)/(1 + lambda) (book: 15 + 60 x 0.60/1.40 = 40.71).
2. Profit per seller (v - c)(1 - lambda)/2 (book: 60 x 0.60 / 2 = 18).
3. For a price p in the support, 1 - F(p) = (1 - lambda)/(2 lambda) x (v - p)/(p - c) (book: 0.75 x 24/36 = 0.50).

Watch for: the spread is a mixed strategy among identical sellers, not a quality difference.

## 2. Monopolistic competition (monopolistic-competition)

    MR=20-q,\qquad MC=5+0.5q
    ATC(q)=5+0.25q+\frac{75}{q}

Ask the user for: residual demand intercept and slope, variable cost, fixed cost.

Steps:
1. Set MR = MC (book: 20 - q = 5 + 0.5q, q = 10, p = 15).
2. Profit = revenue - variable cost - fixed cost (book: 150 - 75 - 75 = 0).
3. Compare price with MC (15 against 10) and output with minimum-ATC output (10 against sqrt(300) = 17.32).

Watch for: entry modeled only as a shift in the residual demand intercept.

## 3. Most-favored-customer effect (most-favored-customer-effect)

    (42-30)(10)>(50-42)Q^P
    Q^P<\frac{120}{8}=15

Ask the user for: old price, bid, marginal cost, new order size, protected past volume.

Steps:
1. Contribution = (bid - MC) x new order (book: 12 x 10 = 120).
2. Refund = (old price - bid) x protected volume (book: 8 x 80 = 640).
3. Net = contribution - refund (book: -520); bid only if protected volume is below contribution / discount (book: 15).

Watch for: the clause's breadth and timing, not its name, decide the protected volume.

## 4. Diamond search paradox (diamond-search-paradox)

    \frac{0.85}{60}+0.15=\frac{197}{1200}\approx0.1642
    (35-12)\frac{197}{1200}=\frac{4531}{1200}\approx\$3.78

Ask the user for: cost, buyer value, number of sellers, informed share, candidate deviation price.

Steps:
1. Common-price profit (v - c)/n (book: 24/60 = 0.40).
2. Deviator demand (1 - phi)/n + phi (book: 0.1642).
3. Deviator profit (p - c) x demand and compare (book: 3.78 > 0.40, so the common price fails).

Watch for: with no informed buyers a cut is invisible, so it only lowers the margin.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
