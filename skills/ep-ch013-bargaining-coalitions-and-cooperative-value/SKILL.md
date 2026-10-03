---
name: ep-ch013-bargaining-coalitions-and-cooperative-value
description: Apply Chapter 13 of The Encyclopedia of Economic Principals (Bargaining, Coalitions, and Cooperative Value) to the user's own numbers. Use when someone predicts how outside options split a deal, how patience divides a surplus in alternating offers, how to share a joint venture's value by marginal contribution, or whether any split of a group saving can satisfy every subgroup.
---

# Chapter 13: Bargaining, Coalitions, and Cooperative Value

Outside options, patience and marginal contributions decide who gets what.

Notebook with the worked examples and figures: `../../notebooks/ch013-bargaining-coalitions-and-cooperative-value.ipynb`

## 1. Nash bargaining solution (nash-bargaining-solution)

    N(x) = x(120 - x).   N'(x) = 120 - 2x = 0,   N_1(x) = (x - 30)(120 - x),

Steps:
1. Surplus over both outside options (book: 120 - 30 - 0 = 90).
2. Each side gets its option plus half that surplus (book: x = 75, gains 45 each).

Watch for: with only a few indivisible options, the product can tie (book: (80, 40) and (40, 80) both 3,200).

## 2. Rubinstein alternating-offers result (rubinstein-alternating-offers-result)

    x = (1 - 0.90)/(1 - (0.90)(0.90)) = 0.10/0.19 approx 0.526316.

Steps:
1. First proposer's share x = (1 - d_responder) / (1 - d_proposer d_responder).
2. Multiply by the surplus (book: 52,631.58; with the firm at 0.80, 71,428.57).

## 3. Shapley value (shapley-value)

    (phi_A, phi_B, phi_C) = (130/3, 145/3, 85/3) approx (43.33, 48.33, 28.33).

Steps:
1. List every arrival order and each member's marginal contribution (book: totals 260, 290, 170).
2. Average over the orders (book: divide by 6).
3. Check the shares sum to the grand coalition's value (book: 120).

## 4. Bondareva-Shapley theorem (bondareva-shapley-theorem)

    (1/2)(60) + (1/2)(60) + (1/2)(60) = 90 <= 100.   2(x_A + x_B + x_C) >= 210,

Steps:
1. Put weights on coalitions so every member is covered exactly once (book: 1/2 on each pair).
2. Weighted claim against the grand coalition (book: 90 <= 100, core nonempty; pairs at 70 give 105 > 100, empty).

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and empty cores instead of forcing a split.
- Do not present the book's hypothetical numbers as facts about real negotiations.
