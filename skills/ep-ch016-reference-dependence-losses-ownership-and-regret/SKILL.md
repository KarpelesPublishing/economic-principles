---
name: ep-ch016-reference-dependence-losses-ownership-and-regret
description: Apply the principles of Chapter 16 of The Encyclopedia of Economic Principals (Reference Dependence, Losses, Ownership, and Regret) to the user's own numbers. Use when an owner asks far more than buyers offer, when a safer option wins against a better gamble because the foregone result will be seen, when past spending is argued as a reason to continue, or when repeated favorable risks are judged one at a time.
---

# Chapter 16: Reference Dependence, Losses, Ownership, and Regret

These principles separate the payoffs of a choice from the reference points, comparisons, histories and frames that move it, so the user can see which part of a decision is doing the work.

Notebook with the worked examples and figures: `../../notebooks/ch016-reference-dependence-losses-ownership-and-regret.ipynb`

## 1. Loss aversion (loss-aversion)

When to use it: an owner's minimum selling price sits well above a buyer's maximum price for the same use value.

Equations as the chapter writes them:

    \mathrm{WTA}=1.5(\$6)=\$9,    \mathrm{WTP}=\$6.    \$9-\$6=\$3.

Ask the user for: the use value v (dollars), a loss coefficient lambda, and any posted price.

Steps:
1. WTA = lambda x v (book: 1.5 x 6 = 9).
2. WTP = v (book: 6).
3. Wedge = WTA - WTP (book: 9 - 6 = 3).
4. At the posted price, the owner sells only if price >= WTA and the buyer buys only if price <= WTP (book: at 7.50 neither trades). State the lambda that would let the owner sell: price / v.

Watch for: ownership alone is not proof of loss aversion; wealth effects and transaction costs must be negligible.

## 2. Regret theory (regret-theory)

When to use it: a chooser prefers a sure amount to a gamble with a higher expected value, and both outcomes will be revealed.

Equations as the chapter writes them:

    E[G]=0.9(\$65)+0.1(\$0)=\$58.50.
    D(G,S)=0.9(225)+0.1(-2{,}500)=-47.5.

Ask the user for: the sure payment S, the gamble's payoffs and probabilities, and a comparison rule Q (the book uses Q(d) = d^2 for d >= 0 and -(-d)^2 for d < 0).

Steps:
1. Expected values (book: E[S] = 50, E[G] = 58.50).
2. For each state, d = gamble payoff - S and Q(d) (book: 15 gives 225; -50 gives -2,500).
3. D(G,S) = sum of p x Q(d) (book: 202.5 - 250 = -47.5).
4. D < 0 means the sure payment is chosen; D > 0 the gamble. Report the probability at which D crosses zero.

Watch for: the reversal depends on the chosen Q and on both outcomes being revealed.

## 3. Sunk-cost effect (sunk-cost-effect)

When to use it: past, irrecoverable spending is offered as a reason to continue a project.

Equations as the chapter writes them:

    B-C=\$45{,}000-\$60{,}000=-\$15{,}000,
    -\$15{,}000+0.10(\$20{,}000)=-\$13{,}000,
    -\$15{,}000+0.10(\$200{,}000)=\$5{,}000,

Ask the user for: remaining benefit B, remaining cost C, past spending, and (to model the bias) a weight alpha.

Steps:
1. Forward value B - C (book: -15,000). This alone decides: continue only if positive.
2. Biased score = (B - C) + alpha x sunk (book: -13,000 for 20,000 sunk; 5,000 for 200,000 sunk).
3. The past spend that flips the biased decision is (C - B) / alpha (book: 15,000 / 0.10 = 150,000).

Watch for: past spending is irrelevant only if it carries no information about receipts or completion.

## 4. Narrow bracketing (narrow-bracketing)

When to use it: a series of favorable independent bets is rejected because each one alone can lose.

Equations as the chapter writes them:

    0.5(\$120)-0.5(\$100)=\$10,
    6(\$10)=\$60.
    120h-100(6-h)=220h-600.

Ask the user for: the gain, the loss, the probability of a gain and the number of bets n.

Steps:
1. Expected value per bet and per bundle (book: 10 and 60).
2. Total with h wins: gain x h - loss x (n - h) (book: 220h - 600).
3. Loss probability: sum of C(n, h) p^h (1 - p)^(n - h) over h where the total is negative (book: 22/64 = 34.375%).
4. Report the worst case and whether the user can bear it (book: -600).

Watch for: the loss probability does not fall smoothly with n (12 bets of +120/-100 lose with probability 38.721%); liquidity for the worst case is required.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
