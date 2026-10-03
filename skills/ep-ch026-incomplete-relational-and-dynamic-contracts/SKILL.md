---
name: ep-ch026-incomplete-relational-and-dynamic-contracts
description: Apply Chapter 26 of The Encyclopedia of Economic Principals (Incomplete, Relational, and Dynamic Contracts) to the user's own numbers. Use when someone prices a loan whose bad outcomes must be audited, asks whether an unenforceable bonus or promise will be honoured, checks whether a seller's reputation is worth more than cheating, or asks whether a party will make a relationship-specific investment that the other side can hold up.
---

# Chapter 26: Incomplete, Relational, and Dynamic Contracts

When courts cannot see the facts, audits, the value of the future and ownership decide which deals hold together.

Notebook with the worked examples and figures: `../../notebooks/ch026-incomplete-relational-and-dynamic-contracts.ipynb`

## 1. Costly state verification (costly-state-verification)

When to use it: a lender can verify a borrower's outcome only at a cost.

    0.25($40 - $10) + 0.75D = $80;  D = ($80 - 0.25($30)) / 0.75 = $96.67

Ask the user for: loan, outcomes and probabilities, audit cost.

Steps:
1. Low-state recovery = low return - audit cost (book: 40 - 10 = 30).
2. Break-even face value D = (loan - p_low x recovery) / (1 - p_low) (book: 72.50 / 0.75 = 96.67).
3. Expected audit cost p_low x c (book: 2.50) is the deadweight loss; surplus = expected output - loan - expected audit (book: 115 - 80 - 2.50 = 32.50).

Watch for: the lender must be committed to audit even when recovery is negative.

## 2. Relational contracts (relational-contracts)

When to use it: a promise cannot be enforced in court but the relationship repeats.

    $50 - $30 = $20;  $90 - $50 = $40;  (0.8 / (1 - 0.8)) x $40 = $160

Ask the user for: the one-time saving from reneging, the per-period gain from cooperation, the continuation factor delta.

Steps:
1. Future loss = delta / (1 - delta) x per-period gain (book: 4 x 40 = 160).
2. Compare with the temptation (book: 160 >= 50, self-enforcing; at delta 0.2 only 10 < 50).
3. State the decision and the delta that would flip it.

Watch for: renegotiation after a breach weakens the punishment.

## 3. Reputation as contract-enforcement capital (reputation-capital)

When to use it: a seller could secretly cut quality once.

    pi^C = $90 - $70 = $20;  G = $70 - $40 = $30;  $30 <= (delta / (1 - delta)) x $20

Steps:
1. Rent at risk = delta / (1 - delta) x honest profit, plus any separate asset B lost on detection (book: 3 x 20 = 60).
2. Honest if rent >= cheating gain (book: 60 >= 30); threshold delta = (G - B) / (G - B + profit) (book: 0.6).
3. Report an exact equality as a tie that just sustains honesty.

Watch for: slow or uncertain detection lowers the rent at risk.

## 4. Hold-up problem (hold-up-problem)

When to use it: one party sinks a specific investment and bargains afterwards.

    $100 - $40 = $60 million;  $60 - $35 = $25 million;  0.70($60) = $42 million

Steps:
1. Increment and joint net gain (book: 60 and 60 - 35 = 25).
2. Investor's private return = share x increment (book: 0.5 x 60 = 30 < 35, declines).
3. Minimum share = cost / increment (book: 35 / 60 = 0.583).

Watch for: shifting ownership can weaken the other side's own investment.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
