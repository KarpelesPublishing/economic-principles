---
name: ep-ch008-social-choice-voting-and-impossibility
description: Apply Chapter 8 of The Encyclopedia of Economic Principals (Social Choice, Voting, and Impossibility) to the user's own rankings and votes. Use when someone asks whether a sequence of majority votes depends on the agenda, whether a group's preferences produce a coherent majority ranking, which budget or position wins a one-dimensional vote, or whether personal rights and unanimity can conflict.
---

# Chapter 8: Social Choice, Voting, and Impossibility

Count every pairwise contest before trusting a collective ranking, and check which domain restriction makes majority rule coherent.

Notebook with the worked examples and figures: `../../notebooks/ch008-social-choice-voting-and-impossibility.ipynb`

## 1. Condorcet paradox (condorcet-paradox)

    A >_M T >_M O >_M A.

Ask the user for: each voter's ranking and the agenda.

Steps:
1. Tally every pairwise vote (book: A beats T 3 to 2, T beats O 4 to 1, O beats A 3 to 2).
2. Run the agenda: the survivor meets the next option (book: A vs T first, then O, gives O).
3. If one option beats all others it is the Condorcet winner and the agenda does not matter (book: member 5 at A > O > T makes A the winner).

## 2. Arrow's impossibility theorem (arrows-impossibility-theorem)

    R >_M B >_M D >_M R.

Ask the user for: rankings and, if the options lie on one line, their order on it.

Steps:
1. Pairwise tallies (book: each 2 to 1 in a cycle).
2. Check single-peakedness on the line (book: D < B < R with D > B > R, B > D > R, R > B > D).
3. If single-peaked, majority order is transitive (book: B > D > R).

## 3. Median voter theorem (median-voter-theorem)

    (10, 25, 40, 50, 65, 80, 95).

Ask the user for: voters' ideal points and the two proposals.

Steps:
1. Cutline = midpoint of the two proposals (book: (50 + 35) / 2 = 42.5).
2. Count voters on each side (book: 4 to 3 against 35 and against 70).

Watch for: several dimensions can bring cycles back.

## 4. Sen's liberal paradox (sens-liberal-paradox)

    a >_P b >_P c,   b >_L c >_L a,   c > a > b > c

Steps:
1. Each right fixes one comparison (book: a > b for P, c > a for L).
2. Pareto adds any comparison both share (book: b > c).
3. Check for a cycle; if one exists, ask which preferences concern another person's private choice.

## How to answer

- Show every tally as votes for and against.
- Say which rankings are the user's and which you assumed.
- Name ties and cycles instead of forcing a winner.
- Do not present the book's hypothetical profiles as facts about real voters.
