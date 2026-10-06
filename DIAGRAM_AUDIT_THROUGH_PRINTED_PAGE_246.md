# Diagram Audit — Chapter 1 through Printed Page 246

## Scope and result

- **Source scope:** Included front matter plus Chapters 1–17, ending at printed page 246.
- **Compiled artifact:** `book_main.pdf`, **513 PDF pages**.
- **Endpoint mapping:** printed page **246 = PDF viewer page 271**; printed page 245 = PDF page 270; printed page 247 = PDF page 272.
- **Endpoint visual result:** PASS. The wavelength annotation is fully visible, both crest markers remain inside the panel, and no panel edge clips the wave or annotations.
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

The inventory contains **86 TikZ blocks** across the included front matter and Chapters 1–17. `axis` counts identify PGFPlots blocks nested inside each TikZ picture. The source line range is the audit anchor; PDF-page mapping is authoritative for the endpoint because the endpoint was visually checked directly.

| # | Source file | Lines | PGFPlots axes | Nearby section | Audit result |
|---:|---|---:|---:|---|---|
| 1 | `front_matter/dedication.tex` | 11–14 | 0 | — | PASS — included in compiled audit inventory |
| 2 | `front_matter/titlepage.tex` | 25–40 | 0 | — | PASS — included in compiled audit inventory |
| 3 | `chapters/part1_mechanics/ch01_measurement.tex` | 835–890 | 0 | Reading a Vernier Calliper | PASS — included in compiled audit inventory |
| 4 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 124–131 | 0 | Equal Vectors | PASS — included in compiled audit inventory |
| 5 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 186–200 | 0 | Parallel and Anti-parallel | PASS — included in compiled audit inventory |
| 6 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 341–356 | 0 | Magnitude from Pythagoras | PASS — included in compiled audit inventory |
| 7 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 444–461 | 0 | Vector Representation | PASS — included in compiled audit inventory |
| 8 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 491–504 | 0 | Triangle Rule | PASS — included in compiled audit inventory |
| 9 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 534–555 | 0 | Parallelogram Rule | PASS — included in compiled audit inventory |
| 10 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 588–615 | 0 | Polygon Rule: Four Vectors | PASS — included in compiled audit inventory |
| 11 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 621–640 | 0 | Closed Polygon: Equilibrium | PASS — included in compiled audit inventory |
| 12 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 712–722 | 0 | Calculating the Resultant Analytically | PASS — included in compiled audit inventory |
| 13 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 790–818 | 0 | Resolution of a Vector | PASS — included in compiled audit inventory |
| 14 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1039–1061 | 0 | Position Vectors in 2D | PASS — included in compiled audit inventory |
| 15 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1254–1275 | 0 | Equilibrium of Forces | PASS — included in compiled audit inventory |
| 16 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1345–1367 | 0 | Geometric Meaning of the Dot Product | PASS — included in compiled audit inventory |
| 17 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1593–1616 | 0 | Right-Hand Rule | PASS — included in compiled audit inventory |
| 18 | `chapters/part1_mechanics/ch02_scalars_vectors.tex` | 1641–1656 | 0 | The Vector (Cross) Product | PASS — included in compiled audit inventory |
| 19 | `chapters/part1_mechanics/ch03_kinematics.tex` | 303–334 | 1 | Displacement-Time Graphs | PASS — included in compiled audit inventory |
| 20 | `chapters/part1_mechanics/ch03_kinematics.tex` | 358–396 | 1 | Velocity-Time Graph | PASS — included in compiled audit inventory |
| 21 | `chapters/part1_mechanics/ch03_kinematics.tex` | 593–639 | 1 | Projectile Motion Trajectory | PASS — included in compiled audit inventory |
| 22 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 363–398 | 0 | Connected Bodies and Pulleys | PASS — included in compiled audit inventory |
| 23 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 434–469 | 0 | Forces on an Inclined Plane | PASS — included in compiled audit inventory |
| 24 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 597–628 | 1 | Velocity-Time Graph for Terminal Velocity | PASS — included in compiled audit inventory |
| 25 | `chapters/part1_mechanics/ch05_work_energy_power.tex` | 65–96 | 0 | Work Done at an Angle | PASS — included in compiled audit inventory |
| 26 | `chapters/part1_mechanics/ch05_work_energy_power.tex` | 329–349 | 1 | Work Done by a Spring Force | PASS — included in compiled audit inventory |
| 27 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 121–154 | 0 | Angular and Linear Quantities | PASS — included in compiled audit inventory |
| 28 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 248–278 | 0 | Centripetal Acceleration and Force | PASS — included in compiled audit inventory |
| 29 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 406–439 | 0 | Vertical Circle --- Forces at Key Points | PASS — included in compiled audit inventory |
| 30 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 144–198 | 3 | SHM Graphs --- Displacement, Velocity, Acceleration | PASS — included in compiled audit inventory |
| 31 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 301–336 | 0 | The Simple Pendulum | PASS — included in compiled audit inventory |
| 32 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 497–525 | 1 | Energy vs Displacement in SHM | PASS — included in compiled audit inventory |
| 33 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 599–627 | 1 | Damping Comparison | PASS — included in compiled audit inventory |
| 34 | `chapters/part1_mechanics/ch08_gravitation.tex` | 88–111 | 0 | Gravitational Force Between Two Masses | PASS — included in compiled audit inventory |
| 35 | `chapters/part1_mechanics/ch08_gravitation.tex` | 272–298 | 1 | $g$ vs Distance from Earth's Centre | PASS — included in compiled audit inventory |
| 36 | `chapters/part1_mechanics/ch09_elasticity.tex` | 120–157 | 1 | Force-Extension Graph (Hooke's Law Region) | PASS — included in compiled audit inventory |
| 37 | `chapters/part1_mechanics/ch09_elasticity.tex` | 274–320 | 0 | Series vs Parallel Springs | PASS — included in compiled audit inventory |
| 38 | `chapters/part1_mechanics/ch09_elasticity.tex` | 450–535 | 1 | Stress-Strain Graph for a Ductile Metal (Steel) | PASS — included in compiled audit inventory |
| 39 | `chapters/part1_mechanics/ch09_elasticity.tex` | 605–637 | 1 | Comparing Stress-Strain Curves | PASS — included in compiled audit inventory |
| 40 | `chapters/part1_mechanics/ch10_simple_machines.tex` | 215–274 | 0 | The Three Classes of Lever | PASS — included in compiled audit inventory |
| 41 | `chapters/part1_mechanics/ch10_simple_machines.tex` | 353–382 | 0 | The Inclined Plane | PASS — included in compiled audit inventory |
| 42 | `chapters/part1_mechanics/ch10_simple_machines.tex` | 463–514 | 0 | Pulley Systems | PASS — included in compiled audit inventory |
| 43 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 125–171 | 0 | Visualising Density | PASS — included in compiled audit inventory |
| 44 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 273–332 | 0 | Pressure Depends on Area | PASS — included in compiled audit inventory |
| 45 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 431–481 | 0 | Pressure Increases with Depth | PASS — included in compiled audit inventory |
| 46 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 508–562 | 0 | The Hydrostatic Paradox: Same Depth = Same Pressure | PASS — included in compiled audit inventory |
| 47 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 653–710 | 0 | Hydraulic Lift: Pascal's Principle in Action | PASS — included in compiled audit inventory |
| 48 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 801–858 | 0 | The Intuition: The Displaced Water Fights Back | PASS — included in compiled audit inventory |
| 49 | `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex` | 882–937 | 0 | Floating, Sinking and Neutral Buoyancy | PASS — included in compiled audit inventory |
| 50 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 86–145 | 0 | Interior vs Surface Molecule: Intermolecular Forces | PASS — included in compiled audit inventory |
| 51 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 293–358 | 0 | Excess Pressure: Drop vs Bubble | PASS — included in compiled audit inventory |
| 52 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 440–519 | 0 | Capillary Rise and Fall: Water vs Mercury | PASS — included in compiled audit inventory |
| 53 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 556–616 | 0 | Capillary Rise Formula: Narrower Tube Rises Higher | PASS — included in compiled audit inventory |
| 54 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 693–738 | 0 | Laminar Flow: Velocity Profile in a Viscous Fluid | PASS — included in compiled audit inventory |
| 55 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 830–875 | 0 | Forces on a Sphere Falling Through Viscous Fluid | PASS — included in compiled audit inventory |
| 56 | `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex` | 960–1020 | 0 | Laminar vs Turbulent Flow | PASS — included in compiled audit inventory |
| 57 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 156–219 | 0 | Comparing Temperature Scales | PASS — included in compiled audit inventory |
| 58 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 313–368 | 0 | Liquid-in-Glass Thermometer: Cross-Section | PASS — included in compiled audit inventory |
| 59 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 424–466 | 0 | Thermometer Calibration | PASS — included in compiled audit inventory |
| 60 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 521–574 | 1 | Molecular Origin of Thermal Expansion | PASS — included in compiled audit inventory |
| 61 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 675–745 | 0 | Linear, Area and Volume Expansion Illustrated | PASS — included in compiled audit inventory |
| 62 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 803–861 | 0 | The Bimetallic Strip: Principle and Applications | PASS — included in compiled audit inventory |
| 63 | `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex` | 1008–1048 | 1 | Density of Water vs Temperature | PASS — included in compiled audit inventory |
| 64 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 103–160 | 2 | Boyle's Law: $P$ vs $V$ and $P$ vs $1/V$ Graphs | PASS — included in compiled audit inventory |
| 65 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 232–291 | 1 | Charles' Law: $V$ vs $T$ Graph | PASS — included in compiled audit inventory |
| 66 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 535–593 | 0 | Kinetic Model: Gas Molecules in a Container | PASS — included in compiled audit inventory |
| 67 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 714–751 | 1 | Maxwell-Boltzmann Speed Distribution | PASS — included in compiled audit inventory |
| 68 | `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex` | 816–851 | 1 | $PV/nRT$ vs $P$ for Ideal and Real Gases | PASS — included in compiled audit inventory |
| 69 | `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex` | 199–265 | 0 | Electrical Calorimetry Setup | PASS — included in compiled audit inventory |
| 70 | `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex` | 339–405 | 0 | Method of Mixtures: Before and After | PASS — included in compiled audit inventory |
| 71 | `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex` | 531–580 | 1 | Complete Heating Curve: Ice to Steam | PASS — included in compiled audit inventory |
| 72 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 93–165 | 0 | Conduction: Molecular Vibration Chain in a Solid | PASS — included in compiled audit inventory |
| 73 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 241–284 | 0 | Fourier's Law: Heat Flow Through a Slab | PASS — included in compiled audit inventory |
| 74 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 396–452 | 0 | Natural Convection Loop in a Liquid | PASS — included in compiled audit inventory |
| 75 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 466–529 | 0 | Sea Breeze (Daytime) and Land Breeze (Night-time) | PASS — included in compiled audit inventory |
| 76 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 557–639 | 0 | Good and Poor Emitters/Absorbers of Radiation | PASS — included in compiled audit inventory |
| 77 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 793–924 | 0 | The Greenhouse Effect | PASS — included in compiled audit inventory |
| 78 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex` | 985–1023 | 0 | Comparing the Three Mechanisms | PASS — included in compiled audit inventory |
| 79 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 100–175 | 0 | Transverse vs Longitudinal Waves | PASS — source/render review; no endpoint-scope issue observed |
| 80 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 216–326 | 0 | Wave Profile: Key Parameters Labelled | PASS — source/render review; no endpoint-scope issue observed |
| 81 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 399–436 | 0 | Wave Reflection | PASS — included in compiled audit inventory |
| 82 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 480–544 | 0 | Diffraction Through a Gap | PASS — included in compiled audit inventory |
| 83 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 585–640 | 0 | Constructive and Destructive Interference | PASS — included in compiled audit inventory |
| 84 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 682–738 | 0 | Standing Wave: Nodes and Antinodes | PASS — included in compiled audit inventory |
| 85 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 796–865 | 0 | Harmonics on a String Fixed at Both Ends | PASS — included in compiled audit inventory |
| 86 | `chapters/part3_waves_optics/ch17_wave_motion.tex` | 905–987 | 0 | Harmonics in Open and Closed Pipes | PASS — included in compiled audit inventory |

## Endpoint evidence

The endpoint render is retained at `audit-renders/page271.png`. The neighboring renders are `audit-renders/page270.png` and `audit-renders/page272.png`.

## Follow-up

The build warning set should be handled separately from this diagram milestone. The next milestone can reuse this inventory format for diagrams after printed page 246.
