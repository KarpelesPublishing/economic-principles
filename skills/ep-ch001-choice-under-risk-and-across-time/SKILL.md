---
name: ep-ch001-choice-under-risk-and-across-time
description: Apply Chapter 1 of The Encyclopedia of Economic Principals (Choice Under Risk and Across Time) to the user's own numbers. Use when someone weighs a sure amount against a gamble or insurance, asks what a risk is worth to them at a given wealth, plans saving across two periods at an interest rate or under a saving limit, or asks how income risk should change saving.
---

# Chapter 1: Choice Under Risk and Across Time

Price a risk with a certainty equivalent, and choose saving with an Euler equation and a lifetime budget.

Notebook with the worked examples and figures: `../../notebooks/ch001-choice-under-risk-and-across-time.ipynb`

## 1. Expected-utility theorem (expected-utility-theorem)

When to use it: comparing a risky prospect with a certain one, such as going uninsured versus buying cover.

    EU(A) = p u(x1) + (1 - p) u(x2);  certainty equivalent c solves u(c) = E[u(X)]

Ask for: the outcomes and their probabilities, the certain alternative, and a utility curve (default u(x) = sqrt(x), as in the chapter; say so).

Steps:
1. Expected income E[X] (book: 0.5 x 100 + 0.5 x 25 = 62.5).
2. Expected utility (book: 0.5 x sqrt(100) + 0.5 x sqrt(25) = 7.5).
3. Certainty equivalent from u(c) = EU (book: c = 7.5^2 = 56.25), risk premium E[X] - c (book: 6.25).
4. The certain option wins when it pays more than c (book: 58 > 56.25, so insure).

Watch for: the answer depends on the utility curvature, which is an assumption, not a measurement.

## 2. Arrow-Pratt risk-aversion measure (arrow-pratt-risk-aversion-measure)

When to use it: a quick price for a small risk at a given wealth.

    A(w) = -u''(w)/u'(w);  pi approx (1/2) A(w) Var(eps)

Steps: with log utility A(w) = 1/w (book: 0.0001 at $10,000); pi approx 0.5 x 0.0001 x 1,000,000 = $50; check against the exact w - CE (book: $50.13). For large stakes relative to wealth, use the exact value.

## 3. Intertemporal choice and discounting (intertemporal-choice-and-discounting)

When to use it: splitting resources between today and next period.

    c1 = beta(1 + r) c0;  c0 + c1/(1 + r) = y0 + y1/(1 + r)

Steps (log utility): resources = y0 + y1/(1 + r) (book: 120 + 100/1.04 = 216.1538); c0 = resources/(1 + beta) (book: 110.28); c1 = beta(1 + r) c0 (0.9984 x 110.2826 = 110.106, so 110.11; the book prints 110.10); saving y0 - c0 (book: 9.72). If saving exceeds a cap, set saving to the cap and recompute (book cap 5: 115 and 105.20).

Watch for: a capped or borrowing-limited path says nothing about patience.

## 4. Prudence and precautionary saving (prudence-and-precautionary-saving)

When to use it: future income becomes riskier with the same mean.

    1/(100 - s) = (1/2) 1/(50 + s) + (1/2) 1/(150 + s)

Steps (log utility, resources 100, future income 100 plus or minus d, no interest or discounting): solve s^2 + 100 s - d^2/2 = 0, so s = (-100 + sqrt(10,000 + 2 d^2))/2 (book d = 50: 11.24). With quadratic utility saving stays at 0.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied (utility form, probabilities).
- Report ties as ties.
- The chapter's numbers are hypothetical teaching values; never present them as facts about a real market.
