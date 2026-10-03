---
name: ep-ch090-networks-trust-enforcement-and-collective-behavior
description: Apply the principles of Chapter 90 of The Encyclopedia of Economic Principals (Networks, Trust, Enforcement, and Collective Behavior) to the user's own numbers. Use when valuing a nonredundant contact in a search, checking whether shared partners make default unprofitable, diagnosing why a valuable link goes unbuilt, or testing whether reputation and a bond deter an agent from cheating.
---

# Chapter 90: Networks, Trust, Enforcement, and Collective Behavior

These principles price what network ties carry and enforce. The chapter's numbers are hypothetical.

Notebook with the worked examples and figures: `../../notebooks/ch090-networks-trust-enforcement-and-collective-behavior.ipynb`

## 1. Strength of weak ties (strength-of-weak-ties)

When to use it: valuing a contact who reaches a different information pool.

Equations as the chapter writes them:

    0.30(0.50)=0.15
    1-(1-0.40)(1-0.15)=0.49

Ask the user for: the chance the existing circle yields a lead, the contact's chance of seeing one, forwarding and overlap.

Steps:
1. Contact's new information = sees x forwards x (1 - overlap) (book: 0.15; with 80% overlap, 0.03).
2. P(lead) = 1 - product of (1 - p) over independent pools (book: 0.49; 0.418 with overlap).

Watch for: a lead is not a job; qualifications and applications are separate stages.

## 2. Network closure as an enforcement mechanism (network-closure-as-an-enforcement-mechanism)

When to use it: checking whether default on a promise is deterred.

Equations as the chapter writes them:

    d\leq p(C_{ij})S(C_{ij})
    0.80(\$2{,}000)=\$1{,}600

Ask the user for: the gain from default, detection probability and sanction at stake.

Steps:
1. Expected consequence pS (book: 0.20 x 1,500 = 300; 0.80 x 2,000 = 1,600).
2. Compare with the gain (book: 1,600 - 1,000 = 600, so repay); name exact ties.

Watch for: more ties without shared information or coordinated sanctions change nothing.

## 3. Strategic network formation (strategic-network-formation)

When to use it: explaining a missing link and the transfer that would fix it.

Equations as the chapter writes them:

    10-12=-2
    10+10-12=8

Ask the user for: each party's value from the link, its cost and who pays.

Steps:
1. Sponsor's payoff = own value + transfer - cost (book: -2; with a 3 transfer, 1).
2. Social surplus = all values - cost (book: 8).
3. Positive social surplus with a negative sponsor payoff signals a missing transfer.

Watch for: if the other party's benefit is absent, no link is also efficient.

## 4. Diaspora networks and middleman minorities (diaspora-middleman)

When to use it: testing whether reputation plus a bond makes honest agency incentive compatible.

Equations as the chapter writes them:

    pF\geq g
    0.9(6{,}000)(1+0.9+0.9^2+0.9^3)=18{,}570.60

Ask the user for: gain from cheating, future payments, discount factor, detection chance and bond.

Steps:
1. Lost business = p x payment x (1 + delta + ... ) (book: 18,570.60).
2. Add the expected bond loss p x bond (book: 2,700; total 21,270.60).
3. Compare with the gain (book: above 20,000, honest; at p = 0.4 only 9,453.60).

Watch for: shared origin matters only through detection and enforcement.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real household, group or place.
