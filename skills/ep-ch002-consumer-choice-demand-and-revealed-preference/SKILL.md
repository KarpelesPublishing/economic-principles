---
name: ep-ch002-consumer-choice-demand-and-revealed-preference
description: Apply Chapter 2 of The Encyclopedia of Economic Principals (Consumer Choice, Demand, and Revealed Preference) to the user's own numbers. Use when someone wants to split a price change into substitution and income effects, value a price rise in money (compensating or equivalent variation), check whether a staple could be a Giffen good, or decide how many units to add at the margin.
---

# Chapter 2: Consumer Choice, Demand, and Revealed Preference

Split a price change, value it in money, and decide at the margin.

Notebook with the worked examples and figures: `../../notebooks/ch002-consumer-choice-demand-and-revealed-preference.ipynb`

## 1. Slutsky equation (slutsky-equation)

    x(p, m) = m/(2p) for u = sqrt(xy);  dx/dp = dh/dp - x dx/dm  (book: -15 = -7.5 - (30)(0.25))

Steps for a finite rise p0 to p1: ordinary x before and after (book: 30 and 20); Slutsky income m + (p1 - p0) x0 (book: 150) or Hicksian income e(p1, u0) (book: 146.97); compensated x (book: 25 or 24.49); substitution = compensated x - x0, income = x1 - compensated x (book: -5 and -5, or -5.51 and -4.49).

## 2. Hicksian-Marshallian demand duality (hicksian-marshallian-demand-duality)

    e(p, u) = 2u sqrt(p);  CV = e(p1, u0) - m;  EV = m - e(p0, u1)

Steps: u1 = v(p1, m) (book: 35.36); CV (book: 141.42 - 100 = 41.42); EV (book: 100 - 70.71 = 29.29). Say which question each answers: payment to accept the change (CV) or to avoid it (EV).

## 3. Giffen paradox (giffen-paradox)

    eps_M = eps_H - s eta  (book: -0.20 - (0.70)(-0.60) = 0.22)

Ask for the compensated elasticity, budget share s and income elasticity eta. Giffen only if eps_M > 0, that is eta < eps_H / s. The book's numbers are a hypothetical calibration, not study estimates.

## 4. Marginal analysis (marginal-analysis)

Steps: list marginal benefit and marginal cost per unit; net increment = MB - MC (book: 600, 320, 60, -180, -400); add units while the increment is positive (book: 3). Leave out costs no option can recover; include forward consequences such as licences or future savings.

## How to answer

- Write each formula, then the user's numbers, then the result.
- State the utility form you assumed if the user gave none.
- Report ties as ties and name any unit whose net increment is exactly zero.
