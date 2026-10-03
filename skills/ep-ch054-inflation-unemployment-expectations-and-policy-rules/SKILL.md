---
name: ep-ch054-inflation-unemployment-expectations-and-policy-rules
description: Apply the principles of Chapter 54 of The Encyclopedia of Economic Principals (Inflation, Unemployment, Expectations, and Policy Rules) to the user's own numbers. Use when someone asks what inflation it takes to hold unemployment below its natural rate, what a Taylor rule prescribes, how fast sticky prices adjust, or how postponed money creation interacts with public debt.
---

# Chapter 54: Inflation, Unemployment, Expectations, and Policy Rules

These principles show what monetary policy can and cannot buy once expectations, rules, price stickiness and the government budget are written down.

Notebook with the worked examples and figures: `../../notebooks/ch054-inflation-unemployment-expectations-and-policy-rules.ipynb`

## 1. Natural-rate hypothesis (natural-rate-hypothesis)

When to use it: someone wants unemployment held below its natural rate.

Equation as the chapter writes it:

    \pi_t=\pi_t^e-\alpha(u_t-u_t^n)+s_t,

Ask the user for: natural rate, target unemployment, alpha, starting expected inflation.

Steps:
1. Each year, pi = expected pi - alpha (u - u_n) (book: 2 - (4 - 5) = 3).
2. Set next year's expected inflation to this year's pi and repeat (book: 3, 4, 5).
3. If inflation stops rising, solve pi = pi_e - alpha(u - u_n) for u (book: 4 = 4 - (u3 - 5), u3 = 5).

Watch for: the result depends on fully adaptive expectations and a known natural rate.

## 2. Taylor rule (taylor-rule)

When to use it: benchmarking a policy rate against inflation and the output gap.

Equation as the chapter writes it:

    i_t=r^*+\pi_t+a(\pi_t-\pi^*)+b x_t.

Ask the user for: inflation, output gap, neutral real rate r*, inflation target, weights a and b.

Steps:
1. i = r* + pi + a(pi - target) + b x (book: 2 + 3 + 0.5 + 1 = 6.5).
2. Compare with the baseline and with the actual rate (book: 2.5 points above 4).
3. Report the real rate i - pi (book: 3.5).

Watch for: r* and potential output are estimates; the weights are illustrations.

## 3. Calvo staggered pricing (calvo-staggered-pricing)

When to use it: estimating how fast a cost change reaches the average price.

Equation as the chapter writes it:

    P_2=0.5625(100)+0.4375(108)=103.50

Ask the user for: probability theta a firm cannot reset, old and new desired prices, periods.

Steps:
1. Share still at the old price after k periods = theta^k (book: 0.75^2 = 0.5625).
2. P_k = theta^k (old) + (1 - theta^k)(new) (book: 103.50).
3. Compare with the halfway point to judge speed.

Watch for: the linear average is an approximation to the model's exact index.

## 4. Unpleasant monetarist arithmetic (unpleasant-monetarist-arithmetic)

When to use it: a central bank tightens while the fiscal deficit continues.

Equation as the chapter writes it:

    B_t=(1+r)B_{t-1}+D_t-S_t,

Ask the user for: starting debt, real rate, primary deficit, seigniorage plans, debt ceiling.

Steps:
1. Roll debt forward with the reduced seigniorage (book: 1.10(100) + 5 = 115).
2. Compute next year's need before seigniorage (book: 1.10(115) + 5 = 131.5).
3. Seigniorage to stay under the ceiling and to return to the baseline path (book: 1.5 and 21).

Watch for: a future primary surplus or growth above the real rate changes the conclusion.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
