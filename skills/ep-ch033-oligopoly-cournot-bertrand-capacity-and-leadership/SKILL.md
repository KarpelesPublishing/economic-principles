---
name: ep-ch033-oligopoly-cournot-bertrand-capacity-and-leadership
description: Apply Chapter 33 of The Encyclopedia of Economic Principals (Oligopoly: Cournot, Bertrand, Capacity, and Leadership) to the user's own numbers. Use when someone solves a Cournot market with different costs, asks whether a cartel can deter cheating, checks whether a merger among quantity setters is profitable, or values a first-mover output commitment.
---

# Chapter 33: Oligopoly: Cournot, Bertrand, Capacity, and Leadership

Solve the few-firm market for quantities and price, then test collusion, mergers and commitment against it.

Notebook with the worked examples and figures: `../../notebooks/ch033-oligopoly-cournot-bertrand-capacity-and-leadership.ipynb`

## 1. Cournot quantity competition (cournot-quantity-competition)

When to use it: firms choose quantities at once and share one linear demand.

    q_A=\frac{90-q_B}{2},\qquad q_B=\frac{66-q_A}{2}

Ask the user for: demand intercept a (P = a - Q) and each firm's marginal cost.

Steps:
1. P = (a + sum of costs)/(n + 1) (book: (100 + 10 + 34)/3 = 48).
2. q_i = P - c_i (book: 38 and 14); drop any firm whose q_i would be negative and re-solve.
3. Profit (P - c_i) q_i (book: 1,444 and 196).

Watch for: the closed form needs homogeneous output and constant marginal cost.

## 2. Cartel instability (cartel-instability)

    \delta^*=\frac{220-120}{220-70}=\frac{2}{3}\approx0.667
    \frac{q\delta(\pi^C-\pi^P)}{1-\delta}

Ask the user for: cartel, deviation and punishment profits per period, discount factor, detection probability.

Steps:
1. delta* = (pi^D - pi^C)/(pi^D - pi^P) (book: 0.667).
2. Expected loss = q delta (pi^C - pi^P)/(1 - delta) (book: 0.40 x 0.80 x 50 / 0.20 = 80).
3. Deterred only if the expected loss exceeds the temptation pi^D - pi^C (book: 80 < 100, not deterred).

Watch for: this is a simplified expected-loss comparison, not a full repeated-game equilibrium.

## 3. Cournot merger paradox (cournot-merger-paradox)

    q(6)=\frac{60}{7}\approx8.57
    P=\frac{115}{6},\qquad q_M=\frac{85}{6},\qquad q_O=\frac{55}{6}

Ask the user for: demand intercept, costs, number of firms, merged firm's cost.

Steps:
1. Pre-merger profit of the two insiders (book: 2 x 73.47 = 146.94).
2. Re-solve Cournot with one fewer firm and the merged cost (book: cost 10 gives 100; cost 5 gives 200.69).
3. The merger pays privately only if step 2 exceeds step 1.

Watch for: no entry and unconstrained outsider expansion.

## 4. Stackelberg leadership (stackelberg-leadership)

    R_F(q_L)=\max\left\{0,\frac{80-q_L}{2}\right\}
    \pi_L=q_L\left[80-q_L-\frac{80-q_L}{2}\right]=\frac{q_L(80-q_L)}{2}

Ask the user for: demand intercept, common marginal cost, leader's committed output.

Steps:
1. Follower q_F = (a - c - q_L)/2 (book: (80 - 40)/2 = 20).
2. Price and profits (book: P = 40, pi_L = 800, pi_F = 400).
3. Compare with Cournot (book: 711.11 each).

Watch for: the commitment must be observable and irreversible.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
