---
name: ep-ch039-innovation-incentives-creative-destruction-and-patent-races
description: Apply Chapter 39 of The Encyclopedia of Economic Principals (Innovation Incentives, Creative Destruction, and Patent Races) to the user's own numbers. Use when someone asks how many firms will enter a race for one prize and how much is spent, whether an incumbent or an entrant will pay to speed up research, why an incumbent gains less from an invention than an entrant, or how prize size and field size change contest effort.
---

# Chapter 39: Innovation Incentives, Creative Destruction, and Patent Races

Count entrants and wasted spending in a race, compare incumbent and entrant motives, and size effort in a prize contest.

Notebook with the worked examples and figures: `../../notebooks/ch039-innovation-incentives-creative-destruction-and-patent-races.ipynb`

## 1. Patent-race rent dissipation (patent-race-rent-dissipation)

When to use it: several equally likely labs racing for one prize.

    90 - 20 = 70,   90/4 - 20 = 2.5

Ask the user for: prize value, entry cost per lab.

Steps:
1. Payoff per lab with n labs is V/n - F (book: 90/4 - 20 = 2.5).
2. Entry stops at the largest n with a payoff not below zero (book: 90/5 - 20 = -2, so n = 4).
3. Total spending n F and rent left V - nF (book: 80 and 10). A lab that exactly breaks even is a tie; say so.

Watch for: losing programs that produce reusable knowledge, which reduce the true waste.

## 2. Patent-race preemption (patent-race-preemption)

    P_I = 100 - 25 = 75,   0.20(75) = 15 > 12,   0.20(40) = 8 < 12

Ask the user for: incumbent value if it wins and if it loses, entrant prize, probability gain, program cost.

Steps:
1. Incumbent prize = value if it wins minus value kept if the entrant wins (book: 75).
2. Benefit = probability gain x prize for each firm (book: 15 and 11).
3. A firm buys if benefit exceeds cost (book: incumbent buys, entrant does not; kept value 60 gives 8 < 12).

Watch for: if the incumbent keeps its value whoever wins, this is the replacement effect instead.

## 3. Arrow replacement effect (arrow-replacement-effect)

    Q_M(c) = (100 - c)/2,   (80 - 60)20 = $400,   1,600 - 400 = $1,200,   (60 - 20)40 = $1,600

Ask the user for: demand, old and new unit cost, the incumbent's current profit, the entrant's rent, the outlay.

Steps:
1. Profit with the new cost (book: 40 units at 60, 1,600).
2. Incumbent gain = new profit minus old profit (book: 1,200); entrant gain = full rent (book: 1,600).
3. Compare each with the outlay (book: 1,400, so only the entrant; with old profit 100, gain 1,500 and both invest).

Watch for: the entrant rent is stipulated at the old competitive price.

## 4. Prize incentives and contest design (prize-incentives-contest)

    e* = rV(n - 1)/(c n^2),   e* = 100(4 - 1)/4^2 = 18.75

Ask the user for: prize V, number of teams n, effort cost c, decisiveness r.

Steps:
1. Effort per team (book: 18.75).
2. Payoff per team V/n - c e* (book: 25 - 18.75 = 6.25); aggregate n e* (book: 75).
3. Compare field sizes (book: 2 teams give 25 each, 50 in all).

Watch for: the welfare test values what the effort produces, not the size of the transfer.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
