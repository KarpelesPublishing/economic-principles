---
name: ep-ch046-market-efficiency-behavioral-finance-and-limits-to-arbitrage
description: Apply Chapter 46 of The Encyclopedia of Economic Principals (Market Efficiency, Behavioral Finance, and Limits to Arbitrage) to the user's own numbers. Use when someone asks what price a piece of news justifies, whether a trading rule beats the market after costs, how big a short against an overpriced asset can be before a margin call, what a momentum long-short earned, or how many units a fund must sell when prices fall and clients redeem.
---

# Chapter 46: Market Efficiency, Behavioral Finance, and Limits to Arbitrage

Price news with a benchmark return, net every cost out of an apparent anomaly, and size convergence trades against the funding that can run.

Notebook with the worked examples and figures: `../../notebooks/ch046-market-efficiency-behavioral-finance-and-limits-to-arbitrage.ipynb`

## 1. Efficient-market hypothesis (efficient-market-hypothesis)

When to use it: a report changes an expected payoff, or a backtest shows a gross abnormal return.

    \frac{93.50}{1.10}=85\text{ dollars}.
    0.60\%-0.30\%-0.25\%-0.15\% =-0.10\%.

Ask for: the expected payoff, the required return, the gross abnormal return and each cost per trade.

Steps:
1. Benchmark price = payoff/(1 + r) (book: 93.50/1.10 = 85).
2. Return at that price = payoff/price - 1 (book: 93.50/85 - 1 = 10%, the normal return).
3. Net abnormal = gross minus every cost (book: 0.60 - 0.30 - 0.25 - 0.15 = -0.10%).
4. A positive net result is needed to say the rule beats the benchmark; zero is a tie.

Watch for: a negative result concerns this signal and these costs only.

## 2. Noise-trader risk (noise-trader-risk)

When to use it: shorting an asset believed overpriced when sentiment can push it higher first.

    118-165=-47\text{ dollars}.
    0.5(23)+0.5(-47)=-12\text{ dollars}.

Ask for: position size, current price, plausible interim prices and probabilities, capital available for margin.

Steps:
1. Marked P/L in each interim state = size(p0 - p1) (book: 118 - 95 = 23; 118 - 165 = -47).
2. Expected mark (book: 0.5(23) + 0.5(-47) = -12).
3. Forced close if the adverse loss exceeds capital (book: 47 > 45, closed; half a share loses 23.50 and survives, earning 9 at maturity).

Watch for: being right about value does not protect against the path.

## 3. Momentum effect (momentum-effect)

When to use it: evaluating a winners-minus-losers portfolio over a holding period.

    MOM=8\%-2\%=6\%.
    MOM=-4\%-10\%=-14\%.

Steps: long P/L = leg x winners' return (book: 400,000 x 0.08 = 32,000); short P/L = -leg x losers' return (book: -8,000); MOM = difference (book: 6%); net = MOM minus costs (book: 6% - 4% = 2%). Check the reversal case (book: -14%).

Watch for: one interval does not estimate the effect; apply costs to actual turnover.

## 4. Limits to arbitrage (limits-to-arbitrage)

When to use it: a fund holding a mispriced asset faces a price drop and redemptions.

    10{,}000(80-60)=200{,}000\text{ dollars},
    \frac{200{,}000}{60} =3{,}333.33\text{ units}.

Steps:
1. Loss = units(p0 - p1) (book: 200,000); equity after = equity - loss (book: 800,000).
2. Redemption = share x equity after (book: 0.5 x 800,000 = 400,000).
3. Units sold = max(0, redemption - cash)/p1 (book: 200,000/60 = 3,333.33). With a lockup, none.

Watch for: patient funding fixes the path, not a wrong value estimate.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
