---
name: ep-ch081-land-housing-transport-congestion-and-urban-form
description: Apply Chapter 81 of The Encyclopedia of Economic Principals (Land, Housing, Transport, Congestion, and Urban Form) to the user's own numbers. Use when someone asks how better transit changes a worker's job chances and take-home pay, how much less a household will pay for housing farther from work, which plots or sites earn land rent as prices change, or whether a large operation really has lower cost per unit than a small one.
---

# Chapter 81: Land, Housing, Transport, Congestion, and Urban Form

Price access, distance and land quality: what a trip costs, what a site is worth, and when size lowers unit cost.

Notebook with the worked examples and figures: `../../notebooks/ch081-land-housing-transport-congestion-and-urban-form.ipynb`

## 1. Spatial-mismatch hypothesis (spatial-mismatch-hypothesis)

When to use it: judging how a transit change affects a job seeker.

    1-(1-0.20)^5=1-0.8^5=0.67232;  2($6)+$10=$22

Ask the user for: offer probability per application, the weekly time and cash budget, hours and fare per application, commute hours and fare, value of time, and the daily wage.

Steps:
1. Applications that fit = the smaller of time budget / hours each and cash budget / fare each, rounded down (book: min(15/3, 60/12) = 5; by bus min(15/2, 60/8) = 7).
2. Chance of at least one offer = 1 - (1 - p)^n (book: 1 - 0.8^5 = 0.67232; by bus 0.7902848).
3. Commute cost = hours x value of time + fare (book: 2($6) + $10 = $22; by bus $12).
4. Net daily pay = wage - commute cost (book: $144 - $22 = $122; by bus $132).

Watch for: if reachable jobs need a credential the worker lacks, p is zero and access changes nothing.

## 2. Alonso-Muth-Mills bid-rent gradient (alonso-muth-mills-bid-rent-gradient)

When to use it: how much a household's housing bid must fall with distance from work.

    \frac{\$2{,}000}{1{,}000\text{ square feet}}=\$2;  4(\$2{,}000)=\$8{,}000

Ask the user for: floor area, yearly commuting cost per extra mile, and the bid at a reference site.

Steps:
1. Gradient = cost per mile / floor area (book: $2,000 / 1,000 = $2 per square foot per mile).
2. Extra burden = extra miles x cost per mile (book: 4 x $2,000 = $8,000).
3. New bid = reference bid - extra burden (book: $30,000 - $8,000 = $22,000, or $22 per square foot; rail at $1,000 per mile gives $26).

Watch for: fixed floor area and no amenity differences are assumptions.

## 3. Ricardian rent (ricardian-rent)

When to use it: finding which sites earn rent and how much.

    S_A=10(30)-140=160;  S_D=12(12)-144=0

Ask the user for: output price, each site's yield and delivered cost (including transport).

Steps:
1. Surplus per site = price x yield - delivered cost (book at price 10: 160, 80, 0).
2. The site that just breaks even is the no-rent margin; rents on better sites equal their surplus.
3. A higher price adds yield x price change to each surplus and can bring a new site into use (book at price 12: 220, 124, 28, and D at 0).

Watch for: rank sites by delivered net value, not yield alone. Do not use the chapter's closing access counterfactual for plot D: its numbers do not add up as printed and await an author decision.

## 4. Economies of scale and the latifundia (economies-of-scale-latifundia)

When to use it: comparing unit cost of a large operation with a small one.

    TC_L=1{,}200+25(100)=3{,}700;  1{,}200+25(80)+34(20)=3{,}880

Ask the user for: fixed cost, variable cost per unit (and any higher cost beyond a size), expected throughput, price, and the rival's unit cost.

Steps:
1. Total cost = fixed + variable cost in each tier (book: 3,700; with coordination loss 3,880).
2. Average cost = total / quantity (book: 37 and 38.8, against the small producer's 45).
3. Profit before land cost = price x quantity - total cost (book: 500 and 320; at 50 tons, a loss of 350).

Watch for: use expected throughput, not capacity; an underused fixed cost erases the scale advantage.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied.
- Report ties as ties.
- The chapter's numbers are hypothetical teaching values; never present them as facts about a real city or farm.
