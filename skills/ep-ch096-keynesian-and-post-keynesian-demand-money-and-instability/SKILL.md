---
name: ep-ch096-keynesian-and-post-keynesian-demand-money-and-instability
description: Apply the principles of Chapter 96 of The Encyclopedia of Economic Principals (Keynesian and Post-Keynesian Demand, Money, and Instability) to the user's own numbers. Use when judging whether a general wage cut raises profits, which spending flows add up to aggregate profit, how far expected demand leaves output below capacity, or how a markup-pricing firm responds to demand and cost shocks.
---

# Chapter 96: Keynesian and Post-Keynesian Demand, Money, and Instability

These principles turn demand-led arguments into small accounting checks: output from spending propensities, profits from spending flows, and prices from normal cost. The chapter's numbers are hypothetical.

Notebook with the worked examples and figures: `../../notebooks/ch096-keynesian-and-post-keynesian-demand-money-and-instability.ipynb`

## 1. Paradox of costs (paradox-of-costs)

When to use it: testing whether an economy-wide wage cut raises aggregate profits.

Equations as the chapter writes them:

    \Pi=(1-\omega)Y.
    60+0.5(40)+20=100,
    Y=0.75Y+20,

Ask the user for: the wage share, spending propensities out of wages and profits, autonomous demand, capacity.

Steps:
1. Spending propensity c = cw omega + cp (1 - omega) (book: 1 x 0.60 + 0.5 x 0.40 = 0.80).
2. Y = A / (1 - c) (book: 20 / 0.20 = 100; at omega 0.50, 20 / 0.25 = 80).
3. Profits = (1 - omega) Y (book: 40 in both cases) and utilization Y / capacity (0.80 against 0.64).

Watch for: debt, prices and foreign demand can change the sign; the result is conditional.

## 2. Kalecki profit equation (kalecki-profit-equation)

When to use it: finding which spending must replace a cut injection if profits are to hold.

Equations as the chapter writes them:

    P=C_c+I+(G-T)+(X-M)-S_w.
    P=40+120+30-10-20=160.

Ask the user for: capitalist consumption, investment, the deficit, net exports, saving out of wages.

Steps:
1. Add injections and subtract worker saving (book: 160).
2. Change one entry at a time (book: deficit 10 gives 140; investment 135 gives 155; worker saving 15 gives 160).
3. Name the offset any forecast relies on.

Watch for: the identity does not say which entry causes which.

## 3. Principle of effective demand (principle-of-effective-demand)

When to use it: estimating output and idle capacity when firms produce for expected sales.

Equations as the chapter writes them:

    D^e(N^*)=Z(N^*).
    Y=20+0.75Y+10,

Ask the user for: autonomous consumption, the marginal propensity to consume, investment, public orders, capacity.

Steps:
1. Y = autonomous spending / (1 - mpc) (book: 30 / 0.25 = 120).
2. Idle capacity = capacity - Y (book: 160 - 120 = 40).
3. Add a credible order (book: 8 gives 152; 10 reaches 160).

Watch for: near capacity, extra demand shows up in prices, not output.

## 4. Administered full-cost pricing (administered-full-cost-pricing)

When to use it: predicting a list price and margin under a normal-cost markup rule.

Equations as the chapter writes them:

    c_n=v_n+\frac{K}{Q_n}, \qquad P=(1+m)c_n.

Ask the user for: direct unit cost, overhead, normal volume, markup, current orders.

Steps:
1. Normal unit cost (book: 60 + 2,000,000 / 100,000 = 80) and price (1.25 x 80 = 100).
2. Actual cost at current orders (book: 60 + 2,000,000 / 70,000 = 88.57; margin 11.43).
3. Cost shocks pass through (book: direct cost 68 gives 110; current-volume overhead would give 120.71).

Watch for: menu costs or contracts can mimic the same price stability.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
