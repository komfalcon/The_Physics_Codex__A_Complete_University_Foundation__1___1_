# Batch 3 Diagram Review — Items 21–30

## Scope

This batch covers the projectile-motion diagram, Newtonian dynamics figures through terminal velocity, the work and spring-energy figures, and the circular-motion and SHM figures listed as inventory items 21–30.

## Review standard

Each item was checked against its surrounding prose and equations for scientific accuracy, label and arrow correctness, learner clarity, print-size readability, and TikZ/PGFPlots containment. The final PDF pages were rendered at 120 dpi and inspected after the source changes.

## Results

| # | Source / lines | Diagram | Scientific verdict | Action | Visual/readability result | PDF page | Unresolved uncertainty |
|---:|---|---|---|---|---|---:|---|
| 21 | `chapters/part1_mechanics/ch03_kinematics.tex:593–639` | Projectile Motion Trajectory | PASS | No source change. For $u=20\ \text{m\,s}^{-1}$, $\theta=45^\circ$, and $g=10\ \text{m\,s}^{-2}$, the plotted trajectory reaches $H_{max}=10\ \text{m}$ at $x=20\ \text{m}$ and $R=40\ \text{m}$, matching the equations and labels. | Curve, maximum-height construction, range marker, axes, and legend are fully visible inside the diagram box. | 80 | None identified. |
| 22 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex:363–398` | Connected Bodies and Pulleys | NEEDS FIX — corrected | The lighter block A was labeled `$a$ (up)` while its arrow pointed downward. The endpoint was changed from `(-0.5,-1.5)` to `(-0.5,-0.5)`, so A's arrow now points upward while heavier B's arrow points downward, matching the text and equations. | Final render clearly distinguishes the upward A acceleration and downward B acceleration; labels and force arrows remain separated. | 91 | None identified. |
| 23 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex:434–469` | Forces on an Inclined Plane | PASS | No source change. The incline has slope $\arctan(3/5)\approx31^\circ$, matching the block rotation and the displayed $\theta$; weight, normal reaction, and the $mg\sin\theta$/$mg\cos\theta$ components have correct directions. | Diagram is balanced and readable; component labels do not clip or overlap the incline or block. | 92 | None identified. |
| 24 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex:597–628` | Velocity-Time Graph for Terminal Velocity | PASS | No source change. The exponential curve starts at zero, approaches the dashed $v_T=55\ \text{m\,s}^{-1}$ asymptote, and its decreasing gradient correctly represents falling acceleration toward zero. | Axes, units, asymptote, curve, and acceleration annotations are legible and contained. | 94 | None identified. |
| 25 | `chapters/part1_mechanics/ch05_work_energy_power.tex:65–96` | Work Done at an Angle | PASS | No source change. The applied force is at $26.6^\circ$ to the horizontal displacement construction, and the figure correctly emphasizes that only $F\cos\theta$ contributes to work. | Force, displacement, component, angle, and formula are readable at print-review size with safe margins. | 99 | None identified. |
| 26 | `chapters/part1_mechanics/ch05_work_energy_power.tex:329–349` | Work Done in Stretching a Spring | NEEDS FIX — corrected | The original title “Work Done by a Spring Force” could imply the signed work done by the restoring force, whereas the positive area shown is work done in stretching the spring and elastic potential energy stored. The title and caption now state that interpretation explicitly. | Final graph, shaded triangular area, equation, title, and explanatory caption are clear and contained. | 102 | None identified. |
| 27 | `chapters/part1_mechanics/ch06_circular_motion.tex:121–154` | Angular and Linear Quantities | PASS | No source change. The radius, arc $s=r\theta$, $45^\circ$ angular displacement, and tangent velocity $v=r\omega$ are geometrically consistent. | Circle, points, arc, radius, angle, and tangent arrow are legible without clipping or overlap. | 112 | None identified. |
| 28 | `chapters/part1_mechanics/ch06_circular_motion.tex:248–278` | Centripetal Acceleration and Force (conical pendulum example) | NEEDS FIX — corrected | The original tension arrow was vertical even though tension acts along the string toward the pivot; the angle arc was also drawn on the wrong side of the vertical. The tension arrow now runs from the ball to the pivot, and the $30^\circ$ arc is on the correct side. | Final render shows the string, tension, weight, centripetal-force arrow, radius, and angle distinctly and without clipping. | 113 | None identified. |
| 29 | `chapters/part1_mechanics/ch06_circular_motion.tex:406–439` | Vertical Circle — Forces at Key Points | NEEDS FIX — corrected | The force directions and bottom/top speed labels were correct, but the explanatory note was too close to the bottom $mg$ label at print size. The note was moved downward locally to improve separation. | Final render has readable bottom/top force labels, speed vectors, and explanatory note inside the diagram box. | 115 | None identified. |
| 30 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex:144–198` | SHM Graphs — Displacement, Velocity, Acceleration | PASS | No source change. For the displayed sine initial condition, velocity is the cosine derivative and acceleration is $-\omega^2x$; the three plots have the correct phase relationships and extrema. | All three stacked PGFPlots panels, phase ticks, labels, titles, and note are legible and contained. | 122 | None identified. |

## Validation

- Clean LaTeX compilation succeeded with `latexmk -pdf -interaction=nonstopmode -file-line-error -halt-on-error book_main.tex`.
- Output remains **513 PDF pages**, A4.
- Final renders inspected at 120 dpi included PDF pages 80, 91–92, 94, 99, 102, 112–115, and 122, with adjacent-page checks where relevant.
- The repaired pulley, spring, conical-pendulum, and vertical-circle figures were visually rechecked after compilation.
- No fatal errors or new warnings were introduced by the Batch 3 changes.

## Build note

The repository still emits pre-existing unresolved references including `tab:si_base`, `tab:prefixes`, `tab:instruments`, `sec:unit_vectors`, `sec:position_vectors`, `sec:component_method`, `tab:densities`, `tab:viscosity`, and `tab:expansion`. The build also retains the repository's pre-existing overfull-box diagnostics. These are unrelated to the Batch 3 diagram changes and were not repaired in this batch.

## Progress

Items **21–30** are now individually reviewed, for **30 of 86** inventory diagrams reviewed. Items **31–86** remain unreviewed and are not certified by this report.
