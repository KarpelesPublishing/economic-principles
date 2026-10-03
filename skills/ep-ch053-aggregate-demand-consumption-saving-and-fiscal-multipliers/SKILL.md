---
name: ep-ch053-aggregate-demand-consumption-saving-and-fiscal-multipliers
description: Apply the principles of Chapter 53 of The Encyclopedia of Economic Principals (Aggregate Demand, Consumption, Saving, and Fiscal Multipliers) to the user's own numbers. Use when judging how much of a bonus, raise or tax cut a household will spend, whether a debt-financed tax cut changes spending, whether more thrift lowers output, or how much a tax-financed spending increase adds to demand.
---

# Chapter 53: Aggregate Demand, Consumption, Saving, and Fiscal Multipliers

These principles say how households spread income over time and how changes in spending feed back into income.

Notebook with the worked examples and figures: `../../notebooks/ch053-aggregate-demand-consumption-saving-and-fiscal-multipliers.ipynb`

## 1. Permanent-income hypothesis (permanent-income-hypothesis)

When to use it: forecasting spending out of a windfall or a raise.

Equation as the chapter writes it:

    C_t=\frac{180{,}000}{4}=45{,}000\text{ dollars}.

Ask the user for: income per period, number of periods, size of the change, whether it lasts, any current need and whether borrowing is possible.

Steps:
1. Add up resources over the horizon (book: 60,000 + 3 x 40,000 = 180,000).
2. Divide by the number of periods (book: 180,000 / 4 = 45,000, a rise of 5,000; 15,000 saved).
3. For a permanent change, consumption rises one for one (book: 240,000 / 4 = 60,000).
4. If a current need exceeds the smoothed level and borrowing is impossible, spend up to the need now (book: 50,000 need, at least 10,000 of the bonus spent).

Watch for: costly credit, risky income and precautionary saving change the split.

## 2. Ricardian equivalence (ricardian-equivalence)

When to use it: judging a tax cut financed by debt that a later tax repays.

Equation as the chapter writes it:

    1.05(1{,}000)=1{,}050\text{ dollars}.

Ask the user for: the cut, the interest rate, and how much the household already wanted to borrow.

Steps:
1. Future tax = (1 + r) x cut (book: 1.05 x 1,000 = 1,050), present value = the cut (book: 1,050 / 1.05 = 1,000).
2. An unconstrained household saves the whole cut; consumption is unchanged.
3. A constrained household spends its desired borrowing and saves the rest (book: 400 spent, 600 saved, 1.05 x 600 = 630).
4. Remaining burden = future tax minus grown saving (book: 1,050 - 630 = 420, worth 400 today).

Watch for: finite lives, redistribution and distortionary taxes break the equivalence.

## 3. Paradox of thrift (paradox-of-thrift)

When to use it: a general rise in saving plans in a slack economy.

Equation as the chapter writes it:

    Y=\frac{20+80}{1-0.8}=500.

Ask the user for: autonomous consumption before and after, the marginal propensity to consume, investment.

Steps:
1. Output Y = (a + I) / (1 - c) (book: 100 / 0.2 = 500; after the cut 90 / 0.2 = 450).
2. Consumption C = a + cY (book: 10 + 0.8 x 450 = 370).
3. Realized saving S = Y - C (book: 450 - 370 = 80, unchanged).
4. Output loss = the cut times 1 / (1 - c) (book: 10 x 5 = 50).

Watch for: if investment rises with saving, output need not fall.

## 4. Balanced-budget multiplier (balanced-budget-multiplier)

When to use it: purchases and taxes rise by the same amount.

Equation as the chapter writes it:

    \frac{1}{1-0.75}(40)=160\text{ million dollars},

Ask the user for: the change in purchases and taxes and the marginal propensity to consume.

Steps:
1. First round = change - c x change (book: 40 - 30 = 10).
2. Rounds sum to first / (1 - c) (book: 10 / 0.25 = 40).
3. Check with the separate effects (book: 160 and -120, net 40).

Watch for: imports, distortionary taxes and differing propensities move the result away from 1.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
