---
name: ep-ch021-experimental-markets-learning-and-preference-elicitation
description: Apply the principles of Chapter 21 of The Encyclopedia of Economic Principals (Experimental Markets, Learning, and Preference Elicitation) to the user's own numbers. Use when judging whether experience narrows a valuation gap, predicting choices in a guess-the-average game, checking how much surplus a trading institution realizes, or testing whether choice and pricing rank options the same way.
---

# Chapter 21: Experimental Markets, Learning, and Preference Elicitation

These principles help the user tell whether measured behavior reflects stable preferences or the experience, institution and elicitation method that produced it.

Notebook with the worked examples and figures: `../../notebooks/ch021-experimental-markets-learning-and-preference-elicitation.ipynb`

## 1. Market-experience effect (market-experience-effect)

When to use it: a gap between what owners ask and buyers offer, measured before and after repeated paid trading.

Equation as the chapter writes it:

    A(0)=\$16-\$8=\$8.
    A(10)=\$12-\$10=\$2,

Ask the user for: the ask and offer (dollars) for novices and for experienced traders, and any posted price.

Steps:
1. Compute each gap A = ask - offer (book: 16 - 8 = 8, then 12 - 10 = 2).
2. A posted price p clears only if offer >= p >= ask (book: at 12 novices do not trade, since 12 < 16).
3. State the fall in the gap (book: 8 - 2 = 6) and the midpoint (book: (12 + 10) / 2 = 11).

Watch for: a falling average gap can come from poor performers leaving, not from learning; ask for each person's change.

## 2. Beauty-contest convergence (beauty-contest-convergence)

When to use it: payoffs depend on guessing a fraction p of what others choose.

Equation as the chapter writes it:

    \bar{x}_1=\frac{50+40+35+30+25+18}{6}=33,
    \bar{x}_2=\frac{99}{6}=16.5, \qquad t_2=\frac{2}{3}(16.5)=11.

Ask the user for: p, the range of choices, and any observed choices.

Steps:
1. Level-k choice = 50 p^k (book: 50, 33.33, 22.22, 14.81 for p = 2/3).
2. For observed choices, mean and target p x mean (book: 198 / 6 = 33, target 22).
3. Closest choice wins (book: 25, 3 away). With p = 1 any common choice is stable.

Watch for: real groups mix depths of reasoning and stop after a few steps.

## 3. Double-auction convergence (double-auction-convergence)

When to use it: comparing how much surplus different trading rules realize.

Equation as the chapter writes it:

    \$70+\$40+\$5=\$115,

Ask the user for: one-unit buyer values and seller costs, and any sealed bids and asks.

Steps:
1. Sort values high to low and costs low to high; gains are value minus cost (book: 70, 40, 5, -25).
2. Q* counts positive gains and maximum surplus sums them (book: Q* = 3, 115); prices from 75 to 80 support it.
3. In a sealed round, only bids at or above asks trade (book: 65 against 40, one trade, 100 - 30 = 70).

Watch for: realized surplus depends on which pairs trade, not on prices, which only divide it.

## 4. Preference reversal (preference-reversal)

When to use it: choice questions and price questions may rank the same options differently.

Equation as the chapter writes it:

    \operatorname{EV}(P)=0.80(\$30)=\$24,
    \operatorname{EV}(D)=0.25(\$100)=\$25.

Ask the user for: each lottery's prize and probability, the direct choice, and the stated selling prices.

Steps:
1. Expected values (book: 0.80 x 30 = 24 and 0.25 x 100 = 25).
2. Rank by stated prices (book: 28 for D above 20 for P).
3. A reversal exists when this ranking differs from the direct choice (book: chose P, priced D higher). If D's price were 18 there would be none.

Watch for: neither the choice nor the price is automatically the true preference.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
