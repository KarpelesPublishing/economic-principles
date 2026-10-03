---
name: ep-ch087-human-capital-technology-signaling-and-discrimination
description: Apply the principles of Chapter 87 of The Encyclopedia of Economic Principals (Human Capital, Technology, Signaling, and Discrimination) to the user's own numbers. Use when estimating how skill-biased technology and skill supply move a wage premium, valuing training over a working horizon, decomposing automation into displacement, scale and new tasks, or checking how unequal score reliability shifts hiring forecasts.
---

# Chapter 87: Human Capital, Technology, Signaling, and Discrimination

These principles price skills, value investment in them and separate the channels that move employment and hiring. The chapter's numbers are hypothetical teaching values.

Notebook with the worked examples and figures: `../../notebooks/ch087-human-capital-technology-signaling-and-discrimination.ipynb`

## 1. Skill-biased technical change (skill-biased-technical-change)

When to use it: predicting the skill premium from a technology ratio and relative skill supply.

Equations as the chapter writes them:

    \ln(H/L)=\ln(A_H/A_L)-2\ln(w_H/w_L).
    \ln(0.25)=\ln(2)-2\ln(w_H/w_L),

Ask the user for: technology ratio, relative supply, elasticity of substitution.

Steps:
1. w_H/w_L = (A_H/A_L / (H/L))^(1/sigma) (book: (2 / 0.25)^(1/2) = 2.83).
2. Compare with the starting premium (book: 2, so +41 percent).
3. Recompute with new supply (book: H/L = 0.40 gives 2.24).

Watch for: the residual between predicted and observed premiums is not proof of another technology shock.

## 2. Ben-Porath life-cycle human-capital model (ben-porath-life-cycle-human-capital-model)

When to use it: deciding whether training pays given the years left to use it.

Equations as the chapter writes them:

    H_{t+1}=(1-\delta)H_t+F(s_tH_t,x_t),
    3{,}000\frac{1-(1.05)^{-20}}{0.05}\approx37{,}386.

Ask the user for: annual gain, discount rate, years of use, tuition and forgone pay.

Steps:
1. PV = gain x (1 - (1 + r)^-T) / r (book: 37,386.63 for 20 years, printed as 37,386).
2. NPV = PV - total cost (book: about 17,387 against 20,000).
3. Repeat for short horizons (book: 5 years 12,988; 8 years 19,390).

Watch for: skill depreciation shortens the useful horizon.

## 3. Task displacement and reinstatement (task-displacement-and-reinstatement)

When to use it: decomposing an automation's effect on employment.

Equations as the chapter writes them:

    \frac{50}{7}\approx7.14.
    (50+15)(1.2)=78

Ask the user for: labor tasks before and after, tasks per worker, output scale, new human tasks.

Steps:
1. Displacement: remaining labor tasks / tasks per worker (book: 50 / 7 = 7.14 against 10).
2. Scale: multiply by output scale (book: 60 / 7 = 8.57).
3. Reinstatement: add new tasks (book: 78 / 7 = 11.14).

Watch for: the end count hides the interim path for displaced workers.

## 4. Statistical discrimination (statistical-discrimination)

When to use it: checking how unequal score reliability shifts forecasts at the same score.

Equations as the chapter writes them:

    E(\theta_i\mid s_i,g)=\lambda_gs_i+(1-\lambda_g)\mu_g,
    E(\theta\mid80,A)=0.75(80)+0.25(60)=75

Ask the user for: score, group prior mean, weight on the score for each group, the cutoff.

Steps:
1. Forecast for each group (book: A 75, B 0.25(80) + 0.75(60) = 65).
2. Compare with the cutoff (book: 70; A hired, B not).
3. Check low scores and equal reliability (book: at 50, A 52.5 and B 57.5; lambda 0.90 gives 78 for both).

Watch for: the weights are beliefs about reliability; test them rather than assume them.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real group or occupation.
