---
name: ep-ch019-attention-information-avoidance-and-bounded-rationality
description: Apply the principles of Chapter 19 of The Encyclopedia of Economic Principals (Attention, Information Avoidance, and Bounded Rationality) to the user's own numbers. Use when a committee weighs a vivid demo against verified evidence, when a search stops at the first good-enough option, when someone declines a useful signal, or when a ranking or badge concentrates attention.
---

# Chapter 19: Attention, Information Avoidance, and Bounded Rationality

These principles price scarce attention: what weight evidence gets, when search should stop, when a signal goes unread and when a badge is credible rather than merely visible.

Notebook with the worked examples and figures: `../../notebooks/ch019-attention-information-avoidance-and-bounded-rationality.ipynb`

## 1. Attention economics and the demo effect (attention-economics-demo-effect)

When to use it: a reviewer ranks options on verified breadth and presentation salience.

Equation as the chapter writes it:

    Q_j=wE_j+(1-w)S_j,  Q_A=0.6(55)+0.4(95)=71

Ask the user for: each option's breadth and salience scores (same scale) and the weight w on breadth.

Steps:
1. Score each option (book: 0.6 x 55 + 0.4 x 95 = 33 + 38 = 71; 0.6 x 68 + 0.4 x 55 = 62.8).
2. Compute the tie weight, (S_A - S_B) / ((S_A - S_B) + (E_B - E_A)) (book: 40/53 = 0.755).
3. State the winner and how far w must move to flip it (book: at w = 0.9, 59 against 66.7).

Watch for: salience can proxy for genuine usability, so a high weight on it is not automatically an error.

## 2. Bounded rationality and satisficing (bounded-rationality-and-satisficing)

When to use it: options are inspected one at a time and the first one clearing a bar is taken.

Equation as the chapter writes it:

    \tau=\min\{t:v(x_t)\geq A\},  (91-77)(\$100)=\$1{,}400

Ask the user for: values in inspection order, the aspiration A, the cost per inspection and the value of one point.

Steps:
1. Find tau, the first value at or above A (book: Omar 77 at tau = 2).
2. Cost of the remaining inspections (book: 2 x 300 = 600).
3. Gain from seeing them, best minus chosen times value per point (book: 14 x 100 = 1,400); net 1,400 - 600 = 800.
4. State whether exhaustive search pays and at what cost it stops paying (book: at 900 per interview, 1,800 exceeds 1,400).

Watch for: the gain uses hindsight; a real searcher does not know the unseen values.

## 3. Information avoidance (information-avoidance)

When to use it: someone declines a free, accurate and actionable signal.

Equation as the chapter writes it:

    0.5(\$120)=\$60,  \$60-\$80=-\$20

Ask the user for: the probability the signal calls for action, the value of acting and the cost of knowing (anxiety, obligation).

Steps:
1. Instrumental value = probability x value of acting (book: 0.5 x 120 = 60).
2. Net = instrumental value - cost of knowing (book: 60 - 80 = -20, so she avoids it).
3. Break-even probability = cost / value (book: 80 / 120 = 0.667). A net of exactly zero is indifference.

Watch for: distrust, privacy, reading cost or inability to act can rationally reduce demand for information.

## 4. Signaling and winner-take-attention markets (signaling-winner-take-attention)

When to use it: a ranking or badge directs attention, and you want to know if it also signals quality.

Equation as the chapter writes it:

    \alpha_A=\frac{5}{6.5}\approx0.7692,  \$5-\$2=\$3>0,  \$5-\$8=-\$3<0

Ask the user for: rank weights, the audience size, the badge benefit and each type's cost of earning it.

Steps:
1. Shares = weight / total weight (book: 5 / 6.5 = 0.7692, about 769 of 1,000 inquiries).
2. Net benefit by type (book: 5 - 2 = 3 for the high type, 5 - 8 = -3 for the weak type).
3. Separating if only the high type gains; a weak-type net of exactly zero is indifference (not strict separation); pooling if both gain (book: weak cost 3).

Watch for: visibility is not credibility, and concentrated attention can reflect real quality or scale.

## How to answer

- Show every substitution: write the formula, then the user's numbers in it, then the result.
- Say which inputs are the user's and which are assumptions you added.
- Name ties and undefined cases instead of forcing a winner.
- Do not present the book's hypothetical numbers as facts about any real market.
