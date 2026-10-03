---
name: ep-ch092-religion-belonging-human-capital-and-social-insurance
description: Apply the principles of Chapter 92 of The Encyclopedia of Economic Principals (Religion, Belonging, Human Capital, and Social Insurance) to the user's own numbers. Use when judging whether an outside service will reduce participation in an organization, how accumulated and specific know-how makes switching costly, how a higher value of time changes participation and output, or how much a mutual-aid fund can cover when losses are correlated.
---

# Chapter 92: Religion, Belonging, Human Capital, and Social Insurance

These principles treat participation as a choice about bundled services, accumulated capital, time and insurance. The chapter's numbers are hypothetical teaching values in utility or resource units, not estimates of real communities.

Notebook with the worked examples and figures: `../../notebooks/ch092-religion-belonging-human-capital-and-social-insurance.ipynb`

## 1. Secularization hypothesis (secularization-hypothesis)

When to use it: predicting whether a new outside service changes participation in an organization that used to supply it.

Equations as the chapter writes them:

    14+9-18=5,
    14+(9-7)-18=-2.

Ask the user for: the core value of participating, the value of each bundled service, the share an outside source now replaces, and the cost of participating.

Steps:
1. Net return = core value + remaining service value - cost (book: 14 + 9 - 18 = 5).
2. Subtract what the outside source replaces (book: 14 + 2 - 18 = -2, Lina stops).
3. Repeat for members with a higher core value (book: Omar 23 + 2 - 18 = 7, keeps attending).

Watch for: lower attendance does not by itself show lower belief; a doubted program replaces less (book: 14 + 7 - 18 = 3).

## 2. Religious human-capital accumulation (religious-human-capital-accumulation)

When to use it: explaining persistence and switching costs when past participation builds a specific stock.

Equations as the chapter writes them:

    K_1^R=0.9(2)+3=4.8.
    (4+1.8)-6=-0.2.

Ask the user for: the current stock, depreciation, how much transfers to the alternative, the benefit rule and the cost.

Steps:
1. Update the stock: K_next = (1 - delta) K + investment (book: 0.9 x 2 + 3 = 4.8).
2. Surplus = benefit with the stock - cost (book: 4 + 4.8 - 6 = 2.8; novice 4 - 6 = -2).
3. Use only transferable capital for the alternative (book: 4 + 1.8 - 6 = -0.2; bridged 3.8 gives 1.8).
4. Decay over idle periods: K (1 - delta)^n (book: 4.8 x 0.9^3 = 3.50).

Watch for: high-capital members may also have stronger preferences; capital is hard to observe.

## 3. Religious household-production model (religious-household-production-model)

When to use it: predicting how hours, purchased inputs and output respond to the value of time.

Equations as the chapter writes them:

    Z=2\sqrt{xt},
    x+4t=100.
    Z=2\sqrt{50(12.5)}=50.

Ask the user for: the full budget, the price of purchased inputs, the value of an hour, and any change in time productivity.

Steps:
1. Equal expenditure shares: x = budget / 2, t = budget / (2 w) (book: x = 50, t = 12.5).
2. Output Z = 2 sqrt(x t) (book: 50; at w = 8, t = 6.25 and Z = 35.36).
3. Apply a time multiplier m as Z = 2 sqrt(x m t) (book: m = 2 restores 50).

Watch for: cash contributions stay at 50 in every case, so they alone hide the change in output.

## 4. Religious organizations as social insurance (religious-organizations-as-social-insurance)

When to use it: sizing what a mutual-aid fund can pay when several members are hit at once.

Equations as the chapter writes them:

    40{,}000-10{,}000-1{,}000+10{,}000=39{,}000.
    40{,}000-10{,}000-1{,}000+2{,}000=31{,}000,

Ask the user for: members, income, the loss, the contribution and how many are hit in the same state.

Steps:
1. Fund = members x contribution (book: 10 x 1,000 = 10,000).
2. Payout = min(loss, fund / claimants) (book: 10,000 for one claimant; 2,000 each for five).
3. Consumption if hit = income - loss - contribution + payout (book: 39,000 or 31,000).

Watch for: pooling redistributes but never restores the loss; contributions must come before the shock.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real community.
