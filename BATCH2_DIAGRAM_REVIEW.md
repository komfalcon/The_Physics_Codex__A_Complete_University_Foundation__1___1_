# Batch 2 Diagram Review — Items 11–20

## Scope

This batch covers the closed-polygon equilibrium diagram, the remaining Chapter 2 vector diagrams through the cross-product rule, and the displacement-time and velocity-time graphs in Chapter 3.

## Results

| # | Diagram | Result | Action |
|---:|---|---|---|
| 11 | Closed Polygon: Equilibrium | PASS | The four arrows close head-to-tail and the zero-resultant statement is scientifically correct. |
| 12 | Calculating the Resultant Analytically | PASS | The 80 N, 60 N, 100 N right-triangle construction and 36.9° direction are consistent and readable. |
| 13 | Resolution of a Vector | PASS | The original vector, perpendicular components, angle, axes, and formulas agree. |
| 14 | Position Vectors in 2D | PASS | Both position vectors originate at O, point coordinates agree with the drawn locations, and AB is correctly directed from A to B. |
| 15 | Equilibrium of Forces | NEEDS FIX — corrected | The left cable was drawn at approximately 51° from the vertical while labeled 30°. Its endpoint is now calculated as $x=-2\tan 30°=-1.155$ for a 2-unit vertical rise. |
| 16 | Geometric Meaning of the Dot Product | PASS | The projection of A onto B, angle, and dot-product identity are scientifically correct and legible. |
| 17 | Right-Hand Rule | NEEDS FIX — corrected | The original “out of page” result included an in-page upward arrow and a zero-length arrow. It now uses the standard circled-dot symbol with an explicit out-of-page label. |
| 18 | The Vector (Cross) Product / cyclic rule | NEEDS FIX — corrected | The drawn cycle is the positive cyclic order $\hat{i}\to\hat{j}\to\hat{k}\to\hat{i}$, but the caption called it negative. The caption now says “Clockwise cycle: positive product.” |
| 19 | Displacement-Time Graphs | PASS | Axes, units, constant-velocity line, accelerating curve, and rest line are correct and readable. |
| 20 | Velocity-Time Graph | PASS | The three phases, slopes, units, shaded displacement areas, and worked values are consistent. |

## Validation

- Clean LaTeX compilation produced **513 pages**.
- Rendered and inspected the affected diagrams at 120 dpi, including PDF pages 52–64 and 76–77.
- The corrected equilibrium diagram now visually matches the 30° and 45° labels.
- The corrected cross-product diagram uses an unambiguous out-of-page convention.
- The velocity-time graph’s shaded areas visibly match the displacement calculations.

## Build note

The repository still emits pre-existing unresolved references for `tab:si_base`, `tab:prefixes`, `tab:instruments`, `sec:unit_vectors`, `sec:position_vectors`, `sec:component_method`, `tab:densities`, `tab:viscosity`, and `tab:expansion`. These are unrelated to the Batch 2 diagram edits and were not introduced by them; they should be handled in a separate reference-integrity pass.
