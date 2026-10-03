---
name: ep-ch061-endogenous-growth-ideas-human-capital-and-innovation
description: Apply the principles of Chapter 61 of The Encyclopedia of Economic Principals (Endogenous Growth, Ideas, Human Capital, and Innovation) to the user's own numbers. Use when judging whether more research effort raises growth or only the level of technology, how faster innovation affects growth and incumbent value, how team sorting and training pay under weakest link production, or how a saving change plays out when returns to capital do not diminish.
---

# Chapter 61: Endogenous Growth, Ideas, Human Capital, and Innovation

These principles separate policies that change the growth rate from those that change only the level, and show how innovation, team quality and saving feed growth.

Notebook with the worked examples and figures: `../../notebooks/ch061-endogenous-growth-ideas-human-capital-and-innovation.ipynb`

## 1. Semi-endogenous growth (semi-endogenous-growth)

When to use it: a research subsidy or larger research workforce is proposed.

Equations as the chapter writes them:

    g_A=\frac{0.025(144)}{\sqrt{8{,}100}}=\frac{3.6}{90}=0.04
    g_A^*=\frac{1(0.02)}{1-0.5}=0.04
    2^{\lambda/(1-\phi)}=2^{1/0.5}=4

Ask the user for: research productivity delta, research labor L_A, knowledge stock A, lambda, phi, research labor growth n.

Steps:
1. Current growth g_A = delta L_A^lambda / A^(1 - phi) (book: 0.025 x 144 / 90 = 0.04).
2. Balanced growth g* = lambda n / (1 - phi) (book: 0.02 / 0.5 = 0.04).
3. A one-time change in L_A by a factor m raises impact growth by m and the long-run level of A by m^(lambda / (1 - phi)) (book: 2^2 = 4), while g* is unchanged.

Watch for: the result needs phi below 1; with phi = 1 the model becomes fully endogenous and scale effects return.

## 2. Schumpeterian quality-ladder growth (schumpeterian-quality-ladder-growth)

When to use it: judging the growth and incumbent effects of faster innovation.

Equations as the chapter writes them:

    g_A=0.10\ln(1.20)\approx0.018232
    V=\frac{15}{0.05+0.10}=100

Ask the user for: arrival rate lambda, step size gamma, leader profit, interest rate r.

Steps:
1. Growth g = lambda ln(gamma) (book: 0.10 x 0.182322 = 1.823 percent).
2. Leader value V = profit / (r + lambda) (book: 15 / 0.15 = 100; at lambda 0.15, 75).
3. State both effects: higher growth, shorter and less valuable leadership.

Watch for: welfare cannot be read from the arrival rate alone; fiscal cost and business stealing are outside.

## 3. O-ring production function (o-ring-production-function)

When to use it: deciding how to group workers or where training pays most when one failure spoils output.

Equations as the chapter writes them:

    120(0.90)(0.60)=64.8
    140.4-129.6=10.8

Ask the user for: scale Bn, worker qualities, the training increase.

Steps:
1. Team output = Bn x product of qualities (book: 120 x 0.90 x 0.60 = 64.8).
2. Compare mixed and sorted totals; the gain is Bn(h - l)^2 (book: 120 x 0.09 = 10.8).
3. Training gain = Bn x partner quality x increase (book: 16.2 beside 0.90, 10.8 beside 0.60).

Watch for: the multiplicative form is an assumption; with additive production sorting gains vanish.

## 4. AK endogenous-growth mechanism (ak-endogenous-growth-mechanism)

When to use it: a claim that more saving or investment raises growth permanently.

Equations as the chapter writes them:

    g_y=(0.24)(0.25)-0.035-0.005=0.02
    y_{10}=50e^{0.02(10)}=50e^{0.20}\approx61.07

Ask the user for: saving rate s, productivity A, depreciation delta, population growth n, starting output, horizon.

Steps:
1. g = s A - delta - n (book: 0.30 x 0.25 - 0.04 = 0.035).
2. y_T = y_0 e^(g T) for each saving rate (book: 70.95 against 61.07 at ten years).
3. Report the gap and note that it widens with the horizon.

Watch for: with diminishing returns the growth difference shrinks during convergence.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
