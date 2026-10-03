---
name: ep-ch079-state-capacity-extractive-institutions-and-development
description: Apply Chapter 79 of The Encyclopedia of Economic Principals (State Capacity, Extractive Institutions, and Development) to the user's own numbers. Use when someone asks whether a ruler with a given tenure will restrain extraction, how a revenue windfall is absorbed by competing claims, why an elite rejects a growth-raising project, or whether an officeholder will pay for tax-collection capacity.
---

# Chapter 79: State Capacity, Extractive Institutions, and Development

Compare the decision maker's private, horizon-weighted payoff with the social value of restraint and investment.

Notebook with the worked examples and figures: `../../notebooks/ch079-state-capacity-extractive-institutions-and-development.ipynb`

## 1. Olson stationary-bandit model (olson-stationary-bandit-model)

When to use it: a ruler chooses between heavy extraction now and a protected tax base.

    45+0.765(15)=56.475.  38.5+0.765(38.5)=67.9525.  45.5-8+0.765(45.5)=72.3075.

Ask the user for: revenue now and later under each policy, any upfront cost, survival probability s and discount factor delta.

Steps:
1. Continuation weight = s x delta (book: 0.85 x 0.90 = 0.765).
2. Value = first-year revenue - cost + weight x later revenue for each policy.
3. Pick the highest (book: patrol 72.3075; at s = 0.20 heavy 47.7 beats patrol 45.69).

Watch for: the ruler's best policy is not necessarily socially optimal.

## 2. Voracity effect (voracity-effect)

When to use it: a windfall arrives where groups cannot commit to restraint.

    \frac{\Delta T}{\Delta W}=\frac{\$48}{\$30}=1.6.  \$180-\$60-\$93=\$27,  \$180-\$60-(\$45+\$18)=\$57.

Ask the user for: normal resources, committed spending, existing transfers, the windfall, the number of groups and each group's extra claim.

Steps:
1. New claims = groups x extra demand (book: 4 x 12 = 48); multiplier = claims / windfall (book: 1.6).
2. Investment = resources + windfall - services - transfers (book: 27, down from 45).
3. With a binding cap on new transfers recompute (book: 57).

Watch for: a cap that is evaded through guarantees or exemptions does not bind.

## 3. Extractive institutions (extractive-institutions)

When to use it: an elite sets an extraction rate and decides on a public input it must pay for.

    y(\tau)=160(1-\tau),  R(\tau)=160\tau(1-\tau).  \frac{dR}{d\tau}=160(1-2\tau)=0,  33.75-30-8=-4.25,

Ask the user for: potential output, the extraction rate, the input's cost and its effect on potential output.

Steps:
1. Output e0(1 - tau), elite revenue tau x output (book: tau 0.5 gives 80 and 40).
2. For a project: elite change = new revenue - old revenue - cost (book: 33.75 - 30 - 8 = -4.25).
3. Compare with the social change (book: 127 vs 120, +7): a positive social gain can still be rejected.

Watch for: changes in who holds power can add to or reverse the ledger.

## 4. Fiscal capacity and state building (fiscal-capacity-state-building)

When to use it: deciding whether to invest in tax administration.

    T_0=0.45(0.18)(\$2{,}000)=\$162.  T_1=0.70(0.18)(\$2{,}000)=\$252,  \$90(1+0.92+0.92^2)=\$248.976.  0.40(\$90)=\$36,

Ask the user for: base, statutory rate, collection capacity before and after, project cost, discount factor, horizon and the officeholder's retention probability.

Steps:
1. Revenue T = q x rate x base before and after (book: 162 and 252, gain 90).
2. Present value of the gain over the horizon (book: 248.976; net of cost 198.976).
3. Officeholder benefit = retention probability x one year's gain (book: 36 < 50, rejects; break-even p = 50/90 = 0.556).

Watch for: compliance, privacy and error costs are omitted and must be added.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied.
- Report ties as ties.
- The chapter's numbers are hypothetical teaching values; never present them as historical facts.
