---
name: ep-ch052-bank-runs-collateral-cycles-crisis-backstops-and-sovereign-links
description: Apply the principles of Chapter 52 of The Encyclopedia of Economic Principals (Bank Runs, Collateral Cycles, Crisis Backstops, and Sovereign Links) to the user's own numbers. Use when judging how a fall in collateral prices cuts borrowing capacity, how much cash a repo borrower must replace when haircuts rise, whether a bank is exposed to a self-fulfilling run, or what a fire sale costs compared with central bank lending.
---

# Chapter 52: Bank Runs, Collateral Cycles, Crisis Backstops, and Sovereign Links

These principles let the user measure how funding stress turns into losses: through collateral values, haircuts, withdrawal expectations and forced sales.

Notebook with the worked examples and figures: `../../notebooks/ch052-bank-runs-collateral-cycles-crisis-backstops-and-sovereign-links.ipynb`

## 1. Kiyotaki-Moore collateral cycle (kiyotaki-moore-collateral-cycle)

When to use it: a borrower's credit limit depends on the market value of assets that other leveraged owners may sell at the same time.

Equations as the chapter writes them:

    0.65(960{,}000)=624{,}000
    0.65(816{,}000)=530{,}400

Ask the user for: units of collateral, price before and after, pledgeable share, internal funds, cash shock.

Steps:
1. Capacity before = funds + share x units x old price (book: 360,000 + 0.65 x 12 x 80,000 = 984,000).
2. Capacity after = (funds - shock) + share x units x new price (book: 270,000 + 530,400 = 800,400).
3. Split the decline into the cash loss and the repricing part, share x units x price fall (book: 90,000 and 93,600).

Watch for: the feedback depends on the assumed clearing price; it is not a universal multiplier.

## 2. Run on repo (run-on-repo)

When to use it: a borrower funds securities overnight and lenders can raise haircuts at rollover.

Equations as the chapter writes them:

    (1-0.04)(240)=230.4
    0.88(238)=209.44

Ask the user for: collateral value, old and new haircut, value at rollover.

Steps:
1. Old funding = (1 - old haircut) x value (book: 0.96 x 240 = 230.4).
2. New funding = (1 - new haircut) x value at rollover (book: 0.88 x 238 = 209.44).
3. Cash to replace = old - new (book: 20.96), split into haircut part (19.2) and markdown part (0.88 x 2 = 1.76); compare with market equity (238 - 230.4 = 7.6).

Watch for: assumes no spare cash or unsecured line.

## 3. Diamond-Dybvig bank-run mechanism (diamond-dybvig-bank-run-mechanism)

When to use it: deciding whether a bank's promised liquid payouts exceed what its assets fetch if liquidated at once.

Equations as the chapter writes them:

    c_2=\frac{87.36}{64}=1.365
    0.20(1.10)+\frac{0.80(1.365)}{1.40}=0.22+0.78=1

Ask the user for: depositors N, long return R, impatient share, early payment c1.

Steps:
1. Interrupted = impatient count x c1 (book: 16 x 1.10 = 17.6).
2. c2 = (N - interrupted) x R / patient count (book: 62.4 x 1.40 / 64 = 1.365); if c2 is above c1, waiting pays when others wait.
3. In a run, full payments = floor(N / c1) (book: 72, paying 79.2 and leaving 0.8); loss = no-run total - N (book: 104.96 - 80 = 24.96).

Watch for: assumes sequential service and no deposit insurance.

## 4. Lender of last resort (lender-of-last-resort)

When to use it: comparing a forced asset sale with borrowing from a central bank facility.

Equation as the chapter writes it:

    \frac{20}{1-0.20}=25

Ask the user for: cash, loans, deposits, run size, fire-sale price, facility haircut, rate and days.

Steps:
1. Gap = run - cash (book: 38 - 18 = 20).
2. Fire sale: loans sold = gap / price (book: 30.769); equity = loans kept - remaining deposits (book: 59.231 - 42 = 17.231).
3. Facility: collateral = gap / (1 - haircut) (book: 25); equity stays 90 - 42 - 20 = 28 before interest of 20 x 0.08 x 60 / 365 = 0.263.

Watch for: lending cannot repair a bank whose assets are worth less than its deposits.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
