---
name: ep-ch022-adverse-selection-lemons-signaling-and-screening
description: Apply the principles of Chapter 22 of The Encyclopedia of Economic Principals (Adverse Selection, Lemons, Signaling, and Screening) to the user's own numbers. Use when one side of a trade knows quality or risk better than the other, for example used goods markets that unravel, insurance pools losing low risks, credentials that may or may not reveal ability, and plan menus meant to sort customers.
---

# Chapter 22: Adverse Selection, Lemons, Signaling, and Screening

These principles tell the user whether hidden quality or risk will shut good trades out of a market, and whether a credential or a menu of contracts can make people reveal what they know.

Notebook with the worked examples and figures: `../../notebooks/ch022-adverse-selection-lemons-signaling-and-screening.ipynb`

## 1. Akerlof lemons equilibrium (akerlof-lemons-equilibrium)

When to use it: buyers cannot see quality and pay the average value of what is offered.

Equation as the chapter writes it:

    0.5($6,000) + 0.5($14,000) = $10,000
    50($14,000 - $11,000) = $150,000

Ask the user for: share of each quality, owners' reservation values, buyers' values (dollars).

Steps:
1. Pooled offer = share-weighted buyer value (book: 0.5 x 6,000 + 0.5 x 14,000 = 10,000).
2. Compare with the high-quality owners' value (book: 10,000 < 11,000, so they withdraw).
3. If they withdraw, the price falls to the low-quality buyer value (book: 6,000) and the lost surplus is the number of good units times (buyer value minus owner value) (book: 50 x 3,000 = 150,000).
4. State the decision and the margin that would flip it (the share of good units that lifts the offer to the owners' value).

Watch for: the drop from the pooled offer to the final price is a transfer, not a social loss.

## 2. Asymmetric information and adverse selection (asymmetric-information-adverse-selection)

When to use it: an insurer or lender prices on average risk and the safe customers can walk away.

Equation as the chapter writes it:

    pi_0 = (50($1,000) + 50($3,000)) / 100 = $2,000
    pi_1 = $3,000
    100($100) = $10,000

Ask the user for: expected claims and maximum willingness to pay for each group, group sizes, cost of classification per applicant.

Steps:
1. Pooled premium = average claim (book: 2,000).
2. If low risks' willingness to pay is below it, they leave and the premium rises to the high-risk claim (book: 1,300 < 2,000, premium 3,000).
3. With classification, each premium = own claim + classification cost; check each against willingness to pay (book: 1,100 and 3,100 at a cost of 100; 1,400 > 1,300 at 400).
4. Total classification cost = applicants x cost (book: 100 x 100 = 10,000).

Watch for: classification can reveal type without restoring trade, and its resource cost counts.

## 3. Costly signaling (costly-signaling)

When to use it: a credential is used to tell high-ability people from low-ability ones.

Equation as the chapter writes it:

    $100,000 - $10,000 = $90,000
    $100,000 - $50,000 = $50,000

Ask the user for: pay with and without the credential, the credential's cost to each type.

Steps:
1. High type: pay with credential minus its cost, compared with pay without (book: 90,000 > 60,000).
2. Low type: pay with credential minus its cost, compared with pay without (book: 50,000 < 60,000).
3. Separation needs both; the low type's break-even cost is the wage gap (book: 40,000). At exactly that cost the low type is indifferent.

Watch for: a separating credential proves incentive compatibility, not that the credential is worth its cost to society.

## 4. Screening and self-selection (screening-self-selection)

When to use it: a seller offers a menu (deductibles, tiers) so that customers sort themselves.

Equation as the chapter writes it:

    $225 + 0.10($500) = $275
    $225 + 0.40($500) = $425

Ask the user for: each plan's premium and deductible, each type's loss probability.

Steps:
1. Expected cost of each plan for each type = premium + probability x deductible (book: 275 and 425 under Plan D, 420 under Plan F).
2. Each type picks its cheapest plan (book: low D, high F).
3. The menu separates only if the types pick different plans (book: yes; at a 175 premium both pick D).

Watch for: risk aversion, administrative costs and changes in care after buying are left out.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
