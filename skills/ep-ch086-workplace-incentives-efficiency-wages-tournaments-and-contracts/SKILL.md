---
name: ep-ch086-workplace-incentives-efficiency-wages-tournaments-and-contracts
description: Apply the principles of Chapter 86 of The Encyclopedia of Economic Principals (Workplace Incentives, Efficiency Wages, Tournaments, and Contracts) to the user's own numbers. Use when checking whether a wage premium and monitoring deter shirking, computing a no-shirking wage floor, testing back-loaded pay as a bond, or judging how a prize spread changes effort and sabotage.
---

# Chapter 86: Workplace Incentives, Efficiency Wages, Tournaments, and Contracts

These principles compare the gain from shirking or gaming with the expected cost a pay scheme attaches to it. The chapter's numbers are hypothetical teaching values.

Notebook with the worked examples and figures: `../../notebooks/ch086-workplace-incentives-efficiency-wages-tournaments-and-contracts.ipynb`

## 1. Efficiency-wage discipline mechanism (efficiency-wage-discipline-mechanism)

When to use it: checking whether the threat of dismissal makes effort worthwhile.

Equations as the chapter writes them:

    qR\geq c.
    R=3(500)=1{,}500\text{ units}.

Ask the user for: effort cost, detection probability, wage premium, expected jobless spell.

Steps:
1. Rent R = premium x jobless months (book: 3 x 500 = 1,500).
2. Expected forfeiture qR (book: 0.20 x 1,500 = 300).
3. Effort if qR >= c (book: 300 = 300, just binds; one month gives 100 and fails).

Watch for: full employment shrinks the rent toward zero.

## 2. No-shirking efficiency wage (no-shirking-efficiency-wage)

When to use it: computing the lowest wage that prevents shirking.

Equations as the chapter writes them:

    w\geq b+c+\frac{(r+s+a)c}{q}.
    w_{NS}=36+4+\frac{(0.05+0.10+0.50)4}{0.25}=50.4.

Ask the user for: value of unemployment, effort cost, discount, separation and job-finding rates, detection hazard.

Steps:
1. Rent term (r + s + a) c / q (book: 0.65 x 4 / 0.25 = 10.4).
2. w_NS = b + c + rent term (book: 50.4; q 0.50 gives 45.2; a 1.00 gives 58.4).
3. Compare with the job's value (book: 58.4 exceeds 54, so the simple contract fails).

Watch for: risk neutrality and the stated value equations.

## 3. Deferred-compensation bonding (deferred-compensation-bonding)

When to use it: testing whether back-loaded pay deters shirking.

Equations as the chapter writes them:

    c\leq q\left(V_{t+1}-V_{t+1}^{out}\right).
    0.25(15{,}000)=3{,}750\text{ units}.

Ask the user for: pay path, outside pay, detection probability, effort cost saved.

Steps:
1. Claim at stake = remaining promised pay - outside path (book: 135,000 - 120,000 = 15,000).
2. Expected forfeiture = q x claim (book: 3,750).
3. Effort if it covers the effort saved (book: 3,750 > 3,000; q = 0.10 gives 1,500 and fails).

Watch for: the firm's promise to pay the late premium must itself be credible.

## 4. Tournament incentives (tournament-incentives)

When to use it: judging how a prize spread changes productive effort and sabotage.

Equations as the chapter writes them:

    \Delta W\frac{\partial\Pr(i\text{ wins})}{\partial e_i},
    0.10(8{,}000)=800\text{ units}.

Ask the user for: prize spread, each action's cost and its effect on the chance of winning.

Steps:
1. Return of each action = slope x spread (book: 0.10 x 8,000 = 800 against 600).
2. Repeat for harmful actions (book: sabotage 0.03 x 8,000 = 240 against 300).
3. Recheck after widening the spread (book: at 16,000 sabotage returns 480 and pays).

Watch for: the private return ignores the harm (book: 1,000 units of customer value).

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real firm.
