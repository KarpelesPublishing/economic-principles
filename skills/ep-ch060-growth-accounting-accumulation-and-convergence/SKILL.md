---
name: ep-ch060-growth-accounting-accumulation-and-convergence
description: Apply the principles of Chapter 60 of The Encyclopedia of Economic Principals (Growth Accounting, Accumulation, and Convergence) to the user's own numbers. Use when the user asks whether capital deepening will continue, whether an economy saves too much or too little for sustainable consumption, how fast a region should catch up given its own target, or how much of output growth is left after measured inputs.
---

# Chapter 60: Growth Accounting, Accumulation, and Convergence

These principles separate transitions from sustained growth: where accumulation stops, which steady state maximizes consumption, how a region's own target sets its catch-up speed, and what the productivity residual contains.

Notebook with the worked examples and figures: `../../notebooks/ch060-growth-accounting-accumulation-and-convergence.ipynb`

## 1. Solow-Swan convergence mechanism (solow-swan-convergence-mechanism)

When to use it: to tell whether capital per effective worker is rising or falling and where it settles.

Equation as the chapter writes it:

    \dot{k}=s k^\alpha-(n+g+\delta)k
    k^*=\left(\frac{s}{n+g+\delta}\right)^{1/(1-\alpha)}

Ask the user for: saving rate s, capital share alpha, n + g + delta, current capital per effective worker k.

Steps:
1. Steady state k* (book: (0.24 / 0.06)^(1/0.60) = 4^(5/3) = 10.079; y* = 10.079^0.40 = 2.520).
2. Investment s k^alpha at the current k (book, k = 4: 0.24 x 1.741 = 0.418).
3. Break-even (n + g + delta) k (book: 0.06 x 4 = 0.240).
4. k-dot = investment minus break-even and its share of k (book: 0.418 - 0.240 = 0.178, 4.45 percent of k).
5. State the direction: positive means deepening toward k*, negative means thinning toward k*.

Watch for: saving that does not become productive capital, or thresholds that create several steady states.

## 2. Golden rule of accumulation (golden-rule-of-accumulation)

When to use it: to judge whether the maintained capital stock is below or above the consumption-maximizing level.

Equation as the chapter writes it:

    c(k)=f(k)-(n+g+\delta)k
    f'(k_{GR})=n+g+\delta

Ask the user for: the production function (or alpha), n + g + delta, the current stock k.

Steps:
1. Solve f'(k) = n + g + delta (book: 0.40 k^(-0.60) = 0.08, so k_GR = 5^(1/0.60) = 14.620).
2. Consumption at k_GR (book: 2.924 - 1.170 = 1.754; saving rate 1.170 / 2.924 = 0.40).
3. Compare the user's MPK with n + g + delta (book: k = 25 gives MPK 0.058 below 0.08, consumption 1.624).
4. State the verdict: MPK above break-even means below the golden rule, below means over-accumulation.

Watch for: the rule compares steady states only; it ignores the consumption cost of the transition.

## 3. Conditional convergence (conditional-convergence)

When to use it: to predict transition growth from the distance to each economy's own target.

Equation as the chapter writes it:

    g_i\approx\lambda\left[\ln(y_i^*)-\ln(y_{i,0})\right]=\lambda\ln\left(\frac{y_i^*}{y_{i,0}}\right)

Ask the user for: initial income, the conditioned target y*, the convergence parameter lambda and its interval.

Steps:
1. Log gap ln(y* / y0) (book: ln(30,000 / 15,000) = ln 2 = 0.69315).
2. Growth g = lambda x gap (book: 0.15 x 0.69315 = 0.1040, about 10.40 log points; target 18,000 gives 2.73).
3. Compare economies by their own gaps, not by initial income.

Watch for: a negative coefficient on initial income identifies nothing causal unless the targets are handled correctly.

## 4. Solow residual (solow-residual)

When to use it: to split output growth into measured inputs and a remainder.

Equation as the chapter writes it:

    g_A=g_Y-\alpha g_K-(1-\alpha)g_L

Ask the user for: output, capital-service and labor-service growth, and the capital weight alpha.

Steps:
1. Input contribution (book: 0.35(9) + 0.65(1.5) = 3.15 + 0.975 = 4.125).
2. Residual (book: 7 - 4.125 = 2.875 points; exact logs give 0.027819, about 2.78 log points).
3. Rebuild with alternative labor-quality or share assumptions (book: labor 2.5 percent gives 2.225 points).

Watch for: markups, utilization and omitted inputs all land in the residual; it is not a direct invention measure.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
