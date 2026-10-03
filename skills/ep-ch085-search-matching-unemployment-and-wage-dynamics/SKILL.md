---
name: ep-ch085-search-matching-unemployment-and-wage-dynamics
description: Apply the principles of Chapter 85 of The Encyclopedia of Economic Principals (Search, Matching, Unemployment, and Wage Dynamics) to the user's own numbers. Use when testing whether sorting workers to firms raises output, computing job-finding rates and steady unemployment from a matching function, telling a move along the Beveridge curve from a shift, or analysing employer wage-setting power and wage floors.
---

# Chapter 85: Search, Matching, Unemployment, and Wage Dynamics

These principles quantify matching frictions and employer power in the labor market. The chapter's numbers are hypothetical teaching values.

Notebook with the worked examples and figures: `../../notebooks/ch085-search-matching-unemployment-and-wage-dynamics.ipynb`

## 1. Assortative matching (assortative-matching)

When to use it: deciding whether pairing the best workers with the best firms raises total output.

Equations as the chapter writes them:

    F(s_H,q_H)+F(s_L,q_L)>F(s_H,q_L)+F(s_L,q_H).
    4(3)+1(2)=14,
    4(2)+1(3)=11.

Ask the user for: two skill levels, two firm qualities, the output function.

Steps:
1. Sorted output (book: 4(3) + 1(2) = 14).
2. Crossed output (book: 4(2) + 1(3) = 11).
3. Compare (book: sorting adds 3; additive output ties at 10; s + q - 0.4sq favours crossing, 5.6 against 4.4).

Watch for: a wage and firm-quality correlation alone does not prove complementarity.

## 2. Search-and-matching unemployment (search-and-matching-unemployment)

When to use it: turning unemployment, vacancies and a matching function into job-finding rates and a steady unemployment rate.

Equations as the chapter writes them:

    M(u,v)=A u^\alpha v^{1-\alpha},
    u^*=\frac{s}{s+f(\theta)}.

Ask the user for: unemployed, vacancies, matching efficiency, separation rate.

Steps:
1. Matches (book: 0.6 sqrt(800 x 450) = 360).
2. f = M / U and q = M / V (book: 0.45 and 0.80).
3. u* = s / (s + f) (book: 0.03 / 0.48 = 6.25 percent).

Watch for: u* is a steady-state benchmark, not a forecast of the current rate.

## 3. Beveridge curve (beveridge-curve)

When to use it: finding the vacancies that sustain steady flows and telling movements from shifts.

Equations as the chapter writes them:

    \Delta U=s(L-U)-M.
    V=\frac{(184/0.8)^2}{400}=132.25.

Ask the user for: labor force, unemployment, separation rate, matching efficiency.

Steps:
1. Separations s(L - U) (book: 0.04 x 4,600 = 184).
2. Required V = (separations / A)^2 / U (book: 132.25).
3. Change A to see the shift (book: A = 0.4 needs 529).

Watch for: vacancies and unemployment rising together point to a shift in matching efficiency.

## 4. Monopsony and labor-market power (monopsony-labor-market-power)

When to use it: analysing pay and employment when a firm faces upward-sloping labor supply, and the effect of a wage floor.

Equations as the chapter writes them:

    ME(L)=w(L)+Lw'(L).
    MRP_L=ME(L).
    w=8+0.5L,

Ask the user for: the supply curve's intercept and slope, the marginal revenue product, any wage floor.

Steps:
1. Set ME = MRP (book: 8 + L = 20, L = 12, w = 14, markdown 6).
2. Competitive benchmark w = MRP (book: L = 24).
3. A floor between the monopsony wage and MRP: hire all who accept (book: floor 16 gives L = 16).

Watch for: a floor above MRP ends profitable hiring; a positive effect at one floor does not extend to higher floors.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
