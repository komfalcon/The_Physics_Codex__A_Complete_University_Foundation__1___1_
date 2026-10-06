# Diagram Audit — Chapter 1 through Printed Page 246

## Scope and result

- **Source scope:** Included front matter plus Chapters 1–17, ending at printed page 246.
- **Compiled artifact:** `book_main.pdf`, **513 PDF pages**.
- **Endpoint mapping:** printed page **246 = PDF viewer page 271**; printed page 245 = PDF page 270; printed page 247 = PDF page 272.
- **Endpoint visual result:** PASS only for the directly inspected endpoint diagram. The wavelength annotation is fully visible, both crest markers remain inside the panel, and no panel edge clips the wave or annotations.
- **Whole-scope publication status:** NOT YET CERTIFIED. The inventory and clean compilation cover the scope, but the remaining diagrams require individual visual review before all can be called publication-ready.
- **Build result:** PASS from clean auxiliaries with `latexmk -pdf -interaction=nonstopmode -file-line-error -halt-on-error book_main.tex`.
- **Source changes required by this audit:** none beyond the already-present page-246 repair in commit `f0c305e`; this branch records the audit evidence rather than duplicating that fix.

## Defect classification

| Area | Result | Evidence |
|---|---|---|
| Geometry / scope containment | PASS | Chapter 17 endpoint source defines named coordinates inside the scaled scope and uses an explicit bounding box. |
| Typography / clipping | PASS at endpoint | PDF page 271 render shows the full wavelength label, crest labels, trough label, and equations. |
| Panel / page overflow | PASS at endpoint | PDF page 271 render shows all endpoint diagram content inside the `diagbox`; adjacent pages 270 and 272 remain stable. |
| Compilation | PASS | 513-page PDF generated from clean auxiliaries. |
| Warnings | REVIEW / pre-existing | Build contains many pre-existing overfull-box warnings in exercise layouts and missing-character diagnostics; no compilation failure or undefined-reference failure occurred. |

## Inventory

The inventory contains **86 TikZ blocks** across the included front matter and Chapters 1–17. `axis` counts identify PGFPlots blocks nested inside each TikZ picture. The source line range is the audit anchor. **Inventory status is not a visual publication certification:** only the page-246 endpoint and its adjacent pages were individually rendered and inspected in this milestone.

