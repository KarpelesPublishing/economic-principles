---
name: ep-ch088-households-marriage-fertility-and-intergenerational-transfers
description: Apply the principles of Chapter 88 of The Encyclopedia of Economic Principals (Households, Marriage, Fertility, and Intergenerational Transfers) to the user's own numbers. Use when predicting how a change in a partner's fallback shifts a household's choice, dividing home and market work by comparative advantage, judging how many children an old-age security motive implies, or checking whether private gifts will offset a public transfer.
---

# Chapter 88: Households, Marriage, Fertility, and Intergenerational Transfers

These principles treat the household as a small economy: bargaining over fixed resources, specialization, insurance through children, and linked budgets across generations. The chapter's numbers are hypothetical.

Notebook with the worked examples and figures: `../../notebooks/ch088-households-marriage-fertility-and-intergenerational-transfers.ipynb`

## 1. Cooperative household bargaining (cooperative-household-bargaining)

When to use it: predicting which feasible allocation a couple chooses when one partner's fallback changes.

Equations as the chapter writes them:

    N_X=(78-35)(52-32)=43(20)=860
    N_Y=(60-35)(70-32)=25(38)=950

Ask the user for: the utility pairs of each feasible allocation and each partner's disagreement utility.

Steps:
1. Drop any allocation that gives a partner less than the fallback.
2. Nash product of each remaining option (book: 43 x 20 = 860 and 25 x 38 = 950, so Y).
3. Recompute with the new fallback (book, d_A = 45: 660 against 570, so X) and name ties.

Watch for: threat utilities are rarely observed and utility is not comparable across people without structure.

## 2. Gains from marital specialization (gains-from-marital-specialization)

When to use it: deciding who should supply home production and what specializing adds.

Equations as the chapter writes them:

    \frac{32}{2}=\$16
    \frac{45}{1.5}=\$30

Ask the user for: each partner's wage, home productivity, available hours and the home output needed.

Steps:
1. Cost per unit of home output = wage / home productivity (book: 16 and 30).
2. The lower-cost partner supplies the need; the rest of the hours go to the market (book: 96 + 540 = 636 against 510 for an equal split).
3. Repeat when productivity changes (book: Ben at 4 units an hour costs 11.25, income 721.50).

Watch for: career costs, risk and preferences over tasks are left out of the static gain.

## 3. Old-age-security fertility motive (old-age-security-fertility-motive)

When to use it: estimating how many children a security target implies.

Equations as the chapter writes them:

    1-(1-0.55)^3=1-0.45^3=90.8875\%
    1-0.65^4=82.1494\%

Ask the user for: the chance each child can support and the required probability.

Steps:
1. P(n) = 1 - (1 - q)^n (book: 90.89% for 3, 95.90% for 4 at q = 0.55).
2. Smallest n with P(n) at or above the target (book: 4; 6 when q = 0.35).

Watch for: sibling outcomes are often correlated, so extra births diversify less than the formula suggests.

## 4. Altruistic-transfer neutrality (altruistic-transfer-neutrality)

When to use it: checking whether a public transfer between linked family members is offset by private gifts.

Equations as the chapter writes them:

    c_D=84{,}000-4{,}500-7{,}500=\$72{,}000
    c_R=26{,}000+4{,}500+7{,}500=\$38{,}000

Ask the user for: donor and recipient incomes, the donor's current gift and the public transfer.

Steps:
1. New gift = max(0, old gift - transfer) (book: 12,000 - 4,500 = 7,500).
2. Consumption = income minus or plus transfer and gift (book: 72,000 and 38,000, unchanged).
3. If the transfer exceeds the gift, only the gift is crowded out (book: 15,000 gives 69,000 and 41,000).

Watch for: gifts tied to services, general tax financing and future bequests break one-for-one offset.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real household, group or place.
