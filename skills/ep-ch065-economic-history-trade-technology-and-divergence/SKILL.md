---
name: ep-ch065-economic-history-trade-technology-and-divergence
description: Apply the principles of Chapter 65 of The Encyclopedia of Economic Principals (Economic History, Trade, Technology, and Divergence) to the user's own numbers. Use when pricing whether a labor-saving machine pays under local wages and energy prices, building a land-equivalent resource balance with coal or import relief, checking whether collective liability makes a contract enforceable, or estimating social savings of a transport improvement against a named alternative.
---

# Chapter 65: Economic History, Trade, Technology, and Divergence

These principles turn historical arguments into explicit calculations: an adoption test, a resource balance, an enforcement chain and a counterfactual saving. The book's examples are invented teaching numbers, not historical data.

Notebook with the worked examples and figures: `../../notebooks/ch065-economic-history-trade-technology-and-divergence.ipynb`

## 1. High-wage, cheap-energy mechanization (high-wage-cheap-energy-mechanization)

When to use it: deciding whether one machine design pays under different wages and energy prices.

Equations as the chapter writes them:

    G=wL_s-p_eE-M
    A_T=\frac{1-(1+r)^{-T}}{r}
    NPV=GA_T-F>0
    w^*=\frac{F/A_T+p_eE+M}{L_s}

Ask the user for: machine cost F, hours saved per year, energy use, maintenance, life in years, discount rate, wage and energy price.

Steps:
1. Annuity factor (book: (1 - 1.08^-5) / 0.08 = 3.992710).
2. Annual gain (book: 11 x 720 - 0.80 x 600 - 480 = 6,960).
3. NPV (book: 6,960 x 3.992710 - 9,600 = 18,189.26; region L: 1,680 x 3.992710 - 9,600 = -2,892.25).
4. Threshold wage (book: (9,600 / 3.992710 + 480 + 480) / 720 = 4.67) and state the decision.

Watch for: credit limits, reliability risk and transport costs make the market wage and fuel price poor guides.

## 2. Great Divergence coal-and-colonies hypothesis (great-divergence-coal-and-colonies-hypothesis)

When to use it: testing whether resource relief lets a proposed scale fit within local land.

Equations as the chapter writes them:

    D_t=F_t+B_t-C_t-X_t
    D_t\leq \bar L

Ask the user for: land capacity, land needs by use, and each relief channel in land-equivalents.

Steps:
1. Gross need (book: 98 + 62 = 160).
2. Subtract relief (book: 160 - 14 - 11 = 135).
3. Compare with land (book: 140 - 135 = 5 slack; coal only deficit 6; imports only deficit 9).

Watch for: conversion factors are uncertain; report ranges, and note relief can shift costs elsewhere.

## 3. Community responsibility system (community-responsibility-system)

When to use it: checking whether collective liability makes a remote trading partner perform.

Equations as the chapter writes them:

    U_D=g-f
    f\geq g

Ask the user for: gain from default, private recovery probability and penalty, group fine, group enforcement cost k and outside sanction S.

Steps:
1. Private remedy payoff (book: 18 - 0.15 x 40 = 12).
2. Group fine payoff (book: 18 - 24 = -6).
3. Credibility: enforce only if k <= S (book: 9 < 60 enforces; 9 > 7 does not).

Watch for: verification errors and collateral punishment of innocent members.

## 4. Railroad social savings (railroad-social-savings)

When to use it: valuing a transport improvement against a named feasible alternative.

Equations as the chapter writes them:

    SS_0=(c_C-c_R)Q
    SS=(c_C-c_R)Q_C+\frac{1}{2}(c_C-c_R)(Q_R-Q_C)

Ask the user for: unit costs under both systems and traffic under each.

Steps:
1. Cost gap (book: 0.07 - 0.04 = 0.03).
2. Rectangle (book: 0.03 x 7,000,000 = 210,000) and triangle (book: 0.5 x 0.03 x 3,000,000 = 45,000).
3. Compare with the fixed-demand estimate (book: 300,000, overstating by 45,000).

Watch for: a static comparison omits settlement and innovation effects, and the alternative changes by date.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real place or period.
