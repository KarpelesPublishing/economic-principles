---
name: ep-ch099-structuralist-feminist-and-ecological-alternatives
description: Apply the principles of Chapter 99 of The Encyclopedia of Economic Principals (Structuralist, Feminist, and Ecological Alternatives) to the user's own numbers. Use when checking a growth target against the balance of payments, writing a household time budget before counting extra paid hours as a gain, comparing material throughput with an ecological ceiling, or measuring what an export drive buys when the terms of trade fall.
---

# Chapter 99: Structuralist, Feminist, and Ecological Alternatives

These principles put hard constraints next to market outcomes: foreign exchange, time and material throughput. The chapter's numbers are hypothetical.

Notebook with the worked examples and figures: `../../notebooks/ch099-structuralist-feminist-and-ecological-alternatives.ipynb`

## 1. Center-periphery structuralism (center-periphery-structuralism)

When to use it: testing a growth target against export demand and import needs.

Expressions as the chapter writes them:

    \eta_x=0.7
    \eta_m=1.5
    2.1/1.5=1.4\%

Ask the user for: starting exports and imports, world growth, both income elasticities, the growth target.

Steps:
1. Export growth = eta_x x world growth (book: 0.7 x 3 = 2.1 percent, exports 102.1).
2. Import growth = eta_m x target (book: 1.5 x 5 = 7.5 percent, imports 107.5; gap 5.4).
3. Constrained growth = export growth / eta_m (book: 1.4 percent; with 1.2 and 0.8 the gap is 0.4).

Watch for: capital flows and relative prices can loosen the constraint for a while.

## 2. Social reproduction and unpaid care (social-reproduction-and-unpaid-care)

When to use it: checking where care hours come from when paid hours rise.

Equation as the chapter writes it:

    h_i+c_i+r_i=T_i.

Ask the user for: each adult's waking hours, paid hours, care hours, wages, the care need, and any purchased care and its charge.

Steps:
1. Rest = T - paid - care for each adult (book: Ana 112 - 25 - 35 = 52).
2. Extra paid hours without replacement care cut someone's rest (book: Ana to 37, or Ben to 42).
3. With purchased care, net cash = extra earnings - charge (book: 15 x 20 - 60 = 240; Ana's 20 and Ben's 15 care hours plus 15 purchased meet the need).

Watch for: the time budget does not value the quality of care.

## 3. Steady-state economy (steady-state-economy)

When to use it: comparing material throughput with a ceiling as durability changes.

Equation as the chapter writes it:

    \Delta K_p=I_p-dK_p.

Ask the user for: the stock, depreciation rate, material per unit built, extra building, the ceiling.

Steps:
1. Replacements = d K (book: 0.02 x 4,000 = 80).
2. Throughput = (replacements + extra) x intensity (book: 8,000 tonnes, 3,000 over 5,000; 4,000 at 1 percent).
3. Check the stock change (book: at 1 percent, 20 extra dwellings mean Delta K = 20, growth, and 6,000 tonnes).

Watch for: efficiency gains that fund extra building rebound into throughput.

## 4. Prebisch-Singer hypothesis (prebisch-singer-hypothesis)

When to use it: measuring the imports an export volume buys after a terms-of-trade change.

Calculations as the chapter writes them:

    0.8\times10{,}000=8{,}000
    0.8\times11{,}500=9{,}200

Ask the user for: export and import price indices, export volume.

Steps:
1. T = P_C / P_M (book: 0.8).
2. Import capacity = T x volume (book: 9,200 after raising exports by 15 percent, 800 fewer than 10,000).
3. Compare with the T = 1 path (book: 11,500 - 9,200 = 2,300).

Watch for: a temporary price swing is not the secular decline the hypothesis describes.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real economy.
