---
name: ep-ch003-production-duality-factor-demand-and-firm-optimization
description: Apply Chapter 3 of The Encyclopedia of Economic Principals (Production Duality, Factor Demand, and Firm Optimization) to the user's own numbers. Use when someone sets output where marginal revenue meets marginal cost, values extra capacity, reads input demand off a cost function, decides whether a loss-making plant should keep running, or finds the least-cost mix of labor and capital.
---

# Chapter 3: Production Duality, Factor Demand, and Firm Optimization

Choose output at the margin and inputs at least cost.

Notebook with the worked examples and figures: `../../notebooks/ch003-production-duality-factor-demand-and-firm-optimization.ipynb`

## 1. Profit-maximization condition (profit-maximization-condition)

    MR(q) = MC(q)  (book: 120 - 4q = 20 + 2q, q* = 50/3 = 16.67)

Steps: solve for q; check capacity (book cap 12 binds); compute price, revenue, cost, profit (book: 86.67, 1,444.44, 811.11, 633.33; at cap 12: 96 and 568). At a binding cap, MR - MC (book: 72 - 44 = 28) is the most one more unit of capacity is worth.

## 2. Shephard's lemma (shephards-lemma)

    c(w, r, y) = 2y sqrt(wr);  dc/dw = y sqrt(r/w) = L

Steps: labor and capital demand (book: 50 and 200 at w = 16, r = 4, y = 100); cost (1,600). For a finite wage change, the tangent (fixed labor) overstates the cost increase (book: 450 versus 400).

## 3. Shutdown rule (shutdown-rule)

    AVC(q) = 80/q + 10 + q;  MC(q) = 10 + 2q

Steps: output from price = MC; contribution = revenue - avoidable cost; operate if positive (book: at 30, 300 - 280 = 20, operate; at 26, -16, close). Costs owed either way cancel (book: if the 80 is owed anyway, contribution at 26 is 64).

## 4. Cost minimization and constrained optimization (cost-minimization-constrained-optimization)

    f_L / f_K = K/(2L) = w/r  for y = L^(1/3) K^(2/3)

Steps: K = 2(w/r) L; substitute into the output target (book: K = 8L, 100 = 4L, L = 25, K = 200, cost 1,500). At w = 45: L = 14.5597, K = 262.07, cost 1,965.56. A binding labor minimum puts the firm at a corner (book example: 40 workers).

## How to answer

- Write each formula, then the user's numbers, then the result.
- Separate avoidable from unavoidable costs before any shutdown verdict.
- Private cost is not social cost; say so when the user asks a policy question.
