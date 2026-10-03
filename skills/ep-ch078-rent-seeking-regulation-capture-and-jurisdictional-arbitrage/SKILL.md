---
name: ep-ch078-rent-seeking-regulation-capture-and-jurisdictional-arbitrage
description: Apply Chapter 78 of The Encyclopedia of Economic Principals (Rent-Seeking, Regulation, Capture, and Jurisdictional Arbitrage) to the user's own numbers. Use when someone asks where a regulator will set a price between producer and consumer pressure, whether a lobby can buy a tariff against a rival lobby, how much of a contested rent is wasted, or whether a rate cap shuts out a loan and how fees or collateral change that.
---

# Chapter 78: Rent-Seeking, Regulation, Capture, and Jurisdictional Arbitrage

Price a political choice, then separate real resource costs from transfers.

Notebook with the worked examples and figures: `../../notebooks/ch078-rent-seeking-regulation-capture-and-jurisdictional-arbitrage.ipynb`

## 1. Peltzman regulatory equilibrium (peltzman-regulatory-equilibrium)

When to use it: a regulator balances producer support against consumer opposition when setting a markup.

    P(m)=10m-\frac{1}{2}m^2,  O(m)=1.25m^2,  10-m=2.5m,  m^*=\frac{20}{7}\approx2.86

Ask the user for: the competitive benchmark price, the producer support slope a, the opposition coefficient k and the price needed to cover cost.

Steps:
1. Solve a - m = 2km, so m* = a/(1 + 2k) (book: 10/3.5 = 2.86).
2. Price = benchmark + m* (book: 15 + 2.86 = 17.86).
3. Compare with the viability floor (book: k = 2.5 gives 16.67, below 17.25, so not viable).

Watch for: a price above the floor may reflect cost, not capture; check viability first.

## 2. Protection-for-sale model (protection-for-sale-model)

When to use it: a lobby offers a contribution for a binary policy such as a tariff.

    2.5(900-870)=75.  120-90=30  4(30)=120.

Ask the user for: welfare with and without the policy, the welfare weight a, the lobby's gain and offer, any rival offer.

Steps:
1. Weighted loss = a x welfare loss (book: 2.5 x 30 = 75).
2. Policy advantage = offer - weighted loss (book: 90 - 75 = 15); compare with the rival offer (book: 15 < 20, free trade wins).
3. Minimum winning offer exceeds loss + rival offer (book: 95), leaving the lobby less than gain - 95 (book: 25).

Watch for: the binary menu ignores bargaining over tariff levels.

## 3. Rent-seeking, monopoly, and regulatory capture (rent-seeking-and-monopoly)

When to use it: firms spend resources competing for a fixed prize such as a license.

    x_i^*=\frac{5-1}{5^2}(1{,}200)=192.  X^*=5(192)=960.  960+260+60=1{,}280.

Ask the user for: the prize R, the number of contestants n, deadweight loss, administration cost, any useful by-product of lobbying.

Steps:
1. x* = (n - 1)/n^2 x R (book: 192); X* = n x* (book: 960).
2. Social cost = acquisition resources + deadweight + administration (book: 1,280); the prize itself is a transfer.
3. Subtract useful information (book: 960 - 150 = 810); an auction cuts acquisition to bid costs (book: 35).

Watch for: gross lobbying spending is not the same as social waste.

## 4. Usury caps and regulatory arbitrage (usury-caps-and-regulatory-arbitrage)

When to use it: a rate cap may sit below the break-even charge for a loan.

    I^*=\$25+\$55+\$20=\$100,  r^*=\frac{\$100}{\$500}=20\%.  0.12(\$500)=\$60,  \$25+\$15+\$20+\$10=\$70,

Ask the user for: principal, administration cost, expected default loss, required return, the cap, any fees outside the cap, collateral effects.

Steps:
1. Required charge = sum of costs (book: 100, 20 percent).
2. Permitted interest = cap x principal (book: 60); shortfall 40, so the loan is rejected.
3. Fees outside the cap raise the charge collected (book: 60 + 50 = 110); collateral changes cost (book: 70, still 10 short).

Watch for: fee substitution and real cost reduction have different welfare meanings.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied.
- Report ties and break-even cases as such.
- The chapter's numbers are hypothetical teaching values; never present them as facts about a real market.
