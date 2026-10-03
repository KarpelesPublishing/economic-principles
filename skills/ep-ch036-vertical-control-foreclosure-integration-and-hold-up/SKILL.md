---
name: ep-ch036-vertical-control-foreclosure-integration-and-hold-up
description: Apply the principles of Chapter 36 of The Encyclopedia of Economic Principals (Vertical Control, Foreclosure, Integration, and Hold-Up) to the user's own numbers. Use when a supplier and a retailer both mark up, when an incumbent pays buyers for exclusivity, when a firm raises a rival's input cost, or when choosing to make or buy a component.
---

# Chapter 36: Vertical Control, Foreclosure, Integration, and Hold-Up

These principles let the user price a supply chain with stacked markups, test whether exclusive contracts foreclose an entrant, check whether raising a rival's cost pays, and find the volume at which making beats buying.

Notebook with the worked examples and figures: `../../notebooks/ch036-vertical-control-foreclosure-integration-and-hold-up.ipynb`

## 1. Double marginalization (double-marginalization)

When to use it: an upstream firm with market power sells through a downstream firm that also has market power.

Equation as the chapter writes it:

    p=\frac{100+w}{2},\qquad Q=\frac{100-w}{2}
    \max_p (p-10)(100-p)

Ask the user for: linear demand (intercept a, slope), upstream marginal cost c.

Steps:
1. Upstream fee w = (a + c) / 2 (book: (100 + 10) / 2 = 55).
2. Retail price p = (a + w) / 2 and quantity (book: 77.50 and 22.5).
3. Profits: upstream (w - c)Q, downstream (p - w)Q (book: 1,012.50 and 506.25, joint 1,518.75).
4. Integrated price (a + c) / 2 and profit (book: 55, 45 units, 2,025). State the price gap and the joint gain.

Watch for: with competitive retail there is no second markup to remove.

## 2. Exclusive-dealing foreclosure (exclusive-dealing-foreclosure)

When to use it: an incumbent pays small buyers for exclusivity and an entrant needs a minimum volume.

Equation as the chapter writes it:

    6(\$500)=\$3{,}000

Ask the user for: number of buyers, units each, entry threshold, payment per exclusive and the per-unit saving from entry.

Steps:
1. Open units = unsigned buyers x units each (book: 5 x 10 = 50).
2. Compare with the threshold (book: 50 < 60, entry blocked).
3. Smallest rejecting coalition, its gain and the payments it gives up (book: 6 x $500 = $3,000 against 6 x $100 = $600).

Watch for: a single large buyer able to reach the threshold alone breaks the scheme.

## 3. Raising rivals' costs (raising-rivals-costs)

When to use it: a firm can pay to raise a competitor's input cost.

Equation as the chapter writes it:

    Q_D=Q_R=\frac{100-2(20)+20}{3}=26.67

Ask the user for: linear inverse demand, each firm's cost before and after, and the cost of the contract.

Steps:
1. Cournot quantities Q_i = (a - 2c_i + c_j) / 3 (book: (100 - 40 + 35) / 3 = 31.67 and 16.67).
2. Price and profit; with P = a - Q_D - Q_R, profit is Q_D^2 (book: (95/3)^2 = 1,002.78).
3. Subtract the contract and compare with the baseline (book: 902.78 against 711.11, a gain of 191.67; with own cost 30 the net is 525 and the strategy fails).

Watch for: the calculation assumes both firms keep producing.

## 4. Vertical integration (vertical-integration)

When to use it: deciding whether to make an input in house or buy it.

Equation as the chapter writes it:

    C_M=100{,}000(\$40)+\$400{,}000+\$600{,}000=\$5.0\text{ million}
    C_I=\$1.8\text{ million}+100{,}000(\$28)+\$300{,}000=\$4.9\text{ million}

Ask the user for: volume, market price, contracting and hold-up costs, internal setup, internal unit cost and administration.

Steps:
1. C_M = V x price + contracting + hazard (book: $5.0 million).
2. C_I = setup + V x unit cost + administration (book: $4.9 million).
3. Break-even volume = (fixed difference) / (unit saving) (book: 1,100,000 / 12 = 91,667). State the choice and how far volume can fall before it flips.

Watch for: hazard and setup terms are expectations; different values move the break-even point.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
