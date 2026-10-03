---
name: ep-ch006-welfare-theorems-efficiency-and-the-second-best
description: Apply Chapter 6 of The Encyclopedia of Economic Principals (Welfare Theorems, Efficiency, and the Second Best) to the user's own numbers. Use when someone tests whether a reallocation is a Pareto improvement, measures the deadweight loss of a tax and offsets it against avoided external cost, judges a second-best subsidy with costly public funds, or asks whether a mandate can beat a market with hidden action.
---

# Chapter 6: Welfare Theorems, Efficiency, and the Second Best

Test changes against each person's starting point, measure the surplus a wedge destroys, and count every distortion a policy leaves in place.

Notebook with the worked examples and figures: `../../notebooks/ch006-welfare-theorems-efficiency-and-the-second-best.ipynb`

## 1. Pareto criterion (pareto-criterion)

    u_A = 2b_A + c_A,   u_B = b_B + 2c_B.

Ask the user for: each person's bundle before and after, and their preferences.

Steps:
1. Utility of each person before and after (book: (4, 4) gives 12 each; after one swap 13 each).
2. Pareto improvement only if no one loses and someone gains (book: unpaid loaf gives 14 and 11, fails).
3. Efficient when no feasible move passes the test (book: (8, 0) and (0, 8), both 16).

Watch for: never add one person's gain to another's loss.

## 2. Deadweight loss (deadweight-loss)

    (20 - 0.10Q) - (4 + 0.10Q) = 4,   (1/2)($4)(2,000) = $4,000.

Ask the user for: inverse demand and supply, the tax, any external damage per unit.

Steps:
1. Solve demand price minus supply price = tax (book: Q = 60 hundred, prices 14 and 10).
2. DWL = 0.5 x tax x quantity cut (book: 0.5 x 4 x 2,000 = 4,000). Revenue is a transfer.
3. Add avoided damage = damage x quantity cut and compare (book: 3 x 2,000 = 6,000, net 2,000).

Watch for: a tax above the damage per unit overshoots.

## 3. General theory of second best (general-theory-of-second-best)

    $12 - $6 - $2 = $4.   $12 - $6 - $2 - $6 = -$2.

Ask the user for: the external cost avoided, the extra resource costs, the subsidy and the cost per dollar of public funds.

Steps:
1. Resource gain (book: 12 - 6 - 2 = 4).
2. Subtract cost of funds = lambda x subsidy (book: 0.75 x 8 = 6, net -2).
3. Break-even lambda = resource gain / subsidy (book: 4 / 8 = 0.5).

Watch for: if the original distortion can be priced directly (a toll), the subsidy is unnecessary.

## 4. Greenwald-Stiglitz constrained inefficiency (greenwald-stiglitz-constrained-inefficiency)

    $6/100 = $0.06.   100($3) + 100(0.04)($100) = $700.

Ask the user for: pool size, loss, accident probabilities with and without the action, action cost, enforcement cost.

Steps:
1. Private gain from acting alone (book: 6 / 100 = 0.06, below the cost of 3, so no one acts).
2. Pool real cost with no policy (book: 1,000) and under a mandate (book: 300 + 400 = 700).
3. Add enforcement (book: 4 per driver gives 1,100, a loss).

Watch for: premium savings mirror avoided claims; do not count them twice.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and zero net gains instead of forcing a verdict.
- Do not present the book's hypothetical numbers as facts about any real market.
