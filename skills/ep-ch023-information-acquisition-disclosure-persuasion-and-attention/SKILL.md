---
name: ep-ch023-information-acquisition-disclosure-persuasion-and-attention
description: Apply the principles of Chapter 23 of The Encyclopedia of Economic Principals (Information Acquisition, Disclosure, Persuasion, and Attention) to the user's own numbers. Use when someone designs a disclosure rule to persuade an audience, relies on reports from an advisor with different aims, decides whether to certify quality voluntarily, or asks whether paying for research can still earn a return when prices are informative.
---

# Chapter 23: Information Acquisition, Disclosure, Persuasion, and Attention

These principles tell the user how much information a sender can credibly pass on, when silence reveals bad news, and why informative prices still leave a reward for research.

Notebook with the worked examples and figures: `../../notebooks/ch023-information-acquisition-disclosure-persuasion-and-attention.ipynb`

## 1. Bayesian persuasion (bayesian-persuasion)

When to use it: a sender can commit in advance to a rule for what it will reveal.

Equation as the chapter writes it:

    Pr(G | retain) = 0.30 / (0.30 + 0.70x)
    0.30 / (0.30 + 0.70x) = 0.50  =>  x = 3/7
    0.30 + 0.70(3/7) = 0.60
    0.60(0.50) + 0.40(0) = 0.30

Ask the user for: the prior probability of the good state, the audience's action threshold.

Steps:
1. If the prior already meets the threshold, no garbling is needed (x = 1).
2. Otherwise x = p(1 - t) / (t(1 - p)) (book: 0.30 x 0.50 / (0.50 x 0.70) = 3/7).
3. Favorable message probability = p + (1 - p)x (book: 0.60, against 0.30 under full revelation).
4. Check Bayes plausibility: average posterior equals the prior (book: 0.60 x 0.50 + 0.40 x 0 = 0.30).

Watch for: the rule needs commitment, and a high favorable rate is not by itself proof of manipulation or of social value.

## 2. Cheap-talk partition equilibrium (cheap-talk-partition-equilibrium)

When to use it: an informed advisor with a known bias sends unverifiable messages.

Equation as the chapter writes it:

    a_L = t/2,   a_H = (t + 1)/2
    t + 0.10 = (a_L + a_H)/2 = (2t + 1)/4
    4t + 0.40 = 2t + 1  =>  t = 0.30

Ask the user for: the bias b on a state uniform over [0, 1].

Steps:
1. Cutoff t = (1 - 4b) / 2 (book: 0.30).
2. Actions a_L = t / 2 and a_H = (t + 1) / 2 (book: 0.15 and 0.65).
3. If t is not between 0 and 1 (b at least 0.25), only babbling remains and the action is 0.50 (book: b = 0.30 gives t = -0.10).

Watch for: several equilibria can coexist, including babbling.

## 3. Disclosure unraveling (disclosure-unraveling)

When to use it: sellers can prove their quality and buyers price silence.

Equation as the chapter writes it:

    (40 + 60 + 80 + 100)/4 = 70
    (40 + 60 + 80)/3 = 60
    (40 + 60)/2 = 50

Ask the user for: the possible qualities (equally likely, or with weights) and the disclosure cost.

Steps:
1. Price silence at the average of the silent pool (book: 70).
2. The best silent seller discloses if quality minus fee exceeds that price (book, fee 15: 100 - 15 = 85 > 70).
3. Recompute and repeat until the next seller would not gain (book: 60 - 15 = 45 < 50, stop at 50). Report an exact equality as indifference.

Watch for: noisy evidence, inattentive buyers or uninformed sellers can stop unraveling.

## 4. Grossman-Stiglitz impossibility (grossman-stiglitz-impossibility)

When to use it: judging whether costly research pays when prices already reflect much of it.

Equation as the chapter writes it:

    0.75($10) + 0.25($30) = $15
    0.975($1) + 0.025($39) = $1.95 < $2

Ask the user for: the two payoffs, how often price matches the state, research cost.

Steps:
1. Prices: pi x high + (1 - pi) x low, and the reverse (book: 110 and 90).
2. Gross profit = pi(high - p_high) + (1 - pi)(high - p_low) (book: 0.75 x 10 + 0.25 x 30 = 15).
3. Net = gross - cost (book: 13); research stops when gross falls below cost (book: 1.95 < 2 at 0.975).

Watch for: outside funding or free information can support revelation beyond the benchmark.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
