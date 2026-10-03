---
name: ep-ch062-structural-transformation-dual-economies-and-migration
description: Apply the principles of Chapter 62 of The Encyclopedia of Economic Principals (Structural Transformation, Dual Economies, and Migration) to the user's own numbers. Use when someone asks how moving workers between sectors changes inequality, how to split a productivity gain into within-sector growth and reallocation, why labor-intensive services get relatively dearer, or whether creating city jobs can raise urban unemployment.
---

# Chapter 62: Structural Transformation, Dual Economies, and Migration

These principles tell the user how composition shifts, relative productivity and expected wages drive what happens as workers leave farming.

Notebook with the worked examples and figures: `../../notebooks/ch062-structural-transformation-dual-economies-and-migration.ipynb`

## 1. Kuznets curve (kuznets-curve)

When to use it: income dispersion changes as workers move from a low-income to a high-income sector.

Equation as the chapter writes it:

    V_1=\frac{2(8-3.2)^2+8(2-3.2)^2}{10}=\frac{57.6}{10}=5.76.

Ask the user for: workers in each sector and the income in each.

Steps:
1. Mean income (book: (2 x 8 + 8 x 2) / 10 = 3.2).
2. Population variance from each group's gap to the mean (book: 57.6 / 10 = 5.76).
3. Repeat at another stage (book: nine modern workers give 3.24) and say whether dispersion is rising or falling.

Watch for: the inverted U is possible, not necessary; dispersion inside the modern sector can change the path.

## 2. Structural transformation (structural-transformation)

When to use it: splitting a rise in output per worker into within-sector growth and reallocation.

Equation as the chapter writes it:

    P=\sum_i s_i p_i.

Ask the user for: employment shares and output per worker by sector, before and after.

Steps:
1. P before and after (book: 580 / 100 = 5.8 and 680 / 100 = 6.8).
2. Within term, sum of s_i0 (p_i1 - p_i0) (book: 0.70(14/3 - 4) = 0.467).
3. Reallocation term, sum of p_i1 (s_i1 - s_i0) (book: 0.533); check the two add to the total change.

Watch for: where released workers go matters (book: informal services at 3 give only 6.1).

## 3. Baumol cost disease (baumol-cost-disease)

When to use it: a service with stagnant productivity gets dearer relative to goods.

Equation as the chapter writes it:

    \frac{p_S}{p_P}=\frac{a_P}{a_S}.

Ask the user for: the common wage, goods output per hour, hours per unit of the service.

Steps:
1. Goods unit cost = wage / output per hour (book: 30 / 4 = 7.50).
2. Service unit cost = hours x wage (book: 8 x 30 = 240).
3. Relative cost = service / goods (book: 240 / 7.50 = 32, up from 16).

Watch for: the result assumes one wage across sectors and labor as the only cost.

## 4. Harris-Todaro migration paradox (harris-todaro-migration-paradox)

When to use it: judging a city job program when migrants respond to expected wages.

Equation as the chapter writes it:

    L_u=J\frac{w_u}{w_r}.

Ask the user for: formal jobs J, formal wage w_u, rural wage w_r.

Steps:
1. Equilibrium labor force (book: 120 x 200 / 100 = 240).
2. Unemployment = L_u - J (book: 240 - 120 = 120).
3. Compare with the baseline (book: 40 migrants for 20 jobs; unemployment up by 20).

Watch for: informal earnings, moving costs or resident-only hiring weaken the paradox.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy or historical episode.
