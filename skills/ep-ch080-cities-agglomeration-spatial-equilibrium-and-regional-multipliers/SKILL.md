---
name: ep-ch080-cities-agglomeration-spatial-equilibrium-and-regional-multipliers
description: Apply Chapter 80 of The Encyclopedia of Economic Principals (Cities, Agglomeration, Spatial Equilibrium, and Regional Multipliers) to the user's own numbers. Use when someone asks how an amenity or productivity gain splits between local wages and rents, whether a regional gap will shrink or compound, how many local jobs follow a new employer, or how large a public works multiplier is after taxes, imports and crowding out.
---

# Chapter 80: Cities, Agglomeration, Spatial Equilibrium, and Regional Multipliers

Trace a local shock into wages, rents, regional gaps and jobs, keeping gross and net effects apart.

Notebook with the worked examples and figures: `../../notebooks/ch080-cities-agglomeration-spatial-equilibrium-and-regional-multipliers.ipynb`

## 1. Rosen-Roback spatial equilibrium (rosen-roback-spatial-equilibrium)

When to use it: a place gains an amenity or productivity and mobile workers and firms re-sort.

    \Delta V=\Delta w-0.5\Delta r+10\Delta a,  \Delta\Pi=8\Delta A-\Delta w-0.25\Delta r.

Ask the user for: the household and firm coefficients and the size of each shock.

Steps:
1. Set both changes to zero and add them: 8 dA + 10 da = 0.75 dr.
2. Solve dr (book: amenity 13.333, productivity 10.667, thousand dollars).
3. dw = 8 dA - 0.25 dr (book: -3.333 and 5.333).

Watch for: the linearization holds only for small shocks with full mobility.

## 2. Circular cumulative causation (circular-cumulative-causation)

When to use it: a regional gap may persist or compound through feedback.

    g_1=0.40(\$10\text{ million})=\$4\text{ million},  g_2=0.40(\$4\text{ million})=\$1.6\text{ million}.

Ask the user for: the initial gap and each reinforcing and offsetting channel.

Steps:
1. Net reinforcement s = sum of reinforcing shares - offsets (book: 0.60 - 0.20 = 0.40).
2. g_t = s^t g0 (book: 4, then 1.6).
3. s above one means the gap grows (book: 1.10 gives 11 and 12.1); a policy that removes a channel lowers s (book: 0.60 gives 6 and 3.6).

Watch for: the values audit feedback; they are not estimated regional multipliers.

## 3. Local employment multiplier (local-employment-multiplier)

When to use it: a new tradable employer arrives and local service jobs follow.

    85(\$80{,}000)(0.30)=\$2.04\text{ million}.  \frac{0.75(\$2.04\text{ million})}{\$60{,}000}=25.5.

Ask the user for: resident workers, wage, local spending share, revenue per service job, share of demand met by more output, re-spending jobs.

Steps:
1. Local demand = residents x wage x local share (book: 2.04 million).
2. First round = quantity share x demand / revenue per job (book: 25.5).
3. m = (first round + re-spending) / direct jobs (book: (25.5 + 6)/100 = 0.315).

Watch for: housing limits and inelastic supply shrink the response (book: 12 jobs, m = 0.15).

## 4. Fiscal multiplier and public works (fiscal-multiplier-public-works)

When to use it: sizing the output effect of public spending with leakages.

    k_G=\frac{1}{1-0.60}=2.5.  k_G=\frac{1}{1-0.60(1-0.20)+0.15}=\frac{1}{0.67}\approx1.493.

Ask the user for: the spending, propensity to consume, tax rate, import share, crowded-out private output and the project's service value.

Steps:
1. k = 1 / (1 - c(1 - t) + m) (book: 1.493).
2. Output gain = k x spending (book: 14.93 million); subtract crowding out (book: 11.93, measured 1.193).
3. Value the project separately (book: 12 - 10 = 2 million).

Watch for: the multiplier assumes idle resources.

## How to answer

- Write each formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you supplied.
- The chapter's numbers are hypothetical teaching values; never present them as facts about a real region.
