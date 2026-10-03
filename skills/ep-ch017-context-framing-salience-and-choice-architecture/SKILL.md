---
name: ep-ch017-context-framing-salience-and-choice-architecture
description: Apply the principles of Chapter 17 of The Encyclopedia of Economic Principals (Context, Framing, Salience, and Choice Architecture) to the user's own numbers. Use when a bigger menu may discourage choosing, a rare large payoff may be overweighted, a price jumps at a round number, or an enrollment rate depends on the default.
---

# Chapter 17: Context, Framing, Salience, and Choice Architecture

These principles separate what an option is worth from how it is presented: menu size, salient contrasts, leading digits and defaults.

Notebook with the worked examples and figures: `../../notebooks/ch017-context-framing-salience-and-choice-architecture.ipynb`

## 1. Choice overload (choice-overload)

When to use it: deciding whether adding options to a menu raises or lowers participation.

Equation as the chapter writes it:

    1{,}000+600-200-50=\$1{,}350.

Ask the user for: best attainable benefit, any match or bonus, comparison hours, value of an hour, anticipated regret, and the value of the outside option (all in dollars).

Steps:
1. Time cost = hours x hourly value (book: 6 x 100 = 600).
2. Net = benefit + match - time cost - regret (book: 1,100 + 600 - 600 - 150 = 950).
3. Compare with the outside option (book: 950 < 1,250, so keep the cash) and solve for the hours that make them equal.

Watch for: regret and time costs are hard to measure; report the break-even hours rather than a single verdict.

## 2. Salience theory (salience-theory)

When to use it: a risky option is pitched by its rare large payoff against a sure alternative.

Equations as the chapter writes them:

    0.10(180)+0.90(35)=\$49.50
    \pi_H=\frac{0.10}{0.10+0.90(0.7)}\approx0.137

Ask the user for: the sure amount, the two lottery payoffs and their probabilities, and a salience discount delta between 0 and 1.

Steps:
1. Expected value with objective probabilities (book: 49.50).
2. Contrast of each state with the sure amount, |x - r| / (x + r) (book: 130/230 = 56.5 percent, 15/85 = 17.6 percent).
3. Multiply the less salient state's probability by delta and normalize (book: 0.10 / 0.73 = 0.137).
4. Weighted value and choice (book: 0.137(180) + 0.863(35) = 54.86 > 50, so the lottery).

Watch for: with delta = 1 the weights are the objective probabilities; the effect is about attention, not the lottery.

## 3. Left-digit bias (left-digit-bias)

When to use it: prices or valuations jump when a number crosses a round threshold.

Equations as the chapter writes them:

    \$15{,}000-200(\$0.10)=\$14{,}980.
    \$14{,}980-\$500=\$14{,}480

Ask the user for: reference value and quantity, smooth rate per unit, threshold, and the observed jump.

Steps:
1. Smooth benchmark = value - rate x extra units (book: 15,000 - 200 x 0.10 = 14,980).
2. Excess discontinuity = observed gap - smooth difference (book: 520 - 20 = 500).
3. Check whether anything real changes at the threshold before calling it bias.

Watch for: a warranty or rule that expires at the threshold can make the jump rational.

## 4. Default effect (default-effect)

When to use it: comparing participation under opt-in, automatic enrollment and active choice.

Equations as the chapter writes them:

    \Delta_i=V_i(E)-V_i(N)=\$30.
    60+9=69,

Ask the user for: group sizes, each group's gain from enrolling, the switching cost, and the share who never act.

Steps:
1. Attentive workers leave the default only if their gain from switching exceeds the cost (book: 30 > 20, so the 60 enroll under opt-in).
2. Inactive workers keep the default (book: 15 enrolled only under automatic enrollment).
3. Under active choice everyone decides on intrinsic gain (book: 60 + 9 = 69 percent).

Watch for: the chapter assumes no endorsement signal in the default; a default read as advice changes the gains.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
