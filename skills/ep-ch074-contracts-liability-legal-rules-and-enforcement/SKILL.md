---
name: ep-ch074-contracts-liability-legal-rules-and-enforcement
description: Apply Chapter 74 of The Encyclopedia of Economic Principals (Contracts, Liability, Legal Rules, and Enforcement) to the user's own numbers. Use when someone compares strict liability with negligence for a risky activity, asks whether a seller should perform or breach given damages, weighs more inspection against higher fines, or reads a price change in a prohibited market.
---

# Chapter 74: Contracts, Liability, Legal Rules, and Enforcement

Treat legal rules as prices on care, activity, breach and offending, and compute the choices they induce.

Notebook with the worked examples and figures: `../../notebooks/ch074-contracts-liability-legal-rules-and-enforcement.ipynb`

## 1. Strict-liability versus negligence result (strict-liability-versus-negligence-result)

When to use it: comparing liability rules when both care and activity level matter.

    B(z) = 24z - z^2/2;  24 - z - 8 = 0 (strict liability);  24 - z - 5 = 0 (negligence)

Steps:
1. Social cost per unit of each care level (book: 2 + 9 = 11, 5 + 3 = 8; due care is efficient).
2. Strict liability: the firm bears the full 8, so z = 16.
3. Negligence: a compliant firm bears only 5, so z = 19, three units too many.

Watch for: if regulation fixes activity, both rules give the same result.

## 2. Expectation-damages efficient-performance result (expectation-damages-efficient-performance-result)

When to use it: deciding whether a seller performs or breaches given the damages it would pay.

    D = V - P;  perform payoff P - C;  breach payoff -D

Steps:
1. Damages (book: 125 - 80 = 45).
2. Compare payoffs (book C = 100: 80 - 100 = -20 beats -45, so perform; surplus 125 - 100 = 25).
3. Check against efficiency, V against C (book C = 150: breach saves 25).
4. Mismeasured damages distort the choice (book: 15 at C = 100 invites breach; 80 at C = 150 forces performance).

Watch for: assumes damages are fully paid and no transaction cost.

## 3. Becker deterrence model of crime (becker-deterrence-model-of-crime)

When to use it: comparing more detection with heavier penalties.

    net payoff = gain - moral cost - p x (collected share x penalty)

Steps:
1. Expected sanction (book: 0.08 x 150 = 12).
2. Net payoff (book: 40 - 6 - (0.08)(150) = 22; at p = 0.25, -3.5).
3. Collection matters (book: 0.40 x 470 = 188 and 40 - 6 - (0.08)(188) = 18.96).
4. Population share deterred (book: 1,000 riders uniform on 0 to 60; sanction 12 leaves 800, sanction 36 leaves 400).

Watch for: citations can rise when inspection expands even as offending falls.

## 4. Prohibition risk premium (prohibition-risk-premium)

When to use it: explaining the price of a banned good.

    p = (production + concealment + expected punishment) / (1 - seizure probability)

Steps:
1. Low enforcement (book: (45 + 7 + 8) / 0.80 = 75; Q = 1,800 - 10(75) = 1,050).
2. High enforcement (book: (45 + 25 + 14) / 0.70 = 120; Q = 600).
3. Check other causes (book: cost 81 with low enforcement also gives 120).

Watch for: a price alone cannot identify the enforcement channel.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
