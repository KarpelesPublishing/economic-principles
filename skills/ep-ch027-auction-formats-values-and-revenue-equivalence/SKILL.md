---
name: ep-ch027-auction-formats-values-and-revenue-equivalence
description: Apply Chapter 27 of The Encyclopedia of Economic Principals (Auction Formats, Values, and Revenue Equivalence) to the user's own numbers. Use when someone weighs recruiting another bidder against setting a reserve price, worries about overpaying in a common-value auction, compares first-price and second-price auction revenue, or asks whether rivals' information should change their valuation.
---

# Chapter 27: Auction Formats, Values, and Revenue Equivalence

Who bids, what they know and how they pay decide what an auction earns.

Notebook with the worked examples and figures: `../../notebooks/ch027-auction-formats-values-and-revenue-equivalence.ipynb`

## 1. Bulow-Klemperer theorem (bulow-klemperer-theorem)

When to use it: choosing between an optimal reserve and one more serious bidder.

    phi(v) = 2v - 1;  1/4 + 1/6 = 5/12 approx 0.417;  2/(3 + 1) = 1/2

Steps:
1. Revenue with n bidders and the optimal reserve (book, uniform values, two bidders: 0.25 + 0.167 = 0.417).
2. Revenue with n + 1 bidders and no reserve (book: 2/4 = 0.500).
3. Subtract the cost of recruiting (book: 0.500 - 0.12 = 0.380 < 0.417, so the reserve wins net); break-even cost is the gross gain (book: 1/12).

Watch for: the theorem needs independent private values from a regular distribution.

## 2. The winner's curse in common-value auctions (winners-curse-common-value-auction)

    B_max = V + max_i eps_i;  E[max eps | n = 2] = (-20(1) + 0(3) + 20(5)) / 9 = 80/9 approx $8.89

Steps:
1. List each bidder's possible estimation errors and count how often each is the largest (book, n = 3: 1, 7, 19 of 27).
2. Expected overpayment of a naive winner = expected largest error (book: 360/27 = 13.33).
3. Shade the bid by at least that amount, more as bidders are added.

Watch for: with purely private values there is no curse.

## 3. Revenue-equivalence theorem (revenue-equivalence-theorem)

    E[min(v1, v2)] = $100/3 approx $33.33;  b(v) = v/2;  $100/3 + $10 = $130/3 approx $43.33

Steps:
1. Second price: payment is the second-highest value (book: 50 for values 80 and 50).
2. First price with two uniform bidders: payment is v/2 (book: 40).
3. Expected revenue is equal (book: 33.33 each) unless a condition changes, such as an entry fee (book: 43.33).

Watch for: risk aversion, asymmetry or correlated values break equivalence.

## 4. Affiliation (affiliation)

    Pr(X2 = H | X1 = H) = 0.40/0.50 = 0.80;  0.40(0.40) >= 0.10(0.10);  0.8($100) + 0.2($75) = $95 million

Steps:
1. Conditional probability of a rival's high signal (book: 0.80).
2. Check P(H,H)P(L,L) >= P(H,L)P(L,H) (book: 0.16 >= 0.01); equality means independence.
3. Expected value given one's own signal (book: 95 million).

Watch for: affiliation is a strong condition; negative association reverses the inference.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
