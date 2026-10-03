---
name: ep-ch091-cultural-transmission-persistence-and-economic-change
description: Apply the principles of Chapter 91 of The Encyclopedia of Economic Principals (Cultural Transmission, Persistence, and Economic Change) to the user's own numbers. Use when tracing how slowly a habit follows a change in practice, testing whether moral terms tip a saving or investment choice, comparing family and institutional transmission of a trait, or judging how much instability a tradition can survive.
---

# Chapter 91: Cultural Transmission, Persistence, and Economic Change

These principles turn habits, values and inherited traits into quantities that move. The chapter's numbers are hypothetical teaching numbers, not historical data.

Notebook with the worked examples and figures: `../../notebooks/ch091-cultural-transmission-persistence-and-economic-change.ipynb`

## 1. Institutional habits and cumulative adaptation (institutional-habits-and-cumulative-adaptation)

When to use it: forecasting how fast a habit catches up with new practice.

Equations as the chapter writes them:

    h_{t+1}=(1-\alpha)h_t+\alpha x_t
    h_2=0.75(0.05)+0.25(0.80)=0.2375

Ask the user for: the starting habit share, the updating speed and the practice path.

Steps:
1. Apply the update each period (book: 0.05, 0.2375, 0.3781, 0.4836).
2. Compare with practice to see the lag (book: 0.80 against 0.4836 after four periods).

Watch for: the update rule is instructional, not an estimated rate.

## 2. Protestant ethic mechanism (protestant-ethic-mechanism)

When to use it: testing whether moral terms change a consumption versus investment choice.

Equations as the chapter writes them:

    70+0.50(30)=85
    40+0.50(78)=79
    40+0.50(55)+5=72.5

Ask the user for: current spending, discount factor, future payoffs and any moral penalties or rewards.

Steps:
1. Score each plan: current + discount x future (book: 85 and 79).
2. Add moral terms (book: 75 and 84, so invest) and remove them for the counterfactual.

Watch for: the example estimates no historical community.

## 3. Cultural transmission (cultural-transmission)

When to use it: projecting next generation's share of a trait.

Equations as the chapter writes them:

    P(A\mid A)=\tau_A+(1-\tau_A)x_t
    x_{t+1}=x_tP(A\mid A)+(1-x_t)P(A\mid B)

Ask the user for: the current share and each type's direct transmission rate, plus any institutional exposure.

Steps:
1. Conditional probabilities (book: 0.65 and 0.24).
2. Next share (book: 0.30 x 0.65 + 0.70 x 0.24 = 0.363).
3. Exposure e: x + e(1 - x) (book: 0.363 + 0.40 x 0.637 = 0.6178).

Watch for: name the channel; family and institutions move the share at very different speeds.

## 4. Cultural persistence (cultural-persistence)

When to use it: judging whether copying tradition survives environmental change.

Equations as the chapter writes them:

    x^*=\frac{\kappa-\Delta\beta}{\kappa(1-\Delta)}, \qquad \Delta\leq\frac{\kappa}{\beta}

Ask the user for: the payoff from the correct action, the cost of learning and the chance the environment changes.

Steps:
1. x* from the formula (book: 12 / 16.2 = 0.741 at Delta 0.10; 0.222 at 0.25).
2. Threshold kappa / beta (book: 0.30); above it x* = 0.

Watch for: the model is stylized; it shows conditional persistence, not a forecast.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real household, group or place.
