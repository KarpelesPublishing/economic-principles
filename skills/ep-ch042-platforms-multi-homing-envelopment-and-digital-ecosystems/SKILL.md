---
name: ep-ch042-platforms-multi-homing-envelopment-and-digital-ecosystems
description: Apply the principles of Chapter 42 of The Encyclopedia of Economic Principals (Platforms, Multi-Homing, Envelopment, and Digital Ecosystems) to the user's own numbers. Use when pricing access to a platform's users, deciding whether to list on a second platform, finding the binding complement in an ecosystem, or valuing a subsidy to one side of a platform.
---

# Chapter 42: Platforms, Multi-Homing, Envelopment, and Digital Ecosystems

These principles tell the user what exclusive reach is worth, when multi-homing pays, which complementary activity limits adoption, and whether a one-sided discount pays through the other side.

Notebook with the worked examples and figures: `../../notebooks/ch042-platforms-multi-homing-envelopment-and-digital-ecosystems.ipynb`

## 1. Competitive bottleneck in two-sided markets (competitive-bottleneck-in-two-sided-markets)

When to use it: pricing access to users who are reachable only through one platform.

Equation as the chapter writes it:

    600(0.07)=42
    42-32-4=6.

Ask the user for: users the platform adds that are not reachable elsewhere, margin per user, fee and integration cost.

Steps:
1. Gross value = unique users x margin (book: 600(0.07) = 42; with 450 overlapping, 150(0.07) = 10.50).
2. Payoff = gross - fee - integration (book: 42 - 32 - 4 = 6).
3. Maximum fee = gross - integration (book: 38, falling to 6.50 with overlap).

Watch for: margin per user stays the same; overlap changes only the reach.

## 2. Multi-homing in two-sided markets (multi-homing-in-two-sided-markets)

When to use it: deciding whether to join a second platform.

Equation as the chapter writes it:

    50(0.40)-12-h=8-h.

Ask the user for: new customers the second platform adds, margin per customer, listing fee and integration cost h.

Steps:
1. Incremental payoff = new customers x margin - listing - h (book at h = 5: 3; at h = 9: -1).
2. Recompute with overlap removed (book: 15(0.40) - 12 - 5 = -11).
3. State the largest overlap that still pays (book at h = 1: 17.5).

Watch for: lowering duplication cost alone cannot rescue a platform that adds few unique customers.

## 3. Complementary Assets and the Ecosystem Effect (complementary-assets-ecosystem-effect)

When to use it: choosing which bottleneck to relieve when several activities must all be ready.

Equation as the chapter writes it:

    A=200\min\{0.92,0.55,0.80,0.70\}=110.

Ask the user for: potential adopters, each activity's readiness share, intervention costs and value per adoption.

Steps:
1. Adoption = potential x smallest share (book: 200 x 0.55 = 110).
2. Relieve the binding activity and find the next one (book: training to 0.75 gives 140, finance binds).
3. Net value = extra adoptions x value - cost (book: 30 x 900 - 15,000 = 12,000).

Watch for: improving a non-binding activity adds nothing (book: finance alone leaves 110).

## 4. Two-Sided Markets, Switching Costs, and Viral Adoption (two-sided-markets-switching-costs)

When to use it: valuing a discount on one side by the participation it draws on the other.

Equation as the chapter writes it:

    n_U=100(4+0.01n_D-p_U),\qquad n_D=10(2+0.005n_U-p_D).

Ask the user for: the two response equations, prices, value per participant on the other side.

Steps:
1. Solve the fixed point (book: n_U = 100/0.95 = 105.26, n_D = 5.2632).
2. Value the other side with the unrounded count (30 x 5.2632 = 157.89; the book multiplies the rounded 5.26 and prints 157.80).
3. Subtract the discount cost on every subsidized participant (157.89 - 105.26 = 52.63; the book prints about 52.54).

Watch for: a bigger discount can lose money (p_U = 2 gives a net of -105.26).

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
