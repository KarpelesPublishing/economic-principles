---
name: ep-ch038-advertising-differentiation-quality-and-organizational-efficiency
description: Apply Chapter 38 of The Encyclopedia of Economic Principals (Advertising, Differentiation, Quality, and Organizational Efficiency) to the user's own numbers. Use when someone sizes an advertising budget from elasticities, compares input mixes that reach the same quality target as input prices change, weighs a status good against a ban and its enforcement, or asks whether a monopolist provides too much or too little quality.
---

# Chapter 38: Advertising, Differentiation, Quality, and Organizational Efficiency

Size advertising from two elasticities, choose the cheaper way to reach a quality target, price status against sanctions, and find the direction of a monopolist's quality distortion.

Notebook with the worked examples and figures: `../../notebooks/ch038-advertising-differentiation-quality-and-organizational-efficiency.ipynb`

## 1. Dorfman-Steiner condition (dorfman-steiner-condition)

When to use it: a firm that sets price and advertising together.

    A/PQ = eta_A / |e|,   (50 - 30)/50 = 0.40,   A/PQ = 0.20/2.5 = 0.08

Ask the user for: price, marginal cost (or price elasticity), advertising elasticity, sales.

Steps:
1. Margin (P - c)/P = 1/|e| (book: 20/50 = 0.40, so |e| = 2.5).
2. Share A/PQ = eta_A / |e| (book: 0.20 / 2.5 = 0.08).
3. Budget = share x sales (book: 0.08 x 500,000 = $40,000); check that the last ad dollar returns $1 of contribution (book: 20 x 0.05 = 1).

Watch for: elasticities estimated away from the optimum; they carry most of the uncertainty.

## 2. Quality-adjusted differentiation and labor-compute substitution (quality-adjusted-differentiation-labor-compute)

When to use it: two input mixes that both reach the same verified quality target.

    C_L = 8 + 7 = $15 million,   C_K = 4 + 14 = $18 million
    C_L' = 4(8) + 7 = $39 million,   C_K' = 4(4) + 14 = $30 million

Ask the user for: each mix's spending on each input, the new input prices.

Steps:
1. Cost each mix at current prices (book: 15 and 18).
2. Re-cost at the new prices (book: expert labor x4 gives 39 and 30).
3. Solve for the price multiple where the costs tie (book: 8w + 7 = 4w + 14, w = 1.75).

Watch for: mixes that do not truly reach the same quality on the failure modes that matter.

## 3. Sumptuary laws and Veblen goods (sumptuary-laws-and-veblen-goods)

When to use it: a status good, a restriction on who may display it, and enforcement.

    U_i = v_i + s_i(p, z) - p,   U_i^I = v_i + s_i(p, z) - p - rho F - c_i^E

Ask the user for: use value, status value at the price, price, detection probability, fine, evasion cost.

Steps:
1. Net utility of each buyer (book: 40 + 1.2(110) - 110 = 62 for M).
2. Expected sanction rho F (book: 0.70 x 100 = 70).
3. Illicit payoff minus sanction; evasion pays if positive (book: 62 - 70 = -8, no; at 0.20, 62 - 20 = 42, yes).

Watch for: linear status values are not credible at very high prices.

## 4. Spence monopoly-quality distortion (spence-monopoly-quality-distortion)

When to use it: a uniform-price seller choosing quality for a fixed set of buyers.

    C(s) = 20 s^2,  C_s(s) = 40 s;   400 = 40 s;   s_M = 900/40 = 22.5

Ask the user for: number of buyers, the boundary buyer's value per unit of quality, the average value, the cost curve.

Steps:
1. Firm: n x boundary value = marginal cost (book: 100 x 4 = 400 = 40s, s_M = 10).
2. Welfare: n x average value = marginal cost (book: 700 = 40s, s_W = 17.5).
3. Compare: s_M below s_W is under-provision; above is over-provision (book: boundary value 9 gives 22.5 > 17.5). Equal values mean no distortion.

Watch for: quality that changes how many buyers subscribe; then both conditions need the entrants.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
