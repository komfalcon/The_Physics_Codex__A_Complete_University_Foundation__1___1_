# Batch 4 Diagram Review — Items 31–40

## Scope

This batch covers the remaining simple-harmonic-motion figures, gravitation figures, elasticity figures, and the lever-class figure listed as inventory items 31–40.

## Review standard

Each item was checked against its surrounding prose and equations for scientific accuracy, force/curve geometry, label correctness, learner clarity, print-size readability, and TikZ/PGFPlots containment. The final PDF pages were rendered at 120 dpi and inspected after the source changes.

## Results

| # | Source / lines | Diagram | Scientific verdict | Action | Visual/readability result | PDF page | Unresolved uncertainty |
|---:|---|---|---|---|---|---:|---|
| 31 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:299–338` | The Simple Pendulum | NEEDS FIX — corrected | The length marker was drawn vertically rather than parallel to the displaced string; the tension arrow was not directed exactly toward the pivot; and the dashed restoring-force arrow was horizontal rather than tangential to the path. The marker is now parallel to the string, tension terminates at the pivot, and the restoring component follows the tangent toward equilibrium. | Final render shows the bob, string, length, angle, $T$, $mg$, and tangential $mg\sin\theta$ without clipping or collision. | 124 | None identified. |
| 32 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:495–528` | Energy vs Displacement in SHM | NEEDS FIX — corrected | The PE curve originally extended to $|x|=1.1A$, outside the physical oscillation range and above the total-energy line. Its domain is now $-A\le x\le A$, matching the KE curve and the $-A$, $0$, $A$ ticks. | Final graph meets the total-energy line at both amplitudes and remains clear and contained. | 126 | None identified. |
| 33 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:597–629` | Damping Comparison | NEEDS FIX — corrected | The original heavy-damping curve was a single exponential with nonzero initial slope, making it appear faster than critical damping at early times and not representing the same zero-initial-velocity displacement condition. It is now an overdamped-style $(1+0.5t)e^{-0.5t}$ curve, which stays non-oscillatory and decays more slowly than the critical curve. | Final plot preserves clear light/heavy/critical ordering and readable legend, axes, and equilibrium line. | 128 | None identified. |
| 34 | `chapters/part1_mechanics/ch08_gravitation.tex:86–113` | Gravitational Force Between Two Masses | PASS | No source change. The equal-magnitude force arrows point inward along the line joining the masses, and the center-to-center distance marker is correct. | Arrows, mass labels, distance $r$, and Newton’s Third Law annotation are legible and contained. | 135 | None identified. |
| 35 | `chapters/part1_mechanics/ch08_gravitation.tex:270–304` | $g$ vs Distance from Earth’s Centre | PASS | No source change. The uniform-density interior model is linear from $g=0$ at the centre to $g_s$ at the surface; the exterior curve follows the inverse-square law and joins continuously at $R_E$. The assumption is explicitly stated. | Surface marker, inside/outside labels, axes, and units are readable without clipping. | 138 | None identified. |
| 36 | `chapters/part1_mechanics/ch09_elasticity.tex:118–159` | Force-Extension Graph (Hooke’s Law Region) | PASS | No source change. The initial line has gradient $k=500\ \text{N\,m}^{-1}$ and reaches $(e,F)=(0.08\ \text{m},40\ \text{N})$ at the marked elastic limit; the post-limit curve is clearly identified as illustrative. | Axes, ticks, gradient construction, elastic-limit marker, and region labels are readable and contained. | 148 | None identified. |
| 37 | `chapters/part1_mechanics/ch09_elasticity.tex:272–322` | Series vs Parallel Springs | PASS | No source change. Series springs share force and add extensions, giving $1/k_s=1/k_1+1/k_2$; parallel springs share extension and add stiffness, giving $k_p=k_1+k_2$. The connection geometry matches both arrangements. | The two spring arrangements, masses, labels, and formulas are visually distinct and fit within the diagram box. | 150 | None identified. |
| 38 | `chapters/part1_mechanics/ch09_elasticity.tex:448–558` | Stress-Strain Graph for a Ductile Metal (Steel) | NEEDS FIX — corrected | The original elastic/yield zone labels and origin/Hooke annotations crowded the high-gradient region at print size. Zone labels were separated, the origin marker moved above the axis, and the Hooke’s-law annotation was repositioned. | Final plot cleanly shows O, A, B, C, D, the four regions, the reference yield line, and the explanatory table without clipping. | 152 | None identified. |
| 39 | `chapters/part1_mechanics/ch09_elasticity.tex:603–639` | Comparing Stress-Strain Curves | PASS | No source change. The normalized ductile, brittle, and rubber-like curves have the intended qualitative behavior: plastic deformation and hardening, sudden brittle fracture, and a J-shaped elastic curve. | Legend and three curves are legible; normalized axes are intentionally unlabeled in scale and do not imply common material units. | 153 | None identified. |
| 40 | `chapters/part1_mechanics/ch10_simple_machines.tex:213–276` | The Three Classes of Lever | NEEDS FIX — corrected | The original long class captions collided with effort arrows and adjacent moment-arm labels. The captions were replaced by compact 1st/2nd/3rd markers beside each beam; the summary table directly below retains the full class arrangements and examples. | Final render clearly separates the three lever geometries, effort/load arrows, fulcra, moment arms, and class markers. | 162 | None identified. |

## Validation

- Clean LaTeX compilation succeeded with `latexmk -pdf -interaction=nonstopmode -file-line-error -halt-on-error book_main.tex`.
- Output remains **513 PDF pages**, A4.
- Final renders inspected at 120 dpi included PDF pages 124, 126, 128, 135, 138, 148, 150, 152, 153, and 162, with adjacent-page checks where relevant.
- The repaired pendulum, SHM energy, damping, stress-strain, and lever figures were visually rechecked after compilation.
- No fatal errors or new source-specific warnings were introduced by the Batch 4 changes.

## Build note

The repository retains its pre-existing unresolved references (`tab:si_base`, `tab:prefixes`, `tab:instruments`, `sec:unit_vectors`, `sec:position_vectors`, `sec:component_method`, `tab:densities`, `tab:viscosity`, and `tab:expansion`) and **516** pre-existing overfull-box diagnostics. These are unrelated to the Batch 4 diagram changes and were not repaired in this batch.

## Progress

Items **31–40** are now individually reviewed, for **40 of 86** inventory diagrams reviewed. Items **41–86** remain unreviewed and are not certified by this report.
