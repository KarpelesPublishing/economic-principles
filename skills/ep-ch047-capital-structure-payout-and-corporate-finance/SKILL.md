---
name: ep-ch047-capital-structure-payout-and-corporate-finance
description: Apply Chapter 47 of The Encyclopedia of Economic Principals (Capital Structure, Payout, and Corporate Finance) to the user's own numbers. Use when someone asks whether to fund a project with cash, debt or new shares, how much debt to carry, why leverage raises the return on equity, or whether a capital project has a positive NPV.
---

# Chapter 47: Capital Structure, Payout, and Corporate Finance

Financing choices move value only through information, taxes, distress and the projects they allow.

Notebook with the worked examples and figures: `../../notebooks/ch047-capital-structure-payout-and-corporate-finance.ipynb`

## 1. Pecking-order theory (pecking-order-theory)

    12 - 10 = 2;  10/0.75 = 13.333;  13.333 - 10 = 3.333

Steps: project NPV (book: 2); claims sold = amount raised / price per dollar of true value (book: 13.33); transfer = claims - amount (book: 3.33); issue equity only if NPV exceeds the transfer. Break-even price = cost / value (book: 0.83). Cash and safe debt have no transfer.

## 2. Trade-off theory of capital structure (trade-off-theory-of-capital-structure)

    100 + 5 - 1 = 104;  104 + 4 - 6 = 102;  104 + 4 - 2 = 106

Steps: for each extra debt slice, add its tax benefit and subtract its expected distress cost; stop at the last slice whose margin is positive (book: one slice, 104). Report a zero margin as indifference.

## 3. Modigliani-Miller leverage proposition (modigliani-miller-leverage-proposition)

    r_E = r_A + (D/E)(r_A - r_D)  (book: 8% + (50/50)(8% - 4%) = 12%; D/E = 3 gives 20%)
    WACC = (E/V) r_E + (D/V) r_D  (book: 8%)

Steps: compute D/E, the equity return, then confirm the weighted return equals the asset return. Without taxes or distress costs, leverage changes the split, not firm value.

## 4. Capital budgeting and NPV (capital-budgeting-npv)

    PV = sum over t of CF_t / (1 + r)^t;  NPV = PV - cost  (book: 1,177,754.25 - 1,000,000 = 177,754.25)

Steps: list after-tax incremental cash by date, including salvage; discount at a risk-adjusted rate; accept if NPV > 0 (book at 280,000 a year: NPV -44,136.33, reject).

## How to answer

- Write each formula, then the user's numbers, then the result.
- Report exact ties as ties.
- The chapter's numbers are hypothetical; never present them as data.
