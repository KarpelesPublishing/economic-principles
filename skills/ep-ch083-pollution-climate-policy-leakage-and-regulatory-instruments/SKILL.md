---
name: ep-ch083-pollution-climate-policy-leakage-and-regulatory-instruments
description: Apply Chapter 83 of The Encyclopedia of Economic Principals (Pollution, Climate Policy, Leakage, and Regulatory Instruments) to the user's own numbers. Use when someone asks whether environmental rules will push a plant abroad, whether growth will lower emissions, whether an announced future carbon charge will speed up extraction, or whether to regulate pollution with a tax or a cap.
---

# Chapter 83: Pollution, Climate Policy, Leakage, and Regulatory Instruments

Compare locations by delivered cost, split emissions into scale, composition and technique, watch the timing of announced policy, and choose between prices and quantities.

Notebook with the worked examples and figures: `../../notebooks/ch083-pollution-climate-policy-leakage-and-regulatory-instruments.ipynb`

## 1. Pollution-haven hypothesis (pollution-haven-hypothesis)

When to use it: judging whether a regulatory gap will move production.

    K_S=14.7+0.3+0.5=15.5\text{ million dollars}

Ask the user for: ordinary, environmental and delivery cost at each site.

Steps:
1. Total each site (book: North 14.0 + 1.8 = 15.8; South 14.7 + 0.3 + 0.5 = 15.5).
2. The cheaper site wins (book: South by 0.3; before the agreement South cost 16.2 and lost).
3. Test equal enforcement (book: South 17.0, no move).

Watch for: a move needs both a regulatory gap and low trade costs.

## 2. Environmental Kuznets curve (environmental-kuznets-curve)

When to use it: asking whether emissions fall as income rises.

    E_L=80[0.45(2.5)+0.55(0.4)]=107.6

Ask the user for: output, dirty-sector share and the two sectors' emission intensities at each stage.

Steps:
1. E = output x (share x dirty intensity + (1 - share) x clean intensity) at each stage (book: 107.6, 217.7, 71.5).
2. Recompute with the original intensities to isolate technique (book: 203.5).
3. Report how much of any fall comes from composition and technique, not income.

Watch for: territorial emissions can fall because dirty industry moved abroad.

## 3. Green paradox (green-paradox)

When to use it: a producer charge announced for a later date.

    p_t=100-q_t;  q_0+q_1=100;  100-q_0=q_0-20

Ask the user for: the stock, the demand curve each period, and the charge in each period.

Steps:
1. Set net prices equal across periods (book: 100 - q0 = q0 - 20).
2. Solve for q0 and q1 (book: 60 and 40, against 50 and 50 without policy).
3. Equal charges in both periods cancel (book: back to 50 and 50).

Watch for: the result assumes a credible announcement and a stock that is all sold.

## 4. Weitzman prices versus quantities (weitzman-prices-versus-quantities-result)

When to use it: choosing a tax or a cap under uncertain abatement cost.

    L_Q(\varepsilon)=\frac{\varepsilon^2}{2(b+c)};  L_P(\varepsilon)=\frac{\varepsilon^2b^2}{2c^2(b+c)}

Ask the user for: the slope of marginal benefit b, the slope of marginal cost c, and the size of the cost shock.

Steps:
1. L_Q = shock^2 / (2(b + c)) (book: 144 / 16 = 9).
2. L_P = shock^2 b^2 / (2 c^2 (b + c)) (book: 576 / 576 = 1).
3. The smaller loss wins: b < c favors the tax, b > c the cap, equal slopes tie (book b = 12, c = 3: 76.8 against 4.8, cap).

Watch for: the result is local, for linear curves near the target.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied.
- Report ties as ties.
- The chapter's numbers are hypothetical teaching values; never present them as facts about a real pollutant or country.
