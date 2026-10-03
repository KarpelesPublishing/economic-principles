---
name: ep-ch015-choice-under-risk-ambiguity-and-probability-weighting
description: Apply the principles of Chapter 15 of The Encyclopedia of Economic Principals (Choice Under Risk, Ambiguity, and Probability Weighting) to the user's own numbers. Use when a choice flips after a shared outcome is removed, when someone refuses a favorable bet, when people avoid options with unknown odds, or when long shots are bought and likely gains are traded for a sure amount.
---

# Chapter 15: Choice Under Risk, Ambiguity, and Probability Weighting

These principles show where expected utility stops describing choices: special treatment of certainty, losses that weigh more than gains, worst-case thinking about unknown odds, and distorted probability weights.

Notebook with the worked examples and figures: `../../notebooks/ch015-choice-under-risk-ambiguity-and-probability-weighting.ipynb`

## 1. Allais paradox (allais-paradox)

When to use it: a choice reverses after an outcome common to both options is added or removed.

Equations as the chapter writes them:

    u(1)>0.10u(5)+0.89u(1).
    0.11u(1)>0.10u(5).
    0.10u(5)>0.11u(1).

Ask the user for: the prizes, the probabilities of each option in both menus, and the choices made.

Steps:
1. Normalize the lowest prize to utility 0 and write each option's expected utility (book: EU(A) = u(1), EU(B) = 0.10u(5) + 0.89u(1)).
2. Subtract the common consequence from both sides (book: 0.11u(1) > 0.10u(5)).
3. Check whether the other menu needs the reverse inequality (book: choosing D needs 0.10u(5) > 0.11u(1), a contradiction). No utility ratio fits both; at u(5)/u(1) = 1.1 both menus are ties.

Watch for: one pair of choices does not identify a weighting function; it only rules out expected utility.

## 2. Prospect theory (prospect-theory)

When to use it: someone refuses a bet with positive expected value.

Equations as the chapter writes them:

    V=0.5(150)+0.5[-2(100)]=75-100=-25.
    0.5g^*-0.5(2)(100)=0,

Ask the user for: the gain, the loss, the probabilities and a loss-aversion coefficient lambda (state that it is assumed).

Steps:
1. Value gains at face value and losses at lambda times the loss (book: -2(100) = -200).
2. Weight and add (book: 0.5 x 150 + 0.5 x (-200) = 75 - 100 = -25, so reject although expected value is 25).
3. Solve for the threshold gain g* = lambda x loss (book: 2 x 100 = 200). A gain exactly at g* is a tie.

Watch for: curvature (alpha below 1) or unequal decision weights change the threshold.

## 3. Ellsberg paradox (ellsberg-paradox)

When to use it: people prefer known odds to unknown odds for both sides of a bet.

Equations as the chapter writes them:

    0.5(100)=50.
    0.2(100)=20.

Ask the user for: the prize, the known probability, and the range of probabilities they find plausible for the unknown option.

Steps:
1. Value the known bet (book: 0.5 x 100 = 50).
2. Value each ambiguous bet at its worst-case probability (book: red 0.2 x 100 = 20; black 1 - 0.8 = 0.2, so 20).
3. Compare: the maxmin gap is 50 - 20 = 30 for each color. If the composition is revealed (book: 65 red), use the single probability (65 and 35).

Watch for: smooth ambiguity models value bets between the worst case and the average, so maxmin is the extreme case.

## 4. Inverse-S probability weighting (inverse-s-probability-weighting)

When to use it: long shots are bought while likely gains are traded for a smaller sure amount.

Equations as the chapter writes them:

    0.01(1{,}000)=10,
    0.05(1{,}000)=50,
    0.80(100)=80,
    0.65(100)=65,

Ask the user for: the probability, the prize, the sure alternative and a decision weight (state that it is assumed).

Steps:
1. Linear benchmark: p x prize (book: 0.01 x 1,000 = 10 against 30, sure amount wins).
2. Weighted value: w(p) x prize (book: 0.05 x 1,000 = 50, gamble wins; 0.65 x 100 = 65 against 70, sure amount wins).
3. Find the weight that flips the choice: w = sure / prize (constructed from the book example: 70 / 100 = 0.70).

Watch for: a weight estimated at one probability says nothing about weights at other probabilities.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
