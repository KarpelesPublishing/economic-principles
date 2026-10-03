---
name: ep-ch020-social-preferences-fairness-identity-and-reciprocity
description: Apply the principles of Chapter 20 of The Encyclopedia of Economic Principals (Social Preferences, Fairness, Identity, and Reciprocity) to the user's own numbers. Use when someone asks how small an offer a fair-minded counterpart will accept, whether extending trust pays, whether paying above the going wage buys enough effort, or where voluntary group contributions will settle.
---

# Chapter 20: Social Preferences, Fairness, Identity, and Reciprocity

These principles put envy, trust, gifts and conditional matching into payoffs, so the user can predict when people reject offers, return favors, work harder for a generous wage, or follow what others give.

Notebook with the worked examples and figures: `../../notebooks/ch020-social-preferences-fairness-identity-and-reciprocity.ipynb`

## 1. Inequity aversion (inequity-aversion)

When to use it: an offer splits a fixed amount and the receiver can refuse.

Equations as the chapter writes them:

    U_R=4-0.5(16-4)=-2.
    s-0.5[(20-s)-s]\geq0.

Ask the user for: the amount to split, the offer, and an envy weight alpha (how much a dollar of being behind hurts).

Steps:
1. Utility of accepting: offer minus alpha times (other's share minus offer) (book: 4 - 0.5 x 12 = -2).
2. Compare with zero from rejecting (book: -2 < 0, reject).
3. Threshold offer s* = alpha x pie / (1 + 2 alpha) (book: 0.5 x 20 / 2 = 5). State the decision and the offer that would flip it; at exactly s* the responder is indifferent.

Watch for: envy weights differ across people and are not observed directly.

## 2. Trust-game reciprocity (trust-game-reciprocity)

When to use it: one side puts money at risk that grows in the other side's hands.

Equations as the chapter writes them:

    \pi_1=12-6+8=\$14,
    \pi_2=18-8=\$10.

Ask the user for: endowment E, amount sent s, multiplier m, expected return r.

Steps:
1. Receiver gets m x s (book: 3 x 6 = 18).
2. Sender payoff E - s + r (book: 12 - 6 + 8 = 14); receiver m s - r (book: 18 - 8 = 10).
3. Trust pays the sender only if r > s; total surplus is E + (m - 1)s (book: 24).

Watch for: returns depend on intentions and norms, not only on the amount received.

## 3. Gift-exchange efficiency wage (gift-exchange-efficiency-wage)

When to use it: deciding whether to pay above the going wage when effort cannot be enforced.

Equations as the chapter writes them:

    8(\$6)=\$48,
    \$60-\$22=\$38.
    \$6[e(22)-e(18)]>\$4.

Ask the user for: base wage and effort, higher wage and expected effort, value per unit of output.

Steps:
1. Profit at each wage: value x effort - wage (book: 48 - 18 = 30 and 60 - 22 = 38).
2. Premium pays if value x (extra effort) > premium (book: 6 x 2 = 12 > 4).
3. Break-even effort = base effort + premium / value (book: 8 + 4/6 = 8.67).

Watch for: the effort response is uncertain and may fade over time.

## 4. Conditional cooperation (conditional-cooperation)

When to use it: voluntary contributions where people give more when they expect others to give more.

Equations as the chapter writes them:

    4(0.4)=1.6>1.
    g_L=2+0.6E_L(\bar g_{-L}),
    g=2+0.6g, g=5.

Ask the user for: group size, return per token to each member, the response intercept and slope, the belief, the cap.

Steps:
1. Contribution g = intercept + slope x belief, within the cap (book: 2 + 0.6 x 15 = 11).
2. Private net cost g(1 - return) and group benefit g x n x return (book: 6.6 and 17.6).
3. Symmetric fixed point g = intercept / (1 - slope) (book: 2 / 0.4 = 5); beliefs above it drift down to it.

Watch for: real response schedules differ across people; some give nothing whatever they expect.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
