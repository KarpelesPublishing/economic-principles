---
name: ep-ch066-tax-incidence-elasticity-salience-and-revenue
description: Apply Chapter 66 of The Encyclopedia of Economic Principals (Tax Incidence, Elasticity, Salience, and Revenue) to the user's own numbers. Use when someone asks how a tax shown separately at checkout changes purchases and revenue, who really pays a per-unit tax in the short and long run, whether cutting a tax rate could raise revenue, or whether to contract out tax collection for a fixed fee or run it directly with monitoring.
---

# Chapter 66: Tax Incidence, Elasticity, Salience, and Revenue

Work out who bears a tax, how much it raises once buyers and the base respond, and who should collect it.

Notebook with the worked examples and figures: `../../notebooks/ch066-tax-incidence-elasticity-salience-and-revenue.ipynb`

## 1. Tax salience (tax-salience)

When to use it: a tax is added at the register or shown apart from the shelf price.

    q = 90 - 2 p-tilde,  p-tilde = p + theta t,  R = t q

Ask the user for: the pretax price, the per-unit tax, a demand line and the share theta of the tax buyers notice.

Steps:
1. Decision price p + theta t (book: 30 + 0.25(6) = 31.5).
2. Quantity from demand at the decision price (book: 90 - 2(31.5) = 27).
3. Revenue t q (book: 6(27) = 162); repeat at higher attention (book theta 0.75: 34.5, 21, 126, a fall of 36).

Watch for: the pretax price is held fixed; with responsive supply it would move too.

## 2. Tax incidence and elasticity (tax-incidence-and-elasticity)

When to use it: deciding who pays a per-unit tax.

    Q_D = 180 - 3 p_b,  Q_S = 30 + p_s,  180 - 3(p_s + 8) = 30 + p_s

Steps: solve demand(p_s + t) = supply(p_s) (book: p_s = 31.5, p_b = 39.5, Q = 61.5); burdens are the price changes from the pretax price (book: buyers 2, sellers 6, buyer share 1/4); revenue t Q (book: 492). Redo with the long-run supply (book -45 + 3p_s: 33.5, 41.5, 55.5, shares 1/2, revenue 444).

Watch for: the side that adjusts quantity more easily bears less, whoever remits the tax.

## 3. The Laffer curve and the tax base (laffer-curve-and-tax-base)

When to use it: a claim that a rate cut raises revenue.

    B_H(t) = 1200(1 - 0.8t),  eps_B(0.80) = 0.80(960)/432 = 16/9 > 1

Steps: base B(t) and revenue t B(t) (book: 432 and 345.6 at t = 0.80); base elasticity t (dB/dt magnitude) / B (book: 16/9); a cut raises revenue only if the elasticity exceeds 1 (book: 375 at the peak t = 0.625, a gain of 29.4). With the weaker base 1200(1 - 0.4t) revenue keeps rising to 720 at t = 1.

Watch for: two sensitivities are two different curves; one observed rate does not locate either.

## 4. Tax farming and the principal-agent problem (tax-farming-principal-agent)

When to use it: a fixed-fee concession against salaried, monitored collection.

    E[Y_H] = 0.5(130) + 0.5(170) = 150;  150 - 110 - 12 = 28;  150 - 15 - 30 = 105

Steps: check the farmer's effort choice (book: high effort 28 beats low effort 10); state receipts per arrangement (book: salary 105, farm 110, monitored 150 - 15 - m); find the monitoring cost that ties the farm (from the book's numbers, 150 - 15 - m = 110 gives m = 25, a value the book does not print; book: at m = 12 monitored nets 123).

Watch for: receipts are not the only criterion; taxpayer harm and renegotiation can reverse the ranking.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
