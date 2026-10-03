---
name: ep-ch025-multitask-team-career-concern-and-robust-contracts
description: Apply the principles of Chapter 25 of The Encyclopedia of Economic Principals (Multitask, Team, Career-Concern, and Robust Contracts) to the user's own numbers. Use when estimating effort driven by reputation, checking whether paying for a measured task crowds out unmeasured work, setting the slope of a commission under noisy output, or judging whether a supplier will hide capacity from a buyer who raises targets.
---

# Chapter 25: Multitask, Team, Career-Concern, and Robust Contracts

These principles tell the user how incentives work beyond the explicit contract: through reputation, competing tasks, noise and future targets.

Notebook with the worked examples and figures: `../../notebooks/ch025-multitask-team-career-concern-and-robust-contracts.ipynb`

## 1. Career-concerns incentives (career-concerns-incentives)

When to use it: effort is rewarded only through what the market infers about ability.

Equations as the chapter writes them:

    \beta=\frac{1}{1+1}=0.5
    \frac{0.45^2}{2}=0.10125
    \beta=\frac{1/3}{1+1/3}=0.25

Ask the user for: prior ability variance, noise variance, discount factor, effort cost curve.

Steps:
1. beta = ability variance / (ability variance + noise variance) (book: 1 / 2 = 0.5).
2. With cost e^2/2, effort = delta x beta (book: 0.9 x 0.5 = 0.45).
3. Effort cost = e^2 / 2 (book: 0.10125); redo with the later variance (book: 1/3 gives 0.225).

Watch for: the incentive vanishes if effort becomes observable.

## 2. Multitask incentive problem (multitask-incentive-problem)

When to use it: one task is measured and paid, another is not, and the two compete for effort.

Equations as the chapter writes them:

    u=bx+4y-\frac12(x^2+y^2)-0.5xy
    x+0.5y=4,  y+0.5x=4
    2(20/3)+10(2/3)=20

Ask the user for: reward per unit on each task, how strongly the tasks compete (rho), value per unit to the firm.

Steps:
1. Solve x + rho y = b and y + rho x = 4, the return on diagnostic effort (book: b = 4 gives x = y = 8/3).
2. Gross value = vx x + vy y (book: 2 x 8/3 + 10 x 8/3 = 32).
3. Repeat at the new reward (book: b = 7 gives 20/3 and 2/3, value 20; with rho = 0 value rises 48 to 54).

Watch for: the book writes the cross term as a fixed 0.5xy and then sets rho = 0 for its counterfactual.

## 3. Linear-contract robustness (linear-contract-robustness)

When to use it: setting the slope of linear pay when output is noisy and the agent is risk averse.

Equations as the chapter writes them:

    S(b)=b-\frac12b^2-\frac12(0.05)(16)b^2=b-0.9b^2
    S(b)=b-0.5b^2-0.1b^2=b-0.6b^2

Ask the user for: residual variance of output, risk aversion r.

Steps:
1. b* = 1 / (1 + r x variance) (book: 1 / 1.8 = 0.556).
2. Effort cost = b*^2 / 2 and risk premium = r x variance x b*^2 / 2 (book: 0.154 and 0.123).
3. Surplus = b* / 2 (book: 0.278; the book's rounded parts sum to 0.279).

Watch for: assumes CARA utility, normal noise and quadratic effort cost.

## 4. Ratchet effect (ratchet-effect)

When to use it: a buyer sets tomorrow's target from today's performance.

Equations as the chapter writes them:

    15+0.9(4)=18.6
    5+0.9(20)=23
    15+0.9(20)=33

Ask the user for: payoff now from revealing and concealing, continuation payoffs, discount factor, whether the buyer can commit.

Steps:
1. Reveal = now payoff + delta x continuation after revealing (book: 15 + 0.9 x 4 = 18.6).
2. Conceal = now payoff + delta x continuation after concealing (book: 5 + 0.9 x 20 = 23).
3. Threshold delta = gain now / future loss (book: 10 / 16 = 0.625); with commitment reveal gives 33.

Watch for: assumes the buyer reads capacity exactly from delivery.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
