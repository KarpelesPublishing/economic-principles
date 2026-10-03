---
name: ep-ch043-risk-return-diversification-and-portfolio-choice
description: Apply Chapter 43 of The Encyclopedia of Economic Principals (Risk, Return, Diversification, and Portfolio Choice) to the user's own numbers. Use when someone sets a hurdle rate from beta, asks why checking a portfolio often makes it feel worse, weighs how much of a portfolio to keep at home, or judges how much pooling reduces insurance risk when losses are correlated.
---

# Chapter 43: Risk, Return, Diversification, and Portfolio Choice

Price the risk that cannot be diversified, and diversify the risk that can.

Notebook with the worked examples and figures: `../../notebooks/ch043-risk-return-diversification-and-portfolio-choice.ipynb`

## 1. Capital asset pricing model (capital-asset-pricing-model)

When to use it: setting the required return for a project or security.

    E[R_i]=R_f+\beta_i\big(E[R_M]-R_f\big).

Ask the user for: risk-free rate, expected market return (percent), project beta.

Steps:
1. Market premium (book: 8.5 - 2.5 = 6).
2. Required return (book: 2.5 + 1.3 x 6 = 10.3%; beta 0.8 gives 7.3%).
3. Put risk independent of the market into expected cash flows, not into beta.

Watch for: the market proxy and beta estimate are approximations; other priced factors may matter.

## 2. Myopic loss aversion (myopic-loss-aversion)

When to use it: comparing how a risky position feels when judged each period versus over the whole horizon.

    0.5(15)+0.5\left[2(-10)\right]=-2.5.
    0.25(30)+0.50(5)+0.25\left[2(-20)\right]=0.

Ask the user for: per-period gain and loss, probabilities, loss weight lambda, number of periods.

Steps:
1. Value per look, losses times lambda (book: 7.5 - 10 = -2.5; two looks -5).
2. Aggregate outcomes first, then apply lambda (book: 7.5 + 2.5 - 10 = 0).
3. Compare; with lambda = 1 the two framings tie.

Watch for: a real need to sell after one period makes the separate view the right one.

## 3. Home-bias puzzle (home-bias-puzzle)

When to use it: judging the volatility cost of a home-heavy allocation.

    \sigma_p^2=w^2(0.22)^2+(1-w)^2(0.16)^2 +2w(1-w)(0.30)(0.22)(0.16).

Ask the user for: domestic weight, both volatilities, correlation, world weight.

Steps:
1. Variance at the user's weight (book: 0.027225 + 0.0016 + 0.00396 = 0.032785, volatility 18.11%).
2. Variance at the world weight (book: 0.0231208, volatility 15.21%).
3. Report the gap and whether costs or liabilities justify it.

Watch for: the comparison assumes equal expected net returns.

## 4. Risk pooling, insurance, and diversification (insurance-risk-pooling)

When to use it: sizing the risk of the average loss in a pool.

    0.04(0.96)(5{,}000)^2=960{,}000,
    960{,}000\left(0.10+\frac{0.90}{225}\right)=99{,}840,

Ask the user for: pool size, loss probability, loss size, pairwise correlation, loadings.

Steps:
1. Individual variance p(1 - p)L^2 (book: 960,000, SD 979.80).
2. Average variance = variance x (rho + (1 - rho)/n) (book: 65.32 at rho 0; 315.97 at rho 0.10).
3. Floor sqrt(rho) x individual SD; premium = expected loss plus loadings (book: 200 + 25 + 15 = 240).

Watch for: correlation tends to rise in catastrophes.

## How to answer

- Write each formula, then the user's numbers, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- The chapter's numbers are hypothetical; never present them as data.
