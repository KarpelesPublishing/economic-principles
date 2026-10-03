---
name: ep-ch077-political-competition-coalitions-and-redistribution
description: Apply Chapter 77 of The Encyclopedia of Economic Principals (Political Competition, Coalitions, and Redistribution) to the user's own numbers. Use when someone asks how an uncertain election moves output through inflation surprises, how a pre-election stimulus plays out afterward, whether a leader's coalition will accept a shift from private rewards to public goods, or why a ruler blocks a reform that raises output.
---

# Chapter 77: Political Competition, Coalitions, and Redistribution

Trace how elections, coalition size and the risk of losing power shape what governments deliver.

Notebook with the worked examples and figures: `../../notebooks/ch077-political-competition-coalitions-and-redistribution.ipynb`

## 1. Partisan business cycle (partisan-business-cycle)

When to use it: wage contracts are set before an election between parties with different inflation plans.

    pi^e = q pi_L + (1 - q) pi_R;  gap_i = alpha (pi_i - pi^e)

Steps:
1. Expected inflation (book: 0.65 x 5.5 + 0.35 x 1.5 = 4.1).
2. Gap for each winner (book: 0.4 x 1.4 = 0.56 and 0.4 x (-2.6) = -1.04).
3. Expected squared gap = alpha^2 q (1 - q) (pi_L - pi_R)^2 (book: 0.5824).

Watch for: indexation or an independent central bank removes the surprise.

## 2. Political business cycle (political-business-cycle)

When to use it: an incumbent raises inflation before a vote under adaptive expectations.

    u_t = u^n - beta(pi_t - pi_t^e);  pi_{t+1}^e = pi_t^e + rho(pi_t - pi_t^e)

Steps:
1. Election-period unemployment (book: 6.5 - 0.35 x (6 - 2.5) = 5.275).
2. Next expectation (book: 2.5 + 0.4 x 3.5 = 3.9).
3. Post-election unemployment with normal inflation (book: 6.5 - 0.35 x (2.5 - 3.9) = 6.99; then 6.794).

Watch for: forward-looking contracts that anticipate the stimulus remove the effect.

## 3. Selectorate winning-coalition principle (selectorate-winning-coalition-principle)

When to use it: judging whether a regime's essential supporters will accept spending on broad public goods.

    b = (R - k - g) / W;  lambda = W / S;  accept a shift if benefit > shift / W

Steps:
1. Private reward per insider (book: (1,200 - 240 - 160) / 20 = 40).
2. Loss per member from a shift (book: 300 / 20 = 15; with W = 600, 0.5).
3. Compare with the per-resident benefit (book: 0.7; accept when W > 428.6).

Watch for: the result changes if the service reaches coalition members unequally.

## 4. Political replacement effect (political-replacement-effect)

When to use it: a reform raises output but also strengthens potential challengers.

    payoff = revenue - cost + (1 - q) V

Steps:
1. Status quo (book: 270 + 0.92 x 700 = 914).
2. Reform (book: 340 - 30 + 0.72 x 700 = 814, so block).
3. Decompose: net fiscal gain 40 against replacement cost (0.28 - 0.08) x 700 = 140.
4. Test remedies (book: a charter holding q to 0.12 gives 926 > 914; a loan cutting cost to 20 gives 824 < 914).

Watch for: partial reforms that keep the feared organization out reveal what the incumbent fears.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real government.
