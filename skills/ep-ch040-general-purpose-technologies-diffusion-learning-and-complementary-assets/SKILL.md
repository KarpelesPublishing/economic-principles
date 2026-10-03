---
name: ep-ch040-general-purpose-technologies-diffusion-learning-and-complementary-assets
description: Apply Chapter 40 of The Encyclopedia of Economic Principals (General-Purpose Technologies, Diffusion, Learning, and Complementary Assets) to the user's own numbers. Use when someone forecasts adoption with the Bass model, decides which stage of a process to expand, asks whether more processors pay for a fixed job, or values a staged research pilot for society and for a private funder.
---

# Chapter 40: General-Purpose Technologies, Diffusion, Learning, and Complementary Assets

Trace adoption, find the binding stage, price parallel hardware against time saved, and value research as an option.

Notebook with the worked examples and figures: `../../notebooks/ch040-general-purpose-technologies-diffusion-learning-and-complementary-assets.ipynb`

## 1. Bass diffusion model (bass-diffusion-model)

    dN/dt = (p + q N/m)[m - N],   N* = m(q - p)/(2q),   (0.02 + 0.30 x 0.02)(980) = 25.48

Ask the user for: market potential m, coefficients p and q, current adopters.

Steps:
1. Each period's flow is (p + q N/m)(m - N) (book: 20, then 25.48, then about 32.1).
2. Add the flow to N and repeat.
3. Peak at N* when q > p (book: 1,000 x 0.28 / 0.6 = 466.7). With q = 0 sales only fall (book: 20, 19.6, 19.2).

Watch for: price cuts and quality gains that look like imitation in q.

## 2. Bottleneck relief (bottleneck-relief-general-purpose-methods)

    X <= min_i c_i,   min(18, 10, 15, 20) = 10

Ask the user for: each stage's usable capacity, demand, contribution per unit, cost of each upgrade.

Steps:
1. Throughput = smallest capacity (book: 10, worth 1,200).
2. After an upgrade, recompute the minimum (book: diagnosis 14 gives 14, +480 for 300).
3. Upgrade only if added units x contribution exceed the cost (book: 17 adds one unit, 120 < 150).

Watch for: nameplate capacity instead of usable output after downtime and defects.

## 3. Parallelization economies (parallelization-economies-scale-elasticity)

    T(N) = s + (1 - s)/N,   100(0.20 + 0.80/10) = 28 hours,   10(19.95)($6) = $1,197

Ask the user for: one-processor hours, serial share, communication cost per processor, price per processor-hour, value of an hour saved.

Steps:
1. Runtime W(s + (1 - s)/N) plus communication (book: P with 0.4N, 19.95 and 18.725 hours).
2. Cost N x T x price (book: 1,197 and 2,247).
3. Compare the extra bill with hours saved x value (book: 1,050 against 61.25, uneconomic).

Watch for: communication that grows with N can erase the speedup entirely.

## 4. Knowledge spillovers and option value (public-goods-knowledge-spillovers)

    NPV_option = -C0 + p max{V - C1, 0},   1 - (1 - 0.10)^10 ≈ 65.1%

Ask the user for: pilot cost, success probability, follow-on cost, social value, capturable value.

Steps:
1. Staged value with social V (book: -100,000 + 0.10 x 2,500,000 = 150,000).
2. Staged value with private V (book: -100,000 + 0.10 x 100,000 = -90,000).
3. Compare with committing both costs up front (book: 0.10 x 3,000,000 - 600,000 = -300,000).

Watch for: staging creates no option if the pilot reveals nothing or the follow-on cost cannot be avoided.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
