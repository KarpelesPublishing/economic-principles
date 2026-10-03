---
name: ep-ch082-exhaustible-resources-biodiversity-and-intergenerational-stewardship
description: Apply Chapter 82 of The Encyclopedia of Economic Principals (Exhaustible Resources, Biodiversity, and Intergenerational Stewardship) to the user's own numbers. Use when someone asks whether to extract a resource now or later, whether a private owner will keep or sell a slow-growing living asset, whether an efficiency gain will really cut resource use, or whether to delay an irreversible project to learn more.
---

# Chapter 82: Exhaustible Resources, Biodiversity, and Intergenerational Stewardship

Treat a deposit, a species or a landscape as an asset and decide on timing: now, later, or after learning.

Notebook with the worked examples and figures: `../../notebooks/ch082-exhaustible-resources-biodiversity-and-intergenerational-stewardship.ipynb`

## 1. Hotelling rule (hotelling-rule)

When to use it: choosing whether to extract a unit now or next period.

    \lambda_t=p_t-c_t;  \lambda_{t+1}=(1+r)\lambda_t

Ask the user for: today's price and marginal cost, expected next-period price and cost, and a comparable risk-adjusted return.

Steps:
1. Today's rent = price - cost (book: $63 after adjustment).
2. Required next-period rent = (1 + r) x today's rent (book: 1.08 x 63 = 68.04).
3. Expected next-period rent = expected price - expected cost (book: 99 - 30.96 = 68.04).
4. Expected above required: postpone; below: extract more now; equal: no shift pays (book at 12 percent: 70.56 > 68.04, extract now).

Watch for: use net rent, not gross price; discoveries, taxes and unpriced damage change the comparison.

## 2. Clark extinction condition (clark-extinction-condition)

When to use it: whether an owner keeps or sells a slow-growing living asset.

    PV_K=\frac{14{,}700}{1.07}=\$13{,}738.32

Ask the user for: sale value today, value of keeping it one more period (growth, offspring, later sale), any survival payment, and the owner's discount rate.

Steps:
1. Present value of keeping = (next-period value + payment) / (1 + r) (book: 14,700 / 1.07 = 13,738.32).
2. Compare with the sale value (book: selling wins by 261.68; at 4 percent keeping wins by 134.62).
3. A payment tied to survival adds to the payoff (book: $900 gives 15,600 / 1.07 = 14,579.44, keeping wins by 579.44).

Watch for: private title alone does not add the unpriced benefits to neighbours.

## 3. Jevons-like demand expansion (jevons-demand-expansion-capex)

When to use it: whether an efficiency gain will cut total resource use.

    R'=R(1-e)(1+g);  \rho=\frac{(1-e)g}{e};  g>\frac{e}{1-e}

Ask the user for: baseline use R, the intensity cut e, and the causal growth in service g.

Steps:
1. Engineering use R(1 - e) (book: 24 x 0.5 = 12).
2. Actual use R' = R(1 - e)(1 + g) (book: 20.4 million kWh).
3. Rebound rho = (1 - e) g / e (book: 0.70); backfire when g > e / (1 - e) (book threshold 1; g = 1.3 gives 27.6, backfire).

Watch for: g must be growth caused by the efficiency change, not trend growth.

## 4. Arrow-Fisher quasi-option value (arrow-fisher-quasi-option-value)

When to use it: delaying an irreversible decision to learn more.

    V_P=8+0.4(230)+0.6(120)=\$172\text{ million}

Ask the user for: value of acting now, value of interim services while waiting, value of acting later, and the probabilities and values of the states a study can reveal.

Steps:
1. Wait and learn: interim + p x high value + (1 - p) x later development (book: 172).
2. Fixed commitment to preserve: interim + p x high + (1 - p) x low (book: 130).
3. Compare both with acting now (book: 140). The gap between the two waiting values is the value of flexibility.

Watch for: the study must be informative, and delay costs must be counted.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied.
- Report ties as ties.
- The chapter's numbers are hypothetical teaching values; never present them as facts about a real resource or species.
