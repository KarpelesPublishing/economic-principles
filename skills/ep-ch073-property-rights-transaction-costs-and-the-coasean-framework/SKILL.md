---
name: ep-ch073-property-rights-transaction-costs-and-the-coasean-framework
description: Apply Chapter 73 of The Encyclopedia of Economic Principals (Property Rights, Transaction Costs, and the Coasean Framework) to the user's own numbers. Use when someone asks whether private bargaining will settle a nuisance under a given legal right, how large a corrective charge should be, who should own a shared asset when both parties must invest, or whether to make a component in house or buy it.
---

# Chapter 73: Property Rights, Transaction Costs, and the Coasean Framework

Decide when rights and bargaining costs change outcomes, and compare governance options by their full cost.

Notebook with the worked examples and figures: `../../notebooks/ch073-property-rights-transaction-costs-and-the-coasean-framework.ipynb`

## 1. Coase theorem (coase-theorem)

When to use it: a conflict between an activity and the people it harms, with a legal right assigned to one side.

    joint surplus = profit - harm

Ask the user for: the activity's profit, the harm, who holds the right and the cost of striking a deal.

Steps:
1. Efficient outcome (book: 140 - 85 = 55, so operating is efficient).
2. Baseline under the right, and the gain from moving away from it.
3. A deal happens only if that gain exceeds the bargaining cost; payments lie between harm and profit (book: 85 to 140; at 100 the operator keeps 140 - 100 = 40 and the resident nets 100 - 85 = 15).
4. Book: with harm 170 and a right to fly, shutdown gains 30, which cannot cover a cost of 40, so the route keeps operating.

Watch for: many parties or hidden values raise bargaining costs.

## 2. Externalities (externalities)

When to use it: setting a per-unit charge for damage caused by each unit of output.

    W(q) = q x price - private costs of the first q units - q x damage

Steps:
1. Social margins (book: 40 - 19 = 21, 40 - 27 = 13, 40 - 35 = 5, 40 - 43 = -3; efficient quantity 3).
2. The producer's choice under the charge (book: no charge gives 4; a charge of 9 gives 3).
3. Welfare at each (book: W(3) = 120 - 54 - 27 = 39; W(4) = 160 - 88 - 36 = 36).

Watch for: a constant charge fits only if damage per unit is constant.

## 3. Incomplete contracts (incomplete-contracts)

When to use it: choosing ownership when two parties make investments a court cannot verify.

    c_A(a) = a^2/2, c_B(b) = b^2/2;  a = share_A x 8, b = share_B x 8

Steps:
1. Investments from each party's share (book: 0.5 x 8 = 4 each; ownership by A gives 6 and 2).
2. Net surplus 8a + 8b - a^2/2 - b^2/2 (book: 48 balanced; 8(6) + 8(2) - 18 - 2 = 44 with A as owner; first best 64).
3. Choose the ownership with the higher total.

Watch for: if one party's investment is much more productive, giving it the asset can rank first.

## 4. Transaction costs (transaction-costs)

When to use it: make or buy.

    TC_M = production + search + drafting + monitoring + adaptation;  TC_F = production + management + measurement + rigidity

Steps:
1. Market total (book: 2,160 + 150 + 360 + 220 + 520 = 3,410).
2. Firm total (book: 2,640 + 260 + 170 + 220 = 3,290; integration saves 120).
3. Redo with changed contracting costs (book: drafting 80 and adaptation 160 give 2,770, so buying is 520 cheaper).

Watch for: quality, capacity and strategic control need their own entries.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
