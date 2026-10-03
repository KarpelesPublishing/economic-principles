---
name: ep-ch028-optimal-auctions-multi-unit-sales-and-package-bidding
description: Apply the principles of Chapter 28 of The Encyclopedia of Economic Principals (Optimal Auctions, Multi-Unit Sales, and Package Bidding) to the user's own numbers. Use when checking whether VCG prices in a package auction can be blocked, setting a revenue-maximizing reserve, judging side bets on correlated bidder types, or spotting demand reduction in a uniform-price sale.
---

# Chapter 28: Optimal Auctions, Multi-Unit Sales, and Package Bidding

These principles let the user price a package auction so no coalition can undercut it, choose a reserve, see when correlation lets a seller extract every rent, and predict when large bidders shade multi-unit demand.

Notebook with the worked examples and figures: `../../notebooks/ch028-optimal-auctions-multi-unit-sales-and-package-bidding.ipynb`

## 1. Core-selecting package auctions (core-selecting-package-auctions)

When to use it: package and single-item bidders compete and VCG revenue looks low.

Equations as the chapter writes them:

    60+60=120>100
    p_A^{VCG}=100-60=40
    p_A+p_B\geq100
    (p_A,p_B)=(50,50)

Ask the user for: each bidder's package and bid.

Steps:
1. Find the welfare-maximizing allocation (book: 60 + 60 = 120 > 100, locals win).
2. VCG payment of each winner = best welfare without it minus the others' value with it (book: 100 - 60 = 40 each, revenue 80).
3. Compare revenue with each losing coalition's bid; if lower, raise payments to the minimum core point (book: 80 < 100, symmetric core (50, 50)).
4. Check each payment stays below the winner's bid, and state whether the outcome was blocked.

Watch for: core payments give up exact truth-telling incentives.

## 2. Myerson optimal-auction theorem (myerson-optimal-auction-theorem)

When to use it: setting a reserve price for independent private values.

Equation as the chapter writes it:

    \phi(v)=v-\frac{1-v/100}{1/100}=2v-100

Ask the user for: the value distribution (bounds if uniform), the seller's own value, and any bid profile to check.

Steps:
1. Compute the virtual value and the reserve where it equals the seller's value (book: 2v - 100 = 0 at v = 50).
2. For a profile, the highest bidder wins if above the reserve and pays max(second bid, reserve) (book: (80, 40) pays 50, utility 30).
3. Compare expected revenue with and without the reserve (book: 125/3 = 41.67 against 100/3 = 33.33).

Watch for: the seller must commit not to resell after a no-sale.

## 3. Cremer-McLean full-surplus extraction (cremer-mclean-full-surplus-extraction)

When to use it: bidders' types are correlated and the seller can bet on rival reports.

Equations as the chapter writes them:

    \Pr(B=H\mid A=H)=\frac{0.4}{0.5}=0.8
    0.8\left(\frac{80}{3}\right)-0.2\left(\frac{20}{3}\right)=20
    0.2\left(\frac{80}{3}\right)-0.8\left(\frac{20}{3}\right)=0

Ask the user for: the joint type distribution and each type's interim rent.

Steps:
1. Compute each type's belief about the rival (book: 0.8 and 0.2).
2. Solve for a charge x and rebate y with high-type expected cost equal to its rent and low-type cost zero (book: x = 80/3, y = 20/3).
3. If the beliefs are equal, say the rank condition fails and no such bet exists.

Watch for: full extraction needs known correlation, risk neutrality and unlimited liability.

## 4. Demand reduction (demand-reduction)

When to use it: a uniform-price sale of identical units to bidders who want several.

Equations as the chapter writes them:

    (100-70)+(90-70)=50
    100-0=100
    100+90-70=120

Ask the user for: each bidder's marginal values and the supply.

Steps:
1. Truthful: top bids win, all pay the highest rejected bid (book: price 70, A earns 50).
2. Shaded: drop the bidder's marginal unit and recompute the price (book: price 0, A earns 100).
3. Report the efficiency loss and the Vickrey comparison (book: 270 - 250 = 20 lost; Vickrey utility 120 > 100).

Watch for: the result assumes rivals bid truthfully.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
