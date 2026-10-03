---
name: ep-ch049-liquidity-fire-sales-and-financial-fragility
description: Apply Chapter 49 of The Encyclopedia of Economic Principals (Liquidity, Fire Sales, and Financial Fragility) to the user's own numbers. Use when someone asks whether asset sales can cure a covenant or margin call, how a margin increase forces deleveraging, what a bank saves by monitoring for its depositors, how much loan value a run destroys, or how a forced sale shrinks lending capacity.
---

# Chapter 49: Liquidity, Fire Sales, and Financial Fragility

When selling to raise cash lowers the value of what is left.

Notebook with the worked examples and figures: `../../notebooks/ch049-liquidity-fire-sales-and-financial-fragility.ipynb`

## 1. Fire-sale externality (fire-sale-externality)

    p = min(buyer cash / units offered, use value)  (book: 8,000 / 100 = 80)
    debt - p x = ratio p (units - x)  (book: 7,500 - 80x = 0.80(80)(100 - x), x = 68.75)

Steps: mark at the first price; compare debt with ratio x price x units (book: 6,400, breach 1,100); solve for x and round up (69); reprice with every seller included (8,000 / 169 = 47.34); recompute debt and capacity (4,233.73 against 1,173.96, shortfall 3,059.76).

## 2. Market-liquidity and funding-liquidity spiral (market-liquidity-and-funding-liquidity-spiral)

    max position = equity / margin;  sale = mark - equity / margin

Steps: equity = mark - debt (book: 9.5 - 9 = 0.5); financeable position at the new margin (0.5 / 0.20 = 2.5); sale (7); repeat at the old margin (4.5) to isolate the margin effect (2.5).

## 3. Financial intermediation and banking (financial-intermediation)

    direct = savers x loans x review cost;  delegated = loans x specialist cost + G
    face sold = (withdrawals - reserves) / price

Steps: compare costs (book: 100,000 against 10,000; delegation loses its edge if G > 92,000); cash gap (60,000 - 20,000 = 40,000); face sold (40,000 / 0.75 = 53,333.33).

## 4. Liquidity crisis and credit crunch (liquidity-crisis-credit-crunch)

    face sold = gap / price;  equity = loans left - claims left;  lending capacity = equity / capital ratio

Steps: gap (book: 60 - 20 = 40); face sold (44.44) and loss (4.44); equity (55.56 - 50 = 5.56); capacity (55.56; the book prints 55.6). With a central bank facility no loans are sold and equity stays 100 - 50 - 40 = 10.

## How to answer

- Write each formula, then the user's numbers, then the result.
- Reprice after counting every seller who reaches the same buyers.
- Separate a liquidity shortfall from insolvency: a facility fixes the first, not the second.
