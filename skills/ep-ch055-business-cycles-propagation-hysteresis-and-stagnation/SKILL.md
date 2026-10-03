---
name: ep-ch055-business-cycles-propagation-hysteresis-and-stagnation
description: Apply the principles of Chapter 55 of The Encyclopedia of Economic Principals (Business Cycles, Propagation, Hysteresis, and Stagnation) to the user's own numbers. Use when sizing an investment swing from a change in expected demand, tracing a cycle from one spending shock, judging how long a productivity shock lasts, or estimating how much recession unemployment becomes permanent.
---

# Chapter 55: Business Cycles, Propagation, Hysteresis, and Stagnation

These principles show why investment swings harder than demand, how one shock can produce a cycle, and why some recessions leave lasting damage.

Notebook with the worked examples and figures: `../../notebooks/ch055-business-cycles-propagation-hysteresis-and-stagnation.ipynb`

## 1. Accelerator principle (accelerator-principle)

When to use it: a firm or sector faces a change in expected output and must size capital spending.

Equation as the chapter writes it:

    K_t^* = v Y_t^e,   I_t^g = K_t^* - K_{t-1} + \delta K_{t-1}

Ask the user for: capital-output ratio v, depreciation rate, current capital, old and new expected output, cost per capital unit.

Steps:
1. Desired capital before and after (book: 6 x 8 = 48 and 6 x 9.5 = 57).
2. Adjustment-period investment (book: (57 - 48) + 0.10 x 48 = 13.8 units, $690,000).
3. Following-period investment once the gap closes (book: 0.10 x 57 = 5.7 units, $285,000), and the drop.

Watch for: immediate adjustment is assumed; real firms spread purchases over several periods.

## 2. Multiplier-accelerator interaction (multiplier-accelerator-interaction)

When to use it: tracing how a one-time spending shock moves income over several periods.

Equation as the chapter writes it:

    Y_t = c(1+v) Y_{t-1} - c v Y_{t-2} + A_t

Ask the user for: propensity to consume c, accelerator coefficient v, normal and shocked autonomous spending.

Steps:
1. Steady state A / (1 - c) (book: 24 / 0.5 = 48).
2. Iterate C_t = c Y_{t-1}, I_t = v (C_t - C_{t-1}), Y_t = C_t + I_t + A_t (book: Y2 = 30 + 7.2 + 24 = 61.2).
3. Report the peak, the turning point and any overshoot (book: Y5 = 43.7532).

Watch for: the lags and fixed coefficients are a stripped-down model; negative net investment means disinvestment.

## 3. Real-business-cycle propagation (real-business-cycle-propagation)

When to use it: judging how long a productivity shock keeps output above trend.

Equation as the chapter writes it:

    Y_t^1 / Y_t^0 = 1.04 (1.03)^{0.65} \approx 1.0602

Ask the user for: capital share, the productivity shock now and next period, the labor response, baseline capital, investment and depreciation.

Steps:
1. Current ratio (1 + z)(1 + n)^(1 - alpha) (book: 1.0602).
2. Next-period capital with and without the shock (book: 175.2 and 171.2).
3. Next ratio (1 + z_next)(K1 / K0)^alpha (book: 1.02 x (175.2 / 171.2)^0.35 = 1.0283).

Watch for: the example does not show the shock is typical or efficient; investment of 28 is assumed.

## 4. Hysteresis in unemployment (hysteresis-in-unemployment)

When to use it: estimating how much recession unemployment remains after demand recovers.

Equation as the chapter writes it (the book prints `mathrm` without its backslash in the program case; corrected here):

    u_{t+1}^* = \bar u + \rho (u_t^* - \bar u) + \gamma (u_t - u_t^*)
    u_{1,\mathrm{program}}^* = 5 + (1/12)(12.5 - 5) = 5.625

Ask the user for: labor force, benchmark rate, recession rate, rho and an assumed gamma.

Steps:
1. New equilibrium rate (book: 5 + 0.9 x 0 + 0.25 x 7.5 = 6.875 percent).
2. Unemployed after recovery (book: 0.06875 x 24,000 = 1,650, 450 embedded).
3. Compare a program's lower gamma (book: 1/12 gives 5.625 percent, 1,350).

Watch for: gamma is assumed, not estimated; the law does not say which channel causes the scar.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
