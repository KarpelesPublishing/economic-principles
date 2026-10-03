---
name: ep-ch007-social-welfare-inequality-and-compensation
description: Apply Chapter 7 of The Encyclopedia of Economic Principals (Social Welfare, Inequality, and Compensation) to the user's own numbers. Use when someone asks whether a transfer with leakage raises summed welfare, compares income distributions with an Atkinson index, looks for a side payment that makes an assignment envy-free, or runs a Kaldor-Hicks compensation test on a project.
---

# Chapter 7: Social Welfare, Inequality, and Compensation

State the value judgment (the utility curve, the inequality aversion, who must be paid), then let the arithmetic rank the options.

Notebook with the worked examples and figures: `../../notebooks/ch007-social-welfare-inequality-and-compensation.ipynb`

## 1. Diminishing marginal utility of income (diminishing-marginal-utility-of-income)

    W_0 = sqrt(25) + sqrt(100) = 5 + 10 = 15.
    W_1 = sqrt(34) + sqrt(91) approx 5.831 + 9.539 = 15.370.

Ask the user for: incomes, the amount taken, the amount lost in transit, the utility curve.

Steps:
1. New incomes (book: (34, 91); with 5 lost, (29, 91)).
2. Sum utilities before and after (book: 15.370 against 15; with leakage the book prints 14.924 and a drop of about 0.076 from rounded terms; unrounded 14.9246 and 0.0754).
3. The transfer passes when the sum rises.

Watch for: the book prints the leaky drop as about 0.076; the exact value is 0.0754.

## 2. Atkinson inequality aversion (atkinson-inequality-aversion)

    A(epsilon) = 1 - y_EDE / mu,   y_EDE,P = sqrt(20 x 80) = sqrt(1600) = 40.

Ask the user for: the incomes in each distribution and the inequality aversion epsilon.

Steps:
1. EDE = (mean of y^(1 - epsilon))^(1 / (1 - epsilon)); geometric mean at epsilon = 1 (book: 40 and 42.426).
2. Index = 1 - EDE / mean (book: 0.20 and 0.057).
3. Rank by EDE (book: Q above P at epsilon 1, P above Q at 0).

Watch for: always report epsilon; the ranking can flip with it.

## 3. Envy-freeness (envy-freeness)

    120 - 15 = 105,  80 + 15 = 95,  90 + 15 = 105,  100 - 15 = 85

Ask the user for: each person's value of each item, the assignment, the payment.

Steps:
1. Each person's own package and their view of the other's (book: A 105 vs 95, B 105 vs 85).
2. Envy-free band: payer's value gap / 2 at most, receiver's gap / 2 at least (book: 5 to 20).

Watch for: a payment outside the band moves the envy to the other person.

## 4. Kaldor-Hicks compensation principle (kaldor-hicks-compensation-principle)

    S = G - L - R = 125 - 80 - 30 = 15.   S' = 125 - 80 - 50 = -5.

Ask the user for: winners' gains, losers' required compensation, real resource cost, cost of paying compensation.

Steps:
1. S = G - L - R - admin (book: 15; with admin 4, 11).
2. Passes when S > 0. It is an actual Pareto improvement only if compensation is paid.

Watch for: transfers are not costs; administration of them is.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and indifference instead of forcing a ranking.
- Do not present the book's hypothetical numbers as facts about real households.
