---
name: ep-ch035-entry-scale-contestability-and-strategic-deterrence
description: Apply the principles of Chapter 35 of The Encyclopedia of Economic Principals (Entry, Scale, Contestability, and Strategic Deterrence) to the user's own numbers. Use when judging how many efficient firms a market can hold, whether to split an overloaded facility, what a cap on licenses does to profit, or how rank-sensitive attention concentrates an audience.
---

# Chapter 35: Entry, Scale, Contestability, and Strategic Deterrence

These principles let the user size a market against efficient plant scale, test a split of an overloaded unit, see how entry or its absence sets profit, and measure how sharply attention favors a leader.

Notebook with the worked examples and figures: `../../notebooks/ch035-entry-scale-contestability-and-strategic-deterrence.ipynb`

## 1. Minimum efficient scale (minimum-efficient-scale)

When to use it: the user knows the output at which unit cost bottoms out and the size of the market.

Equation as the chapter writes it:

    \frac{40{,}000}{150{,}000}=0.2667

Ask the user for: MES (units a year) and annual market demand (units).

Steps:
1. MES ratio = MES / demand (book: 40,000 / 150,000 = 0.2667).
2. Most equal efficient firms = whole part of demand / MES (book: 3, since 3 x 40,000 = 120,000).
3. Check one more firm: demand / (firms + 1) falls below MES (book: 150,000 / 4 = 37,500 < 40,000). State the count and the change in MES or demand that would add a firm.

Watch for: the count is a cost pressure, not a prediction; unequal shares and ramp-up losses change it.

## 2. Diseconomies of scale (diseconomies-of-scale)

When to use it: one facility is running past its lowest average cost and splitting is an option.

Equation as the chapter writes it:

    C(Q)=80{,}000+4Q+0.0008Q^2
    Q^*=\sqrt{\frac{80{,}000}{0.0008}}=10{,}000

Ask the user for: fixed cost F, unit cost c, quadratic coefficient b, volume Q and the number of units considered.

Steps:
1. Q* = sqrt(F / b) (book: 10,000, average cost $20).
2. Cost of one unit at Q (book: 80,000 + 64,000 + 204,800 = $348,800, $21.80 a parcel).
3. Cost of h units at Q / h each, times h (book: two hubs 2 x 163,200 = $326,400).
4. State the saving or loss of splitting (book: saves $22,400; at b = 0.0003 one hub costs $220,800 and splitting loses).

Watch for: identical units and no coordination cost between them are assumed.

## 3. Free-entry zero-profit condition (free-entry-zero-profit-condition)

When to use it: deciding whether profits in a trade will be competed away or are protected by a cap on entry.

Equation as the chapter writes it:

    Q_D=1200-30p
    30\left(\frac{p}{2}\right)=1200-30p

Ask the user for: market demand, each firm's cost function and any cap on the number of firms.

Steps:
1. Free-entry price = minimum average cost (book: C = 144 + q^2, minimum at q = 12, p = $24).
2. Free-entry count = demand at that price / output per firm (book: 480 / 12 = 40).
3. Under a cap n below that, solve n(p/2) = demand (book: n = 30 gives p = 26.67, q = 13.33, profit 177.78 - 144 = $33.78; n = 35 gives $15.56).
4. State whether profit persists and why.

Watch for: a license payment capitalizes the rent and is a transfer, not a resource cost.

## 4. Superstar markets and attention (power-law-superstar)

When to use it: a small quality gap appears to produce a very large gap in audience or revenue.

Equation as the chapter writes it:

    s_A=\frac{100^{80}}{100^{80}+97^{80}}=\frac{1}{1+0.97^{80}}\approx0.9196

Ask the user for: the two quality scores, an attention sensitivity kappa, audience size and revenue per viewer.

Steps:
1. Ratio term (z_B / z_A)^kappa (book: 0.97^80 = 0.087432).
2. s_A = 1 / (1 + term) (book: 0.9196).
3. Audiences and revenues (book: 459,793 and 40,207 viewers; the book rounds to 459,800 and 40,200; ratio 11.4 to 1).
4. Recompute with a lower kappa to show sensitivity (book: kappa 4 gives 0.5304).

Watch for: the share rule is illustrative; a capacity limit on the leader breaks the concentration.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
