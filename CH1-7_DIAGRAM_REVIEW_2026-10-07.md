The baseline audit visually checked all **31 instructional drawings in Chapters 1–7** and the **two requested front-matter TikZ graphics** against the untouched 508-page PDF built from commit `10ea81c`. In the final integrated candidate PDF at `/tmp/physics-codex-diagram-reaudit-final-r5/book_main.pdf` (508 A4 pages; SHA-256 `b8cef6c11222ec6a74e1ced0bc289473d0f7e4a18f15543f129b23b4c5bb2b92`), all **20 source-edited instructional figures** have a post-edit visual check. The r4 integrated sweep exposed five residual layout collisions; after their corrections, pages 53, 76, 95, 98, and 124 were rechecked in r5. The later three corrections on pp.87, 90, and 111 were also checked in r5 at 220 dpi. All eight latest pages pass with no locator shifts; the other edited figures retain their earlier integrated post-edit checks. Table locations are physical PDF page / printed page; front matter is unnumbered. The table records baseline dispositions and edit history; the integrated r5 result is summarized below.

## Figure-by-figure checklist

| # | Figure | Source | Baseline PDF page (physical / printed) | Baseline disposition / source-edit history |
|---:|---|---|---:|---|
| 1 | Title-page atom-like emblem | `front_matter/titlepage.tex:25` | 2 / unnumbered | Inspected; unchanged; see cover recommendation below |
| 2 | Dedication-page frame | `front_matter/dedication.tex:11` | 4 / unnumbered | Inspected; unchanged; decorative |
| 3 | Reading a Vernier Calliper | `chapters/part1_mechanics/ch01_measurement.tex:835` | 36 / 15 | Edited; post-edit figure checked in integrated r4 |
| 4 | Equal Vectors | `chapters/part1_mechanics/ch02_scalars_vectors.tex:124` | 41 / 20 | Inspected; no source edit |
| 5 | Parallel and Anti-parallel Vectors | `chapters/part1_mechanics/ch02_scalars_vectors.tex:188` | 42 / 21 | Inspected; no source edit |
| 6 | Magnitude from Pythagoras | `chapters/part1_mechanics/ch02_scalars_vectors.tex:343` | 45 / 24 | Edited; post-edit figure checked in integrated r4 |
| 7 | Vector Representation | `chapters/part1_mechanics/ch02_scalars_vectors.tex:446` | 46 / 25 | Inspected; no source edit |
| 8 | Triangle Rule | `chapters/part1_mechanics/ch02_scalars_vectors.tex:493` | 46 / 25 | Edited; post-edit figure checked in integrated r4 |
| 9 | Parallelogram Rule | `chapters/part1_mechanics/ch02_scalars_vectors.tex:536` | 47 / 26 | Inspected; no source edit |
| 10 | Polygon Rule: Four Vectors | `chapters/part1_mechanics/ch02_scalars_vectors.tex:590` | 48 / 27 | Edited; post-edit figure checked in integrated r4 |
| 11 | Closed Polygon: Equilibrium | `chapters/part1_mechanics/ch02_scalars_vectors.tex:623` | 48 / 27 | Inspected; no source edit |
| 12 | Worked perpendicular-force resultant | `chapters/part1_mechanics/ch02_scalars_vectors.tex:714` | 49 / 28 | Inspected; no source edit |
| 13 | Resolution of a Vector | `chapters/part1_mechanics/ch02_scalars_vectors.tex:792` | 50 / 29 | Inspected; no source edit |
| 14 | Position Vectors in 2D | `chapters/part1_mechanics/ch02_scalars_vectors.tex:1041` | 53 / 32 | Edited; the final integrated r5 check confirms $\vect{AB}$ is clear of the dashed arrow |
| 15 | Two-cable traffic-light equilibrium | `chapters/part1_mechanics/ch02_scalars_vectors.tex:1256` | 56 / 35 | Edited; post-edit figure checked in integrated r4 |
| 16 | Geometric Meaning of the Dot Product | `chapters/part1_mechanics/ch02_scalars_vectors.tex:1348` | 57 / 36 | Edited; post-edit figure checked in integrated r4 |
| 17 | Right-Hand Rule | `chapters/part1_mechanics/ch02_scalars_vectors.tex:1599` | 60 / 39 | Inspected; no source edit |
| 18 | Cyclic Rule for Unit Vectors | `chapters/part1_mechanics/ch02_scalars_vectors.tex:1643` | 60 / 39 | Inspected; baseline arrows and “clockwise” caption agree; unchanged |
| 19 | Displacement-Time Graphs | `chapters/part1_mechanics/ch03_kinematics.tex:303` | 72 / 51 | Edited; post-edit figure checked in integrated r4 |
| 20 | Velocity-Time Graph | `chapters/part1_mechanics/ch03_kinematics.tex:358` | 73 / 52 | Edited; post-edit figure checked in integrated r4 |
| 21 | Projectile Motion Trajectory | `chapters/part1_mechanics/ch03_kinematics.tex:594` | 76 / 55 | Edited; final integrated r5 check confirms range annotation clear of x-axis title and sample-position key |
| 22 | Atwood-machine forces (Example 4.4) | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex:366` | 87 / 66 | Edited; final integrated r5 check confirms stems clear of 4 kg and 6 kg labels |
| 23 | Forces on an Inclined Plane | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex:437` | 88 / 67 | Edited; post-edit figure checked in integrated r4 |
| 24 | Velocity-Time Graph for Terminal Velocity | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex:604` | 90 / 69 | Edited; final integrated r5 check confirms “$a$ decreasing” is clear of the curve |
| 25 | Work Done at an Angle | `chapters/part1_mechanics/ch05_work_energy_power.tex:65` | 95 / 74 | Edited; final integrated r5 check confirms $\theta$ and $F\cos\theta$ are separated |
| 26 | Work Done in Stretching a Spring | `chapters/part1_mechanics/ch05_work_energy_power.tex:329` | 98 / 77 | Edited; final integrated r5 check confirms the equation clears the data line and legend |
| 27 | Angular and Linear Quantities | `chapters/part1_mechanics/ch06_circular_motion.tex:121` | 108 / 87 | Inspected; no source edit |
| 28 | Conical Pendulum | `chapters/part1_mechanics/ch06_circular_motion.tex:248` | 109 / 88 | Edited; post-edit figure checked in integrated r4 |
| 29 | Vertical Circle — Forces at Key Points | `chapters/part1_mechanics/ch06_circular_motion.tex:408` | 111 / 90 | Edited; final integrated r5 check confirms “Bottom” is clear of the downward $mg$ stem |
| 30 | SHM Graphs — Displacement, Velocity, Acceleration | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:144` | 118 / 97 | Edited; post-edit figure checked in integrated r4 |
| 31 | The Simple Pendulum | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:301` | 120 / 99 | Inspected; no source edit |
| 32 | Energy vs Displacement in SHM | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:497` | 122 / 101 | Edited; post-edit figure checked in integrated r4 |
| 33 | Damping Comparison | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:599` | 124 / 103 | Edited; final integrated r5 check confirms the legend is clear of all three curves |

The corrected Chapter 2 mapping includes the **Four-Vector Polygon at physical p. 48 / printed p. 27**. Other corrected physical-page locations are **Position Vectors p. 53** (not p. 52), **traffic-light equilibrium p. 56** (not p. 55), the worked resultant sketch **p. 49** (not p. 48), and **both** cross-product drawings on **p. 60**.

## Earlier nine source edits retained

1. **Vernier calliper — Chapter 1, p. 36:** changed the inset range to `3.0–4.24 cm`, matching the last plotted vernier mark; the reading remains `3.34 cm`.
2. **Velocity–time graph — Chapter 3, p. 73:** replaced the single gradient arrow with a rise/run triangle and explicit `Δt` and `Δv` labels.
3. **Projectile trajectory — Chapter 3, p. 76:** allowed the below-axis range annotation to render and identified the plotted red dots as sampled positions, not velocity vectors, with a matching legend key.
4. **Inclined-plane forces — Chapter 4, p. 88:** anchored vectors at the block’s centre and corrected component directions and relative lengths for the drawn 31° slope.
5. **Terminal-velocity graph — Chapter 4, p. 90:** removed a duplicate terminal-speed label and enlarged/repositioned the acceleration annotations; the r5 follow-up moved “$a$ decreasing” clear of the plotted curve.
6. **Conical pendulum — Chapter 6, p. 109:** moved the radius dimension to the bob’s height and connected it to the axis and bob projection.
7. **SHM phase plots — Chapter 7, p. 118:** extended each horizontal limit so the full-period `T` tick is not clipped.
8. **SHM energy plot — Chapter 7, p. 122:** changed the equal-energy condition from only `A/√2` to the symmetric `±A/√2`.
9. **Damping comparison — Chapter 7, p. 124:** replaced the inconsistent curves with light, critical and overdamped responses sharing `x(0)=A`, `ẋ(0)=0`, and `ω₀=1 rad s⁻¹`; labeled the normalized displacement/time axes and damping ratios.

I also rechecked the cyclic-rule drawing rather than retaining the earlier diagnosis. With the node positions shown, the correct positive-product cycle `î → ĵ → k̂ → î` is clockwise; the baseline arrows and caption already agree. I restored that figure to baseline, so **it is not an edited item** and Chapter 2 has no source diff.

## Smaller readability/layout notes — dispositions

1. **Displacement-time graph, Chapter 3 p. 72 — Fixed and checked in integrated r4.** Moved the three-column legend above the axes so it no longer obscures the `Time t (s)` title.
2. **Atwood machine, Chapter 4 p. 87 — Fixed and checked in integrated r5.** Pushed the acceleration stems clear of the 4 kg and 6 kg labels as well as the blocks and weight annotations; their directions are unchanged.
3. **Vertical-circle forces, Chapter 6 p. 111 — Fixed and checked in integrated r5.** Shifted “Bottom” left of the downward $mg$ stem; the weight arrow remains vertical and rooted at the bottom point. The two top-force arrows remain separated and point toward the centre.
4. **Dot-product projection, Chapter 2 p. 57 — Fixed and checked in integrated r4.** Put the projection arrow on a short, offset baseline below $B$ and shortened its label to $A\cos\theta$; dotted guides and the explanatory dot-product equation preserve the projection meaning.
5. **Cable equilibrium, Chapter 2 p. 56 — Fixed and checked in integrated r4.** Moved the left `30°` label away from $T_1$ and aligned both arcs to the vertical reference.
6. **Work at an angle, Chapter 5 p. 95 — Fixed and rechecked in integrated r5.** Kept $F\cos\theta$ above the component arrow and moved $\theta$ left to separate the two labels; the destination block and displacement path remain clear.
7. **Magnitude from Pythagoras, Chapter 2 p. 45 — Fixed and checked in integrated r4.** Moved the magnitude formula farther below the component baseline and $A_x$ label.
8. **Triangle Rule, Chapter 2 p. 46 — Fixed and checked in integrated r4.** Offset “Head of B” above and right of the shared arrowhead endpoint.
9. **Four-vector polygon, Chapter 2 physical p. 48 / printed p. 27 — Fixed and checked in integrated r4.** Shifted $F_4$ above/right and put “End” above the final vertex.
10. **Position vectors, Chapter 2 p. 53 — Fixed and rechecked in integrated r5.** Moved the $\vect{AB}$ label below its dashed arrow; the vector remains $A\to B=\vect{r}_B-\vect{r}_A$.
11. **Spring work-energy plot, Chapter 5 p. 98 — Fixed and rechecked in integrated r5.** Moved the area equation into open upper-left plot space, clear of the curve and legend.

None of these 11 notes was a taste-only styling preference: each identified an overlap or tight separation that could impede reading, so each received a targeted diagram-only correction. None is marked optional / not required: all 11 notes identified overlaps or tight separation that could impede reading, rather than taste-only styling preferences. **Scientific check:** the cable problem explicitly states 30° and 45° from vertical and its coordinates/equations use those angles. The baseline left arc ended at 122° (32°), despite the stated 30° convention; its origin was also offset from the vertical reference. Both arcs now start on the vertical reference and the left arc ends at 120°, matching the stated problem. No physics convention remains unresolved. The vertical-circle top forces remain downward toward the centre; their small lateral offset is solely for legibility.

**Front matter:** the title emblem on p. 2 is decorative, but its nucleus and three electron-like dots on elliptical paths can be read as a planetary/Bohr atom model. Recommendation: replace it with non-orbital abstract geometry or add an explicit “decorative, not an atomic model” cue. I made no cover change. The p. 4 dedication frame is purely decorative and has no physics-teaching claim; no change is recommended.

**Final integrated verification:** all 20 edited instructional figures pass their post-edit visual checks, and all 33 inventoried items (including the two decorative front-matter graphics) remain accounted for. The eight pages with the latest collision fixes—items 14, 21, 22, 24–26, 29, and 33—were checked in the final integrated r5 PDF; no locator shift or overlap remains. Other source-edited figures passed their earlier integrated post-edit checks and had no later source changes. The decorative atom emblem remains unchanged; see the recommendation above. No diagram residual requiring a source edit remains in this range.
