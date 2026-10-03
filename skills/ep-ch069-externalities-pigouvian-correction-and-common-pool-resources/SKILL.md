---
name: ep-ch069-externalities-pigouvian-correction-and-common-pool-resources
description: Apply Chapter 69 of The Encyclopedia of Economic Principals (Externalities, Pigouvian Correction, and Common-Pool Resources) to the user's own numbers. Use when someone asks whether open access is wasting a fishery or other shared resource, what a corrective tax should be or what a miscalibrated one costs, how many teams a prize contest should invite, or how far users of a shared basin overdraw it.
---

# Chapter 69: Externalities, Pigouvian Correction, and Common-Pool Resources

Find the rent that free entry destroys, the tax that matches marginal harm, the prize design that avoids wasteful duplication, and the gap between private and coordinated use of a commons.

Notebook with the worked examples and figures: `../../notebooks/ch069-externalities-pigouvian-correction-and-common-pool-resources.ipynb`

## 1. Gordon open-access rent dissipation (gordon-open-access-rent-dissipation)

When to use it: a resource anyone may harvest, such as a fishery, and the question is what free entry does to its rent.

    G(X)=0.5X(1-X/100);  H=0.01EX;  10(0.01)X=5

Ask for: growth rate and carrying capacity, catchability, price per unit of harvest, cost per unit of effort.

Steps:
1. Open-access stock where effort just pays: X_OA = c/(q p) (book: 5/(0.01 x 10) = 50).
2. Sustainable harvest H = G(X_OA) (book: 0.5 x 50 x 0.5 = 12.5) and effort E = H/(q X) (book: 25).
3. Revenue p H equals cost c E (book: 125 and 125), so rent is zero.
4. Compare a controlled stock (book X = 75: harvest 9.375, effort 12.5, rent 93.75 - 62.50 = 31.25).

Watch for: a higher price only lowers the stock under free entry (book $20: X = 25, rent still 0).

## 2. Pigouvian correction (pigouvian-correction)

When to use it: setting or judging a per-unit tax on a harmful activity.

    100-Q=20+Q+12;  MPC_t(Q)=32+Q

Ask for: marginal benefit and marginal private cost schedules, marginal damage, the tax.

Steps:
1. Untaxed output from MB = MPC (book: Q^p = 40).
2. Efficient output from MB = MPC + damage (book: (80 - 12)/2 = 34).
3. Taxed output from MB = MPC + tax (book: 34 with a $12 tax).
4. If tax and damage differ, the welfare loss with slopes summing to 2 is 0.5 x gap x 2 x gap (derived, not in the book: damage $5, tax $12 gives a gap of 3.5 and a loss of 12.25 thousand dollars).

Watch for: the rate must track marginal harm at the efficient quantity, not the label "corrective".

## 3. Prize incentives and contest design (prize-incentives-contest-design)

When to use it: choosing how many independent teams to fund or invite into a prize.

    q_4=1-0.75^4=0.68359375;  W_4=0.68359375(1,500,000)-320,000=705,390.625

Ask for: value of success V, prize P, cost per team, each team's success probability, the number of teams.

Steps:
1. q_n = 1 - (1 - p)^n (book: 0.68359375).
2. W_n = q_n V - n cost (book: 705,390.625) and compare with the direct contract (book: 0.40 x 1,500,000 - 300,000 = 300,000).
3. Expected prize per team q_n P / n (book: 170,898.4375 > 80,000, so teams enter).
4. Check whether entry continues past the best n (book 12 teams: W falls to 492,485.472 exactly; the book prints an approximate 492,485.475 from rounded q_12; teams still expect 80,693.64).

Watch for: correlated approaches make the independence formula overstate success.

## 4. Tragedy of the commons (tragedy-of-the-commons)

When to use it: several users draw on one stock whose depletion cost they share.

    20-2x-0.2(4x)/4=0;  W(x)=4(20x-x^2)-0.1(4x)^2

Ask for: number of users N, benefit per user a x - x^2, depletion coefficient k.

Steps:
1. Private use x^N = a/(2 + 2k) (book: 20/2.2 = 9.09, total 36.36).
2. Coordinated use x* = a/(2 + 2kN) (book: 20/2.8 = 7.14, total 28.57).
3. Welfare at each, W = N x (a - (1 + kN) x) (book: 264.46 and 285.71, gain 21.25 from a cut of 7.79).

Watch for: identical users and equal sharing are assumptions; real users differ.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
