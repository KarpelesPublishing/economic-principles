---
name: ep-ch029-mechanism-design-revelation-and-implementation
description: Apply the principles of Chapter 29 of The Encyclopedia of Economic Principals (Mechanism Design, Revelation, and Implementation) to the user's own numbers. Use when judging how much trade a posted price can achieve, comparing weighted social choice rules, designing a forecast scoring rule, or computing VCG payments for a shared resource.
---

# Chapter 29: Mechanism Design, Revelation, and Implementation

These principles let the user see what a fixed price cannot achieve, how weights decide a public choice, how to pay forecasters for honesty, and what each winner owes under VCG.

Notebook with the worked examples and figures: `../../notebooks/ch029-mechanism-design-revelation-and-implementation.ipynb`

## 1. Myerson-Satterthwaite theorem (myerson-satterthwaite-theorem)

When to use it: bilateral trade where both sides have private values that overlap.

Equations as the chapter writes them:

    \frac14(30+0+80+30)=35
    \frac14(80)=20
    \frac14(30+80)=27.5

Ask the user for: possible buyer values, seller costs, their probabilities, and the posted price.

Steps:
1. First best: average the positive gains over all pairs (book: 35).
2. At price p, keep pairs with value >= p >= cost (book: p = 60 keeps only (100, 20), gains 20).
3. Report the shortfall and whether any price reaches the first best (book: 35 - 20 = 15; best prices reach 27.5).

Watch for: the finite example illustrates the theorem; it is not the continuous-type proof.

## 2. Roberts affine-maximizer theorem (roberts-affine-maximizer-theorem)

When to use it: a public choice that weights groups differently.

Equations as the chapter writes them:

    S_F=90+1.5(25)-60=67.5
    S_G=55+1.5(70)-50=110,\qquad S_N=0

Ask the user for: each group's values per option, weights and fixed constants.

Steps:
1. Score each option: weighted sum of values plus its constant (book: 67.5, 110, 0).
2. Pick the highest; find the weight at which the top two tie (book: 30 + 25w = 5 + 70w, w = 0.556).

Watch for: weights must be fixed before reports arrive.

## 3. Strictly proper scoring rules (strictly-proper-scoring-rules)

When to use it: paying forecasters for probability reports.

Equations as the chapter writes them:

    0.65(0.8775)+0.35(0.5775)=0.7725
    0.65q+0.35(1-q)=0.35+0.30q

Ask the user for: the forecaster's belief and the scoring rule.

Steps:
1. Score each outcome for the report (book: 0.8775 and 0.5775 at q = 0.65).
2. Expected score = belief-weighted average (book: 0.7725).
3. Find the report that maximizes it; the rule is proper only if that is the belief (book: quadratic peaks at 0.65, linear at 1).

Watch for: a forecaster with a stake in the outcome can still misreport.

## 4. Vickrey-Clarke-Groves mechanism (vickrey-clarke-groves-mechanism)

When to use it: allocating items or packages and charging each winner its externality.

Equations as the chapter writes them:

    80+75=155>140
    p_Y=140-75=65
    p_Z=140-80=60

Ask the user for: each bidder's package and value.

Steps:
1. Find the welfare-maximizing allocation (book: Y and Z, 155 > 140).
2. For each winner, best welfare without it minus the others' value with it (book: 140 - 75 = 65 and 140 - 80 = 60).
3. Report utilities and revenue (book: 15 each, revenue 125 against value 155).

Watch for: a binding payment budget breaks the benchmark.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
