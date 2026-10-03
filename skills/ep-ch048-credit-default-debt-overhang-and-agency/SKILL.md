---
name: ep-ch048-credit-default-debt-overhang-and-agency
description: Apply Chapter 48 of The Encyclopedia of Economic Principals (Credit, Default, Debt Overhang, and Agency) to the user's own numbers. Use when someone asks whether a leveraged firm's owners gain from riskier plans, why a firm with heavy debt turns down a profitable project, how to value equity and debt as options on firm assets, or why a lender refuses to raise its rate and rations credit instead.
---

# Chapter 48: Credit, Default, Debt Overhang, and Agency

Work out who receives the upside and who bears the downside of a debt contract, and what that does to risk taking, investment and lending.

Notebook with the worked examples and figures: `../../notebooks/ch048-credit-default-debt-overhang-and-agency.ipynb`

## 1. Asset-substitution risk shifting (asset-substitution-risk-shifting)

When to use it: owners of a leveraged firm choose between a safe and a risky plan.

    0.55(160)+0.45(20)=97 dollars
    0.55(160-90)+0.45(0)=38.50 dollars
    0.55(70)+0.45(-30)=25 dollars

Ask the user for: debt promise, payoffs and probabilities of each plan, any escrow or covenant.

Steps:
1. Expected enterprise value of each plan (book: safe 115, risky 97).
2. Split each outcome: debt gets min(V, D), equity the rest (book: risky creditors 58.50, equity 38.50; safe 90 and 25).
3. Compare equity across plans (book: gain 13.50 while the firm loses 18).
4. Add an escrow paid to creditors on failure and redo equity net of the deposit (book: 30 gives 25, a tie).

Watch for: the escrow removes the private gain but does not make the risky plan efficient.

## 2. Debt-overhang underinvestment (debt-overhang-underinvestment)

    35-24=11 dollars
    10-24=-14 dollars
    105-70=35 dollars

Ask the user for: assets in place, debt face, investment cost, project payoff.

Steps:
1. Project NPV = payoff minus cost (book: 35 - 24 = 11).
2. Equity with and without the project: max(assets + payoff - face, 0) and max(assets - face, 0) (book: 10 and 0).
3. Private NPV = equity gain minus cost (book: 10 - 24 = -14, rejected).
4. Find the face that flips the decision (book: written down to 70, private NPV 11).

Watch for: new senior money alone does not give shareholders a reason to invest.

## 3. Merton structural default model (merton-structural-default-model)

    E_t=V_tN(d_1)-De^{-r\tau}N(d_2)
    d_1=\frac{\ln(150/120)+(0.03+0.5(0.25)^2)}{0.25}\approx1.138

Ask the user for: asset value V, debt promise D, rate r, horizon tau, asset volatility sigma.

Steps:
1. d1 = (ln(V/D) + (r + sigma^2/2) tau) / (sigma sqrt(tau)), d2 = d1 - sigma sqrt(tau) (book: 1.138, 0.888).
2. Equity = V N(d1) - D e^(-r tau) N(d2) (book: 150(0.87235) - 120e^(-0.03)(0.81262) = 36.22).
3. Debt = V - E (book: 113.78); default probability N(-d2) (book: 18.7 percent).

Watch for: N(-d2) is a pricing probability, not a forecast of real default frequency.

## 4. Stiglitz-Weiss credit rationing (stiglitz-weiss-credit-rationing)

    \frac{12{,}480-12{,}000}{12{,}000}=0.04=4\%
    \frac{12{,}240-12{,}000}{12{,}000}=0.02=2\%

Ask the user for: loan size, the quotes being compared, expected repayment at each quote after default and recovery.

Steps:
1. Return at each quote = (expected repayment - loan) / loan (book: 4 percent at 7 percent, 2 percent at 13 percent).
2. The bank keeps the quote with the higher return and rations the excess demand (book: 80 loans for 140 applicants).
3. Check the counterfactual with borrower mix fixed (book: 12,840 gives 7 percent, so 13 percent would win).

Watch for: the promised repayment (book: 13,560) is not the expected repayment.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and nonbinding cases instead of forcing a result.
- Do not present the book's hypothetical numbers as facts about any real firm or bank.
