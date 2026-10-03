---
name: ep-ch030-social-choice-mechanisms-and-strategy-proofness
description: Apply the principles of Chapter 30 of The Encyclopedia of Economic Principals (Social Choice Mechanisms and Strategy-Proofness) to the user's own numbers. Use when checking whether a median rule with phantom voters can be manipulated, computing Clarke pivot payments and the funding gap for a shared project, scoring peer reports with a log rule, or tallying a quadratic vote.
---

# Chapter 30: Social Choice Mechanisms and Strategy-Proofness

These principles show which collective rules make honest reporting safe, and what that safety costs in money or information.

Notebook with the worked examples and figures: `../../notebooks/ch030-social-choice-mechanisms-and-strategy-proofness.ipynb`

## 1. Generalized-median voter schemes (generalized-median-voter-schemes)

When to use it: a group picks a number on a line (a target, a budget) and preferences are single-peaked.

Equations as the chapter writes them:

    15,35,40,50,55,60,65,75,90,
    f(r)=55.
    |60-55|=5

Ask the user for: each participant's reported peak and any fixed phantom points.

Steps:
1. Pool reports and phantoms and sort them (book: 15, 35, 40, 50, 55, 60, 65, 75, 90).
2. Take the middle point as the outcome (book: fifth of nine, 55).
3. Test a misreport by re-sorting (book: reporting 45 instead of 60 gives 50, distance |60 - 50| = 10 > 5).

Watch for: preferences that are not single-peaked (the chapter's grant at exactly 50) break truthful reporting.

## 2. Green-Laffont impossibility (green-laffont-impossibility)

When to use it: pricing a shared project so that everyone reports value honestly.

Equations as the chapter writes them:

    70+55+15=140,
    140-110=30.
    0-(-40)=40.
    40+25+0=65,
    110-65=45.

Ask the user for: each party's value and the project cost.

Steps:
1. Build if total value covers cost (book: 70 + 55 + 15 = 140 >= 110, net 30).
2. For each party, compare the others' best welfare without them to the others' welfare (cost included) with the project (book: owner 1, others 70 < 110, pays 0 - (70 - 110) = 40; owner 2 pays 25; owner 3, others 125 >= 110, pays 0).
3. Sum payments and compare with cost (book: 40 + 25 + 0 = 65, gap 110 - 65 = 45).

Watch for: the gap needs outside money; collusion among parties breaks the incentives.

## 3. Peer-prediction mechanism (peer-prediction-mechanism)

When to use it: paying for reports that cannot be checked against truth, only against a peer.

Equations as the chapter writes them:

    0.75\ln(0.75)+0.25\ln(0.25)\approx -0.562.
    0.75\ln(0.25)+0.25\ln(0.75)\approx -1.112.
    \frac{1}{2}\ln(3)\approx 0.549.

Ask the user for: the probability q that a peer shares the same signal.

Steps:
1. Truthful expected score: q ln q + (1 - q) ln(1 - q) (book: -0.562).
2. False expected score: q ln(1 - q) + (1 - q) ln q (book: -1.112).
3. The advantage is the difference of the unrounded scores (book: ln(3)/2 = 0.549); a constant added to every score changes nothing.

Watch for: at q = 0.5 the advantage is zero; coordinated label swapping is another equilibrium.

## 4. Quadratic voting (quadratic-voting)

When to use it: a vote where intensity should count, priced by credits.

Equations as the chapter writes them:

    v_S=\frac{24}{2}=12
    v_O=\frac{-4}{2}=-2
    12+4(-2)=4,

Ask the user for: each voter's normalized value V (signed).

Steps:
1. Votes v = V/2, credits v^2 (book: supporter 12 votes, 144 credits; each opponent -2 votes, 4 credits).
2. Sum votes (book: 12 + 4(-2) = 4, passes; with V = 14, 7 - 8 = -1, fails).
3. State the value that would tie (book: V = 16 against four opponents).

Watch for: v = V/2 is a continuous benchmark; identity fraud and blocs break it.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
