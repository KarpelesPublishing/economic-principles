---
name: ep-ch041-network-effects-standards-compatibility-and-tipping
description: Apply the principles of Chapter 41 of The Encyclopedia of Economic Principals (Network Effects, Standards, Compatibility, and Tipping) to the user's own numbers. Use when sizing the launch cohort a network needs, judging whether compatibility reverses a buyer's choice, testing whether an early lead will tip a standards race, or comparing fee splits on a two-sided platform.
---

# Chapter 41: Network Effects, Standards, Compatibility, and Tipping

These principles tell the user how many participants a network needs before joining pays, when an interface changes the winner, and why equal projected receipts can hide very different participation.

Notebook with the worked examples and figures: `../../notebooks/ch041-network-effects-standards-compatibility-and-tipping.ipynb`

## 1. Direct network effects (direct-network-effects)

When to use it: deciding how large a guaranteed first cohort must be.

Equation as the chapter writes it:

    12+0.60(n-1)-30\geq0.

Ask the user for: stand-alone value, fee and value per other member, in the same units.

Steps:
1. Compute n - 1 >= (fee - stand-alone) / value per member (book: (30 - 12) / 0.60 = 30).
2. The smallest integer n is the threshold (book: 31).
3. Check utility just below it (book: 12 + 0.60(29) - 30 = -0.6) and state the cohort that flips the decision.

Watch for: content that adds no reachable members does not move the threshold.

## 2. Compatibility (compatibility)

When to use it: judging whether an interface between two systems changes which one a buyer picks.

Equation as the chapter writes it:

    U_A=16+0.025(480)=28
    U_B=22+0.025(120)=25.

Ask the user for: each system's users and stand-alone value, value per reachable user, and the share of cross-system interactions the interface carries (theta).

Steps:
1. Effective base = own users + theta x other users (book at 0.60 for B: 120 + 0.60(480) = 408).
2. U = stand-alone + value per user x effective base (book: 22 + 0.025(408) = 32.2).
3. Compare and give the theta at which the choice reverses (book: 9 theta > 3, theta above 1/3).

Watch for: a numerical compatibility rate overstates access if the missing functions are the essential ones.

## 3. Market tipping (market-tipping)

When to use it: testing whether an early adoption lead will take over a standards race.

Equation as the chapter writes it:

    3+0.012n_A=3.3+0.012(120-n_A)

Ask the user for: total adopters, each format's stand-alone value and the same-format coefficient k.

Steps:
1. Value each format at the current split (book: 3 + 0.012(75) = 3.90 against 3.3 + 0.012(45) = 3.84).
2. Solve for the crossing n_A = (b - a + kN) / 2k (book: 72.5, so 73 adopters).
3. Say which side adoption moves toward, and how portability (lower k) moves the crossing (book: k 0.004 gives 97.5).

Watch for: large coordinated adopters can jump expectations past the crossing.

## 4. Platform Economics and Two-Sided Markets (platform-two-sided)

When to use it: comparing fee splits between the two sides of a platform.

Equation as the chapter writes it:

    3+0.40(30)-9=6,
    0.20(150)-18=12.

Ask the user for: participants and values on each side, serving costs and the proposed fee pairs.

Steps:
1. Check each side's utility at full participation (book: buyers 6, sellers 12).
2. Remove any side with negative utility and recompute the other side (book: fees 16 and -17 give buyer utility -1, so buyers leave).
3. Compute profit from actual participants, not projected receipts (book: 1,350 against -750).

Watch for: projected receipts at fixed quantities are the same for every split and say nothing about participation.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
