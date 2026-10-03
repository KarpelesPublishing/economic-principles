---
name: ep-ch094-health-capital-medical-uncertainty-and-provider-incentives
description: Apply the principles of Chapter 94 of The Encyclopedia of Economic Principals (Health Capital, Medical Uncertainty, and Provider Incentives) to the user's own numbers. Use when deciding whether a review or second opinion saves money, whether an insurance pool is entering a premium spiral and whether reinsurance stops it, how depreciation and technology change the spending needed to maintain health, or how cost sharing changes visits and their resource cost.
---

# Chapter 94: Health Capital, Medical Uncertainty, and Provider Incentives

These principles separate pooling, screening, health as a stock and the price a patient sees. The chapter's numbers are hypothetical teaching values in resource units, not clinical or market data.

Notebook with the worked examples and figures: `../../notebooks/ch094-health-capital-medical-uncertainty-and-provider-incentives.ipynb`

## 1. Arrow medical-care uncertainty principle (arrow-medical-care-uncertainty-principle)

When to use it: valuing an independent review before costly treatment.

Equations as the chapter writes them:

    28(20{,}000)=560{,}000\text{ units}.
    28(1{,}000)+16(20{,}000)=348{,}000\text{ units},

Ask the user for: positive cases, procedure cost, review fee per case and false positives the review removes.

Steps:
1. Automatic cost = positives x procedure (book: 560,000).
2. Reviewed cost = positives x fee + remaining procedures x cost (book: 28,000 + 320,000 = 348,000).
3. Saving = difference (book: 212,000).

Watch for: a reviewer paid per procedure may not filter as assumed.

## 2. Health-insurance adverse-selection death spiral (health-insurance-adverse-selection-death-spiral)

When to use it: checking whether a break-even premium drives out low-risk members round after round.

Equations as the chapter writes them:

    p_{t+1}=k+E[c_i\mid v_i-p_t\geq o_i].
    \frac{600(2{,}000)+400(8{,}000)}{1{,}000}=4{,}400\text{ units}.

Ask the user for: members and expected claims by risk group, renewal thresholds, and any reinsurance.

Steps:
1. Premium = total expected claims of renewing members / members (book: 4,400).
2. Drop groups whose threshold is below the premium and recompute (book: 5,429 with 300 low-risk, 6,800 with 100).
3. Test a policy against the threshold (book: reinsurance at 6,000 gives 4,286, below 4,500).

Watch for: lowering average claims is not enough; the premium must fall below actual renewal thresholds.

## 3. Grossman health-capital model (grossman-health-capital-model)

When to use it: relating medical spending to the change in a health stock.

Equations as the chapter writes them:

    I=4\sqrt{M},
    H_{t+1}=0.8(80)+8=72.

Ask the user for: the health stock, depreciation rate, investment technology and medical input.

Steps:
1. Investment I = A sqrt(M) (book: 4 x 2 = 8).
2. H_next = (1 - delta) H + I (book: 0.8 x 80 + 8 = 72 at delta 0.20).
3. Maintenance M = (delta H / A)^2 (book: 4 at delta 0.10, 16 at 0.20, 4 again with A = 8).

Watch for: the chapter's inline text writes delta = 0.10 without the TeX backslash; the value is 0.10.

## 4. Ex-post moral hazard in health insurance (ex-post-moral-hazard-in-health-insurance)

When to use it: estimating extra care used because insurance lowers the patient's price.

Equations as the chapter writes them:

    B_q(q;s)=cp.
    q=6-0.02P_o,

Ask the user for: the demand schedule, resource cost per visit, coinsurance rate and marginal benefits.

Steps:
1. P_o = coinsurance x cost (book: 0.25 x 200 = 50).
2. Visits q = 6 - 0.02 P_o (book: 5).
3. Gap = cost of visits worth less than cost minus their benefit (book: 600 - 360 = 240).

Watch for: the gap is not the full welfare effect; insurance also protects against an uncertain bill.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as clinical facts.
