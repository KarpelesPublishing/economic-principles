---
name: ep-ch037-natural-monopoly-regulation-and-public-utility-pricing
description: Apply the principles of Chapter 37 of The Encyclopedia of Economic Principals (Natural Monopoly, Regulation, and Public-Utility Pricing) to the user's own numbers. Use when pricing shared capacity by time of use, testing whether one supplier is cheaper than several, setting markups to cover a deficit, or judging the cost of a price ceiling.
---

# Chapter 37: Natural Monopoly, Regulation, and Public-Utility Pricing

These principles let the user decide who should pay for capacity, whether a market is a natural monopoly, how to spread required markups, and what a binding price ceiling costs.

Notebook with the worked examples and figures: `../../notebooks/ch037-natural-monopoly-regulation-and-public-utility-pricing.ipynb`

## 1. Peak-load pricing (peak-load-pricing)

When to use it: a facility is full at some times and idle at others.

Equation as the chapter writes it:

    p_O=20,\qquad p_P=20+40=60

Ask the user for: demand in each period, operating cost and capacity cost per unit.

Steps:
1. Off-peak price = operating cost (book: 20); peak price = operating cost + capacity cost (book: 60).
2. Quantities from each demand (book: q_O = 80, q_P = 100).
3. Capacity K = peak quantity and idle off-peak capacity (book: K = 100, idle 20). Check the off-peak quantity stays below K; if not, both periods share the capacity cost.

Watch for: a uniform price (book: 40) shifts use to the peak and needs more capacity (K = 120).

## 2. Natural monopoly by subadditivity (natural-monopoly-by-subadditivity)

When to use it: deciding whether one supplier serves a market more cheaply than several.

Equation as the chapter writes it:

    C(q)=100+2q,\qquad 0<q\leq100
    C(q)=40+q+0.02q^2

Ask the user for: total demand and the cost function of one supplier.

Steps:
1. Cost of one firm serving all demand (book: 300 linear, 340 congestion).
2. Cost of realistic splits (book: linear 60/40 split 400; congestion 2 x 140 = 280).
3. State whether subadditivity holds: one firm cheapest means yes.

Watch for: the number of firms observed does not reveal which technology applies.

## 3. Ramsey-Boiteux pricing (ramsey-boiteux-pricing)

When to use it: a regulated service must raise a set amount through markups on several products.

Equation as the chapter writes it:

    1{,}000(m_C+m_L)=900,\qquad m_C+m_L=0.90

Ask the user for: marginal cost, initial quantities, the revenue target and each product's elasticity.

Steps:
1. Total markup = target / quantity (book: 900 / 1,000 = 0.90).
2. Split by inverse elasticity m_C / m_L = e_L / e_C (book: 2 / 0.5 = 4, so 0.72 and 0.18).
3. Lost quantity e x (m / p) x q and deadweight loss (1/2) m |dq| (book: 180 and 180, 64.80 + 16.20 = 81; uniform 0.45 gives 126.56).

Watch for: this is a small-change approximation; large markups need the full demand curves.

## 4. Price controls and rationing (price-controls-rationing)

When to use it: a price ceiling is set below the market-clearing price.

Equation as the chapter writes it:

    Q_D=120-2p,\qquad Q_S=3p
    \int_0^{36}\left(60-\frac{q}{2}-\frac{q}{3}\right)dq =\$1{,}620

Ask the user for: demand and supply schedules, the ceiling and any queuing or search cost.

Steps:
1. Clearing price and quantity (book: 24 and 72).
2. Demand, supply and shortage at the ceiling (book: 96, 36, 60).
3. Marginal willingness to pay at the supplied quantity (book: $42, a resale premium up to $30).
4. Surplus on the supplied units against the benchmark (book: 1,620 against 2,160, a loss of 540) and after queuing (book: 1,320).

Watch for: a ceiling at or above the clearing price does not bind and creates no queue.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
