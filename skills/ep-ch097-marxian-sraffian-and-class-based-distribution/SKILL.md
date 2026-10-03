---
name: ep-ch097-marxian-sraffian-and-class-based-distribution
description: Apply the principles of Chapter 97 of The Encyclopedia of Economic Principals (Marxian, Sraffian, and Class-Based Distribution) to the user's own numbers. Use when computing a rate of surplus value from hours and wages, tracing a one-good wage-profit frontier, finding prices of production under a common profit rate with unequal wages, or checking whether a rising composition of capital lowers the profit rate.
---

# Chapter 97: Marxian, Sraffian, and Class-Based Distribution

These principles are value and price accounting: split the working day, divide a surplus between wages and profits, and spread surplus at a common rate. The chapter's numbers are hypothetical, not estimates.

Notebook with the worked examples and figures: `../../notebooks/ch097-marxian-sraffian-and-class-based-distribution.ipynb`

## 1. Surplus value and exploitation (surplus-value-and-exploitation)

When to use it: splitting a working day into necessary and surplus labor.

Equation as the chapter writes it:

    v=mh,\qquad s=m(L-h),\qquad \frac{s}{v}=\frac{L-h}{h}.

Ask the user for: new value per hour m, the daily wage, the length of the day, constant capital.

Steps:
1. Necessary hours h = wage / m (book: 120 / 30 = 4).
2. Surplus s = m (L - h) (book: 30 x 4 = 120) and s / v (100 percent; 150 percent at 10 hours).
3. Batch value c + v + s (book: 300 + 240 = 540).

Watch for: one firm's productivity gain does not lower systemwide necessary labor.

## 2. Sraffian wage-profit frontier (sraffian-wage-profit-frontier)

When to use it: reading the trade-off between a real wage and the profit rate for a given technique.

Equations as the chapter writes them:

    p=(1+r)pA+wl.
    100=(1+r)50+100w_g.

Ask the user for: output, input advanced, labor hours, the real wage.

Steps:
1. Profit = output - input - labor x wage (book: 100 - 50 - 20 = 30).
2. r = profit / input (book: 60 percent; 30 percent at w = 0.35; 0 at w = 0.50).
3. A new technique shifts the frontier (book: input 40, w = 0.35 gives 62.5 percent).

Watch for: with many goods, prices change along the frontier too.

## 3. Unequal exchange (unequal-exchange)

When to use it: computing prices of production when capital earns a common rate but wages differ.

Equation as the chapter writes it:

    p_i=c_i+v_i+rK_i,

Ask the user for: each sector's constant capital, wage bill and new value.

Steps:
1. Surplus s = new value - v (book: 40 and 20).
2. r = total surplus / total capital (book: 60 / 120 = 50 percent).
3. Prices (1 + r) K (book: 75 and 105, ratio 1.4; equal wages give 90 and 90).

Watch for: the value categories themselves are disputed.

## 4. Tendency of the rate of profit to fall (tendency-of-the-rate-of-profit-to-fall)

When to use it: checking whether automation lowers the profit rate.

Equation as the chapter writes it:

    r=\frac{s}{c+v}=\frac{s/v}{c/v+1}.

Ask the user for: constant capital, variable capital, surplus value before and after.

Steps:
1. k = c / v and e = s / v (book: 9 and 2 after automation).
2. r = s / (c + v) (book: 30 / 150 = 20 percent; 24 gives 16 percent; c = 105 gives 25 percent).
3. Compare with the baseline (book: 20 / 100 = 20 percent).

Watch for: cheaper machinery and faster turnover offset rising composition.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as estimates for any real economy.
