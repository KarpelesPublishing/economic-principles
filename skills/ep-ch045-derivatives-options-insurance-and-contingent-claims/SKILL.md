---
name: ep-ch045-derivatives-options-insurance-and-contingent-claims
description: Apply Chapter 45 of The Encyclopedia of Economic Principals (Derivatives, Options, Insurance, and Contingent Claims) to the user's own numbers. Use when someone prices a European call and its delta hedge, prices a loan that is repaid only if a venture succeeds, sets an insurance premium and checks how correlated losses change claim uncertainty, or tests option quotes against put-call parity.
---

# Chapter 45: Derivatives, Options, Insurance, and Contingent Claims

Price a contingent claim by the cost of a position that delivers the same payoff, and separate what moves the mean from what moves the risk.

Notebook with the worked examples and figures: `../../notebooks/ch045-derivatives-options-insurance-and-contingent-claims.ipynb`

## 1. Black-Scholes-Merton option pricing (black-scholes-merton-option-pricing)

When to use it: valuing a European call on a non-dividend stock and sizing its hedge.

    C = S_0 N(d_1) - K e^{-rT} N(d_2)
    d_1 = [ln(S_0/K) + (r + sigma^2/2) T] / (sigma sqrt(T));  d_2 = d_1 - sigma sqrt(T)

Ask the user for: stock price, strike, years to expiry, continuously compounded rate, annual volatility.

Steps:
1. d_1 and d_2 (book: S_0 80, K 85, T 0.5, r 0.04, sigma 0.25 gives d_1 = -0.1414, d_2 = -0.3182).
2. N(d_1), N(d_2) and C (book: 80 x 0.4438 - 85 e^{-0.02} x 0.3752 = 4.24).
3. Hedge = number of calls x N(d_1) (book: 500 x 0.4438 = 221.9 shares). At sigma 0.35 the call is 6.49.

Watch for: constant volatility and costless continuous rebalancing are assumptions; real hedges leak.

## 2. Bottomry loans as options and futures (bottomry-as-options-futures)

When to use it: a loan forgiven if the venture fails.

    qR = L(1 + r) + k;  R = [L(1 + r) + k] / q

Steps:
1. Required expected receipt (book: 120,000 x 1.03 + 3,000 = 126,600).
2. R = receipt / q (book: 126,600 / 0.75 = 168,800; at q 0.60, 211,000).
3. Borrower's expected proceeds q(V - R) (book: 0.75(230,000 - 168,800) = 45,900; at q 0.60, 11,400).

Watch for: q is an estimate; the charge may also include bargaining rents.

## 3. Maritime insurance and risk pricing (maritime-insurance-risk-pricing)

    pi = pI + a + rho
    SD(L_N/N) = I sqrt(p(1 - p)[1/N + c(1 - 1/N)])

Steps:
1. Premium (book: 0.016 x 750,000 + 2,400 + 1,600 = 16,000).
2. SD of average claims (book: 7,842.19 with c = 0 and N = 144; 27,659.72 with c = 0.08, about 3.53 times).
3. Correlation changes the SD, not the expected claim; frequency changes both.

Watch for: a single pairwise correlation is a simplification of common shocks.

## 4. Put-call parity (put-call-parity)

    C_0 + K e^{-rT} = P_0 + S_0

Steps:
1. Cost of call plus bond and of put plus stock (book: 5.20 + 48.50 = 53.70; 2.40 + 52 = 54.40).
2. Buy the cheaper, sell the dearer; the gap is the receipt (book: 0.70). Both pay max(S_T, K) at expiry.
3. Trade only if the gap exceeds all costs (with costs 0.85: 0.70 - 0.85 = -0.15, no trade).

Watch for: shorting, borrow fees and collateral can absorb the gap.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties (a zero parity gap) instead of forcing a trade.
- The chapter's numbers are hypothetical; do not present them as facts about any real market.
