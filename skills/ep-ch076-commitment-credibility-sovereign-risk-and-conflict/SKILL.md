---
name: ep-ch076-commitment-credibility-sovereign-risk-and-conflict
description: Apply Chapter 76 of The Encyclopedia of Economic Principals (Commitment, Credibility, Sovereign Risk, and Conflict) to the user's own numbers. Use when someone asks whether a contract penalty or threat will actually deter, how default beliefs set a government's borrowing and whether repayment is credible, why discretionary policy produces an inflation bias, or whether a peace deal survives a shift in power.
---

# Chapter 76: Commitment, Credibility, Sovereign Risk, and Conflict

Test every promise or threat at the moment it must be carried out.

Notebook with the worked examples and figures: `../../notebooks/ch076-commitment-credibility-sovereign-risk-and-conflict.ipynb`

## 1. Credible commitment and credible threats (credible-commitment-and-threats)

When to use it: a contract relies on a penalty that someone must choose to enforce.

    45 - 52 = -7;  80 - 18 = 62 < 80;  escrow: 62 >= 80 - 45p

Ask for: price, cost of compliance, penalty, enforcement cost, and detection probability.

Steps:
1. Enforcer's net from enforcing (book: 45 - 52 = -7, so the lab forgives).
2. Breacher compares compliance with breach (book: 62 against 80, so low quality).
3. With automatic enforcement, breach pays price - penalty x p (book: 80 - 45 x 0.60 = 53 < 62).
4. Deterrence threshold p >= compliance cost / penalty (book: 18 / 45 = 0.40); at exactly the threshold the party is indifferent.

Watch for: false positives and escrow administration costs before concluding total surplus rises.

## 2. Credible commitment and sovereign default (credible-commitment)

When to use it: pricing a sovereign or other unenforceable promise to repay.

    q = (1 - p_d) face / (1 + r);  repay if output - face > output - penalty

Steps:
1. Bond price (book: 0.70 x 150 / 1.08 = 97.22, below the 120 needed; at 0.08, 127.78).
2. Repay payoff (book: 180 - 150 = 30) against default payoff (book: 180 - 165 = 15, repay; with penalty 100, 80, default).
3. A low default belief is justified only when repaying is the better choice.

Watch for: inability to pay after a disaster is not the same as unwillingness.

## 3. Time inconsistency and commitment devices (time-inconsistency)

When to use it: a policymaker announces a rule it may want to break after others act on it.

    L = pi^2 + 0.5(pi - pi^e - 2)^2;  pi = (pi^e + 2)/3

Steps (general weight b, ambition k: pi = b(pi^e + k)/(1 + b)):
1. Reaction to the promised zero (book: 2/3).
2. Equilibrium where pi = pi^e (book: pi = 1).
3. Losses (book: L_D = 1 + 0.5 x 4 = 3 against L_C = 2).

Watch for: rigid delegation can respond poorly to genuine supply shocks.

## 4. Commitment-problem theory of war (commitment-problem-theory-of-war)

When to use it: a settlement depends on a party whose power is rising.

    w_i = p_i x prize - cost_i;  deal holds if B's revision payoff < B's share

Steps:
1. War payoffs today (book: 0.65 x 100 - 15 = 50 and 0.35 x 100 - 20 = 15, range 50 to 85).
2. War payoffs after the shift (book: 5 and 60).
3. B's revision payoff = future war payoff - guarantor penalty (book: 60 - 20 = 40 < 45, deal holds; without a guarantor 60 > 45, it fails).

Watch for: the guarantor's penalty must itself be credible.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real country or market.
