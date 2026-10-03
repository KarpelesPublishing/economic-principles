---
name: ep-ch067-optimal-commodity-income-and-capital-taxation
description: Apply Chapter 67 of The Encyclopedia of Economic Principals (Optimal Commodity, Income, and Capital Taxation) to the user's own numbers. Use when someone asks how much a tax on interest costs a long-horizon saver, how to set commodity tax rates from demand elasticities, how large a transfer from high to low earners survives the incentive to mimic, or what discount rate to use for a long-lived public project and whether it passes.
---

# Chapter 67: Optimal Commodity, Income, and Capital Taxation

Decide where taxes do least harm: across goods, across people and across time.

Notebook with the worked examples and figures: `../../notebooks/ch067-optimal-commodity-income-and-capital-taxation.ipynb`

## 1. Chamley-Judd zero long-run capital-tax result (chamley-judd-zero-long-run-capital-tax-result)

When to use it: judging a recurring tax on interest for savers with long horizons.

    1,500(1.045)^35 approx 7,001.02;  0.045(1 - 0.25) = 0.03375;  1,500(1.03375)^35 approx 4,793.30

Ask the user for: the amount saved, the pre-tax return, the tax rate on interest and the horizon.

Steps:
1. Net return r(1 - tau) (book: 0.03375).
2. Values with and without the tax (book: 7,001.02 and 4,793.30 at 35 years).
3. Shortfall 1 - taxed/untaxed (book: 31.53%; 10.26% at 10 years).

Watch for: the result concerns the compounding wedge; it does not show the replacement tax is costless.

## 2. Ramsey inverse-elasticity rule (ramsey-inverse-elasticity-rule)

When to use it: setting rates on unrelated goods to raise revenue with least distortion.

    Delta q_i^c / q_i approx eps_i^c tau_i;  tau_b = 0.012/0.40 = 0.03;  tau_d = 0.012/1.20 = 0.01

Steps: pick a common contraction; each rate is the contraction divided by the elasticity's size (book: 0.03 and 0.01); revenue is unit tax times new quantity summed (book: 0.60(988) + 0.40(494) = 790.4).

Watch for: the rule ignores distribution and cross-effects; it does not by itself recommend taxing necessities.

## 3. Mirrlees optimal-income-tax tradeoff (mirrlees-optimal-income-tax-tradeoff)

When to use it: checking whether a proposed transfer survives the high earner's option to earn less.

    78,000 - x >= 44,000 + x;  x <= 17,000

Steps: honest high-type utility (book: 96,000 - x - 18,000); mimicking utility (book: 48,000 + x - 4,000); the cap where they are equal (book: 17,000; a proposed 18,000 gives 60,000 against 62,000 and fails).

Watch for: two types and quasi-linear utility; participation and wage effects are left out.

## 4. Ramsey social-discounting rule (ramsey-social-discounting-rule)

When to use it: discounting distant public benefits.

    r = 0.8% + 1.4(1.8%) = 3.32%;  PV = 120/(1.0332)^35 approx 38.26

Steps: r = rho + eta g (book: 3.32%); PV of the benefit (book: 38.26 against a cost of 45, fails); redo at other growth rates (book g = 0.4%: 1.36%, 74.79, passes; g = -1%: r = -0.6%, the book gives no PV).

Watch for: the verdict moves with g and eta; report it for a range rather than one rate.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
