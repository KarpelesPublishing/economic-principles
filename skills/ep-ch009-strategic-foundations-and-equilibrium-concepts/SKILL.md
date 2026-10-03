---
name: ep-ch009-strategic-foundations-and-equilibrium-concepts
description: Apply Chapter 9 of The Encyclopedia of Economic Principals (Strategic Foundations and Equilibrium Concepts) to the user's own payoffs. Use when someone needs an optimal randomized inspection or monitoring rate, the Nash equilibria of a two-by-two game, whether to act on information the other side may not have received, or whether a recommendation schedule will be obeyed.
---

# Chapter 9: Strategic Foundations and Equilibrium Concepts

Predict play by asking what each side does against the other's best choice, and check what each side knows.

Notebook with the worked examples and figures: `../../notebooks/ch009-strategic-foundations-and-equilibrium-concepts.ipynb`

## 1. Minimax theorem (minimax-theorem)

    4p = 2(1 - p),   4q = 2(1 - q)

Ask the user for: the 2 x 2 zero-sum payoffs.

Steps:
1. Check for a saddle point; if none, equalize the two lines (book: 4p = 2(1 - p), p = 1/3).
2. Value = the common payoff (book: 4/3, about $1,333).
3. If the opponent can observe the draw, the mixed guarantee disappears (book: 0).

## 2. Nash equilibrium and existence (nash-equilibrium-and-existence)

    p(-1) + (1 - p)6 = 6 - 7p,   p(0) + (1 - p)4 = 4 - 4p.

Ask the user for: the four payoff pairs.

Steps:
1. Best reply to each rival action (book: Offer against both, so (O, O) is unique).
2. Mark cells where both reply best (book with -1 at (O, O): (O, N) and (N, O)).
3. Mixed: make the rival indifferent (book: p = 2/3, payoff 4/3).

## 3. Common knowledge (common-knowledge)

    0.9(5) + 0.1(-50) = -0.5.   0.9(5) + 0.1(-10) = 3.5 > 0.

Steps:
1. Expected payoff of acting = d x gain - (1 - d) x loss (book: -0.5, so wait).
2. Break-even d = loss / (gain + loss) (book: 50 / 55 = 0.909).

## 4. Correlated equilibrium (correlated-equilibrium)

    0.4 / (0.4 + 0.2) = 2/3,   (2/3)(2) + (1/3)(4) = 8/3,   (2/3)(0) + (1/3)(6) = 2.

Steps:
1. For each recommendation, the conditional distribution of the other's recommendation (book: 2/3).
2. Compare obeying with the best deviation (book: 8/3 against 2, obeyed).
3. Expected payoff of the schedule (book: 4 each against 3 under mixing).

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which payoffs are the user's and which are assumptions you added.
- Name ties and multiple equilibria instead of forcing one prediction.
- Do not present the book's hypothetical payoffs as facts about real firms.