| # | Source file | Lines | PGFPlots axes | Nearby section | Audit result |
|---:|---|---:|---:|---|---|
| 1 | `front_matter/dedication.tex` | 11–14 | 0 | — | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 2 | `front_matter/titlepage.tex` | 25–40 | 0 | — | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 3 | `chapters/part1_mechanics/ch01_measurement.tex` | 835–890 | 0 | Reading a Vernier Calliper | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 4 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 124–131 | 0 | Equal Vectors | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 5 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 186–200 | 0 | Parallel and Anti-parallel | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 6 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 341–356 | 0 | Magnitude from Pythagoras | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 7 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 444–461 | 0 | Vector Representation | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 8 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 491–504 | 0 | Triangle Rule | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 9 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 534–555 | 0 | Parallelogram Rule | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 10 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 588–615 | 0 | Polygon Rule: Four Vectors | REVIEWED — see BATCH1_DIAGRAM_REVIEW.md |
| 11 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 621–640 | 0 | Closed Polygon: Equilibrium | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 12 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 712–722 | 0 | Calculating the Resultant Analytically | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 13 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 790–818 | 0 | Resolution of a Vector | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 14 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1039–1061 | 0 | Position Vectors in 2D | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 15 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1254–1275 | 0 | Equilibrium of Forces | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 16 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1345–1367 | 0 | Geometric Meaning of the Dot Product | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 17 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1593–1616 | 0 | Right-Hand Rule | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 18 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1641–1656 | 0 | The Vector (Cross) Product | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 19 | `chapters/part1_mechanics/ch03_kinematics.tex` | 303–334 | 1 | Displacement-Time Graphs | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 20 | `chapters/part1_mechanics/ch03_kinematics.tex` | 358–396 | 1 | Velocity-Time Graph | REVIEWED — see BATCH2_DIAGRAM_REVIEW.md |
| 21 | `chapters/part1_mechanics/ch03_kinematics.tex` | 593–639 | 1 | Projectile Motion Trajectory | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 22 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 363–398 | 0 | Connected Bodies and Pulleys | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 23 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 434–469 | 0 | Forces on an Inclined Plane | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 24 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 597–628 | 1 | Velocity-Time Graph for Terminal Velocity | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 25 | `chapters/part1_mechanics/ch05_work_energy_power.tex` | 65–96 | 0 | Work Done at an Angle | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 26 | `chapters/part1_mechanics/ch05_work_energy_power.tex` | 329–349 | 1 | Work Done in Stretching a Spring | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 27 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 121–154 | 0 | Angular and Linear Quantities | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 28 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 248–278 | 0 | Centripetal Acceleration and Force | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 29 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 406–439 | 0 | Vertical Circle --- Forces at Key Points | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 30 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 144–198 | 3 | SHM Graphs --- Displacement, Velocity, Acceleration | REVIEWED — see BATCH3_DIAGRAM_REVIEW.md |
| 31 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 301–336 | 0 | The Simple Pendulum | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 32 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 497–525 | 1 | Energy vs Displacement in SHM | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 33 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 599–627 | 1 | Damping Comparison | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 34 | `chapters/part1_mechanics/ch08_gravitation.tex` | 88–111 | 0 | Gravitational Force Between Two Masses | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 35 | `chapters/part1_mechanics/ch08_gravitation.tex` | 272–298 | 1 | $g$ vs Distance from Earth's Centre | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 36 | `chapters/part1_mechanics/ch09_elasticity.tex` | 120–157 | 1 | Force-Extension Graph (Hooke's Law Region) | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 37 | `chapters/part1_mechanics/ch09_elasticity.tex` | 274–320 | 0 | Series vs Parallel Springs | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 38 | `chapters/part1_mechanics/ch09_elasticity.tex` | 450–535 | 1 | Stress-Strain Graph for a Ductile Metal (Steel) | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 39 | `chapters/part1_mechanics/ch09_elasticity.tex` | 605–637 | 1 | Comparing Stress-Strain Curves | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 40 | `chapters/part1_mechanics/ch10_simple_machines.tex` | 215–274 | 0 | The Three Classes of Lever | REVIEWED — see BATCH4_DIAGRAM_REVIEW.md |
| 41 | `chapters/part1_mechanics/ch10_simple_machines.tex` | 353–382 | 0 | The Inclined Plane | INVENTORIED — individual visual review still required |
| 42 | `chapters/part1_mechanics/ch10_simple_machines.tex` | 463–514 | 0 | Pulley Systems | INVENTORIED — individual visual review still required |
| 43 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 125–171 | 0 | Visualising Density | INVENTORIED — individual visual review still required |
| 44 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 273–332 | 0 | Pressure Depends on Area | INVENTORIED — individual visual review still required |
| 45 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 431–481 | 0 | Pressure Increases with Depth | INVENTORIED — individual visual review still required |
| 46 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 508–562 | 0 | The Hydrostatic Paradox: Same Depth = Same Pressure | INVENTORIED — individual visual review still required |
| 47 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 653–710 | 0 | Hydraulic Lift: Pascal's Principle in Action | INVENTORIED — individual visual review still required |
| 48 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 801–858 | 0 | The Intuition: The Displaced Water Fights Back | INVENTORIED — individual visual review still required |
| 49 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 882–937 | 0 | Floating, Sinking and Neutral Buoyancy | INVENTORIED — individual visual review still required |
| 50 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 86–145 | 0 | Interior vs Surface Molecule: Intermolecular Forces | INVENTORIED — individual visual review still required |
| 51 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 293–358 | 0 | Excess Pressure: Drop vs Bubble | INVENTORIED — individual visual review still required |
| 52 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 440–519 | 0 | Capillary Rise and Fall: Water vs Mercury | INVENTORIED — individual visual review still required |
| 53 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 556–616 | 0 | Capillary Rise Formula: Narrower Tube Rises Higher | INVENTORIED — individual visual review still required |
| 54 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 693–738 | 0 | Laminar Flow: Velocity Profile in a Viscous Fluid | INVENTORIED — individual visual review still required |
| 55 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 830–875 | 0 | Forces on a Sphere Falling Through Viscous Fluid | INVENTORIED — individual visual review still required |
| 56 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 960–1020 | 0 | Laminar vs Turbulent Flow | INVENTORIED — individual visual review still required |
| 57 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 156–219 | 0 | Comparing Temperature Scales | INVENTORIED — individual visual review still required |
| 58 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 313–368 | 0 | Liquid-in-Glass Thermometer: Cross-Section | INVENTORIED — individual visual review still required |
| 59 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 424–466 | 0 | Thermometer Calibration | INVENTORIED — individual visual review still required |
| 60 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 521–574 | 1 | Molecular Origin of Thermal Expansion | INVENTORIED — individual visual review still required |
| 61 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 675–745 | 0 | Linear, Area and Volume Expansion Illustrated | INVENTORIED — individual visual review still required |
| 62 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 803–861 | 0 | The Bimetallic Strip: Principle and Applications | INVENTORIED — individual visual review still required |
| 63 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 1008–1048 | 1 | Density of Water vs Temperature | INVENTORIED — individual visual review still required |
| 64 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 103–160 | 2 | Boyle's Law: $P$ vs $V$ and $P$ vs $1/V$ Graphs | INVENTORIED — individual visual review still required |
| 65 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 232–291 | 1 | Charles' Law: $V$ vs $T$ Graph | INVENTORIED — individual visual review still required |
| 66 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 535–593 | 0 | Kinetic Model: Gas Molecules in a Container | INVENTORIED — individual visual review still required |
| 67 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 714–751 | 1 | Maxwell-Boltzmann Speed Distribution | INVENTORIED — individual visual review still required |
| 68 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 816–851 | 1 | $PV/nRT$ vs $P$ for Ideal and Real Gases | INVENTORIED — individual visual review still required |
| 69 | `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex` | 199–265 | 0 | Electrical Calorimetry Setup | INVENTORIED — individual visual review still required |
| 70 | `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex` | 339–405 | 0 | Method of Mixtures: Before and After | INVENTORIED — individual visual review still required |
| 71 | `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex` | 531–580 | 1 | Complete Heating Curve: Ice to Steam | INVENTORIED — individual visual review still required |
| 72 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 93–165 | 0 | Conduction: Molecular Vibration Chain in a Solid | INVENTORIED — individual visual review still required |
| 73 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 241–284 | 0 | Fourier's Law: Heat Flow Through a Slab | INVENTORIED — individual visual review still required |
| 74 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 396–452 | 0 | Natural Convection Loop in a Liquid | INVENTORIED — individual visual review still required |
| 75 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 466–529 | 0 | Sea Breeze (Daytime) and Land Breeze (Night-time) | INVENTORIED — individual visual review still required |
| 76 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 557–639 | 0 | Good and Poor Emitters/Absorbers of Radiation | INVENTORIED — individual visual review still required |
| 77 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 793–924 | 0 | The Greenhouse Effect | INVENTORIED — individual visual review still required |
| 78 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 985–1023 | 0 | Comparing the Three Mechanisms | INVENTORIED — individual visual review still required |
| 79 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 100–175 | 0 | Transverse vs Longitudinal Waves | PASS — source/render review; no endpoint-scope issue observed |
| 80 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 216–326 | 0 | Wave Profile: Key Parameters Labelled | PASS — source/render review; no endpoint-scope issue observed |
| 81 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 399–436 | 0 | Wave Reflection | INVENTORIED — individual visual review still required |
| 82 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 480–544 | 0 | Diffraction Through a Gap | INVENTORIED — individual visual review still required |
| 83 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 585–640 | 0 | Constructive and Destructive Interference | INVENTORIED — individual visual review still required |
| 84 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 682–738 | 0 | Standing Wave: Nodes and Antinodes | INVENTORIED — individual visual review still required |
| 85 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 796–865 | 0 | Harmonics on a String Fixed at Both Ends | INVENTORIED — individual visual review still required |
| 86 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 905–987 | 0 | Harmonics in Open and Closed Pipes | INVENTORIED — individual visual review still required |

## Endpoint evidence

The endpoint render is retained at `audit-renders/page271.png`. The neighboring renders are `audit-renders/page270.png` and `audit-renders/page272.png`.

## Follow-up

The build warning set should be handled separately from this diagram milestone. The next milestone can reuse this inventory format for diagrams after printed page 246.
