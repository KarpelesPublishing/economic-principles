---
name: ep-ch095-insurance-education-poverty-and-targeting
description: Apply the principles of Chapter 95 of The Encyclopedia of Economic Principals (Insurance, Education, Poverty, and Targeting) to the user's own numbers. Use when deciding whether an unemployment benefit should rise, whether an enrollment burden screens the intended people, how a categorical tag's errors change cost and what reaches the target group, or how much of a public program's enrollment is new coverage.
---

# Chapter 95: Insurance, Education, Poverty, and Targeting

These principles weigh insurance value against behavioral cost and test whether targeting devices reach the intended people. The chapter's numbers are hypothetical teaching values, not estimates from real programs.

Notebook with the worked examples and figures: `../../notebooks/ch095-insurance-education-poverty-and-targeting.ipynb`

## 1. Baily-Chetty optimal unemployment-insurance formula (baily-chetty-optimal-unemployment-insurance-formula)

When to use it: judging locally whether a benefit should rise.

Equations as the chapter writes them:

    \varepsilon_{D,b}=\frac{b}{D}\frac{dD}{db}.
    \frac{3{,}000-2{,}400}{3{,}000}=0.20.

Ask the user for: consumption employed and unemployed, risk aversion, and the duration response to a benefit change.

Steps:
1. Drop = (c_e - c_u) / c_e (book: 0.20).
2. Smoothing index = gamma x drop (book: 0.40).
3. Elasticity = percent change in duration / percent change in benefit (book: 0.05 / 0.10 = 0.50).
4. Raise only if the smoothing index exceeds the elasticity (book: 0.40 < 0.50, do not raise; at 2,100 the index is 0.60).

Watch for: the simplified comparison omits prudence, unemployment share, match quality and equilibrium effects.

## 2. Ordeal mechanism (ordeal-mechanism)

When to use it: checking whether a hassle or requirement screens in the intended group.

Equation as the chapter writes it:

    B_i-c_i(z)\geq 0.

Ask the user for: the benefit's value and the burden for each group, group sizes, and program cost per recipient.

Steps:
1. Net value = value - burden for each group (book: 180 - 100 = 80, 80 - 100 = -20).
2. Groups with nonnegative net value enroll; transfers = enrollees x cost (book: 12,000).
3. Ordeal cost = enrollees x burden (book: 10,000).

Watch for: burdens that fall hardest on the needy screen the wrong way (book: 190 and 60 give -10 and 20).

## 3. Akerlof tagging principle (akerlof-tagging-principle)

When to use it: comparing a categorical payment with a universal one.

Arithmetic as the chapter writes it (inline):

    0.75(400)=300
    0.10(600)=60
    540(8{,}000)=4{,}320{,}000

Ask the user for: target and non-target group sizes, the tag's hit and false-positive rates, and both payment levels.

Steps:
1. Tagged = hit rate x target + false-positive rate x others (book: 300 + 60 = 360).
2. Cost = tagged x payment (book: 2,880,000); target receipts = hits x payment (book: 2,400,000).
3. Compare with the universal rule (book: 4,000,000 and 1,600,000).

Watch for: resources spent to obtain the tag are waste, distinct from transfers.

## 4. Public-insurance crowd-out (public-insurance-crowd-out)

When to use it: measuring the net coverage gain from a public expansion.

Equation as the chapter writes it:

    G=300+60+320=680.

Ask the user for: enrollees who left private coverage and enrollees who were uninsured.

Steps:
1. G = switchers + uninsured take-up (book: 680).
2. P = switchers; N = G - P (book: 360 and 320).
3. Crowd-out = P / G (book: 0.529).

Watch for: enrollment alone hides displaced private coverage.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as estimates from any real program.
