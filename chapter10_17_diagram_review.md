# The Physics Codex — Chapters 10–17 diagram review

All 46 inventoried entries numbered 41–86 were checked against source and the rendered PDF. After the fixes below, 39 entries pass and seven minor issues remain: #53, #54, #57, #68, #73, #74 and #79. The previously identified major and moderate diagram/physics issues have been corrected and rechecked in the forced 507-page build. One inventory title was also corrected: #78 is the thermos-flask figure, not a comparison of heat-transfer mechanisms. Page numbers below are PDF pages; printed folios are in parentheses where supplied.

## Chapter 10 — Simple Machines

- **#41 The Inclined Plane** — `chapters/part1_mechanics/ch10_simple_machines.tex:353–382`, PDF p. 159 (printed p. 138). **Pass after correction.** The horizontal run is labelled `ℓ cos θ`; the vertical height remains `h` and the slope length is `ℓ`. Rebuilt and visually checked.
- **#42 Pulley Systems** — `chapters/part1_mechanics/ch10_simple_machines.tex:463–514`, PDF p. 160 (printed p. 139). **Pass after correction.** One continuous rope is anchored at the ceiling, supports the movable pulley on two strands, passes over the offset fixed pulley, and ends at the correctly directed effort arrow. Rebuilt and visually checked.
- **#40 The Three Classes of Lever** — PDF p. 162. **Pass.** The prior review reports the revised labels and lever geometry clear; see `BATCH4_DIAGRAM_REVIEW.md`.

## Chapter 11 — Density, Pressure and Archimedes’ Principle

- **#43 Visualising Density** — `chapters/part2_fluids_thermal/ch11_density_pressure_archimedes.tex:123–176`, PDF p. 172 (printed p. 151). **Pass.**
- **#44 Pressure Depends on Area** — `…:271–336`, PDF p. 174 (printed p. 153). **Pass.**
- **#45 Pressure Increases with Depth** — `…:429–488`, PDF p. 175 (printed p. 154). **Pass.** The completed source/PDF review found no blocking issue.
- **#46 The Hydrostatic Paradox: Same Depth = Same Pressure** — `…:506–564`, PDF p. 176 (printed p. 155). **Pass after correction.** The diagram now compares three separate vessel shapes with the same free-surface height, marking sample points the same depth below their free surfaces. Rebuilt and visually checked.
- **#47 Hydraulic Lift: Pascal’s Principle in Action** — `…:651–710`, PDF p. 177 (printed p. 156). **Pass after correction.** The annotations now describe transmission of the applied pressure increment `ΔP`; the caption also notes that absolute pressure varies with height in a static fluid.
- **#48 The Intuition: The Displaced Water Fights Back** — `…:799–860`, PDF p. 179 (printed p. 158). **Pass after correction.** The debug grid was removed; all three stages are visible in the rebuilt PDF.
- **#49 Floating, Sinking and Neutral Buoyancy** — `…:889–935`, PDF p. 179 (printed p. 158). **Pass after correction.** Weight arrows point down and upthrust arrows point up; equal forces are shown for floating/neutral cases and `W > U` for sinking. Rebuilt and visually checked.

## Chapter 12 — Surface Tension, Viscosity and Capillarity

- **#50 Interior vs Surface Molecule: Intermolecular Forces** — `chapters/part2_fluids_thermal/ch12_surface_tension_viscosity_capillarity.tex:86–145`. **Pass.**
- **#51 Excess Pressure: Drop vs Bubble** — `…:293–358`. **Pass after correction.** Bubble film fills are drawn before both surface outlines so both interfaces remain visible.
- **#52 Capillary Rise and Fall: Water vs Mercury** — `…:440–519`. **Pass.**
- **#53 Capillary Rise Formula: Narrower Tube Rises Higher** — `…:556–616`. **Minor issue remains.** Align each height arrow with the stated meniscus reference (normally the lowest point), or clarify that the arrow is schematic.
- **#54 Laminar Flow: Velocity Profile in a Viscous Fluid** — `…:693–738`. **Minor issue remains.** Use an unambiguous transverse coordinate for the vertical gradient, such as `dv/dy`, or define the plotted transverse coordinate and apply it consistently.
- **#55 Forces on a Sphere Falling Through Viscous Fluid** — `…:843–868`, PDF p. 196 (printed p. 175). **Pass after correction.** Weight is downward, upthrust and drag are upward, and the to-scale annotation matches `W = U + F_d`. Rebuilt and visually checked.
- **#56 Laminar vs Turbulent Flow** — `…:960–1020`. **Pass.**

## Chapter 13 — Temperature and Thermal Expansion

- **#57 Comparing Temperature Scales** — `chapters/part2_fluids_thermal/ch13_temperature_thermal_expansion.tex:156–219`. **Minor issue remains.** Kelvin and Celsius increments are equal; the schematic should not imply that Kelvin intervals are larger. Mark it as schematic or correct the graduation spacing.
- **#58 Liquid-in-Glass Thermometer: Cross-Section** — `…:337–348`, PDF p. 206 (printed p. 185). **Pass after correction.** The duplicate tick-label loop was removed, leaving one readable set of scale values. Rebuilt and visually checked.
- **#59 Thermometer Calibration** — `…:424–466`. **Pass.**
- **#60 Molecular Origin of Thermal Expansion** — `…:538–567`, PDF p. 208 (printed p. 187). **Pass after correction.** The energy-level endpoints now meet the plotted Lennard-Jones-like curve at the displayed energies, with the high-temperature mean position to the right of the low-temperature mean. Rebuilt and visually checked.
- **#61 Linear, Area and Volume Expansion Illustrated** — `…:675–745`. **Pass.**
- **#62 The Bimetallic Strip: Principle and Applications** — `…:803–861`. **Pass after correction.** The heated strip now bends downward, with the higher-expansion brass on the longer outer arc and steel on the shorter inner arc. Rebuilt and visually checked.
- **#63 Density of Water vs Temperature** — `…:1013–1040`, PDF p. 213 (printed p. 192). **Pass after correction.** The empirical curve now stays within the axes over 0–25°C and has its maximum near 4°C. Rebuilt and visually checked.

## Chapter 14 — Gas Laws and Kinetic Theory

- **#64 Boyle’s Law: P–V and P–1/V Graphs** — `chapters/part2_fluids_thermal/ch14_gas_laws_kinetic_theory.tex:103–160`, PDF p. 220 (printed p. 199). **Pass after correction.** The hyperbolas now follow `P=a/V` without an additive pressure offset.
- **#65 Charles’ Law: V–T Graph** — `…:235–273`, PDF p. 221 (printed p. 200). **Pass after correction.** Celsius coordinates and axis labels now agree, pressure/slope ordering is consistent, and the unsupported 0°C “real gas region” boundary was removed. Rebuilt and visually checked.
- **#66 Kinetic Model: Gas Molecules in a Container** — `…:569–575`, PDF p. 225 (printed p. 204). **Pass after correction.** The label now defines pressure as normal force per unit area and gives `P=F_⊥/A`. Rebuilt and visually checked.
- **#67 Maxwell–Boltzmann Speed Distribution** — `…:711–745`, PDF p. 227 (printed p. 206). **Pass after correction.** The distributions are normalized to unit area and fit within the plot. Rebuilt and visually checked.
- **#68 PV/nRT vs P for Ideal and Real Gases** — `…:813–845`, PDF p. 228 (printed p. 207). **Minor issue remains.** The CO₂ curve exits above the plot at 600 atm; enlarge the vertical range or adjust the plotted endpoint to match the stated data.

## Chapter 15 — Heat, Energy and Calorimetry

- **#69 Electrical Calorimetry Setup** — `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex:199–265`, PDF p. 235 (printed p. 214). **Pass after correction.** The heater and ammeter are in series, the voltmeter is parallel across the heater, and the thermometer bulb is below the sample surface. Rebuilt and visually checked.
- **#70 Method of Mixtures: Before and After** — `…:337–407`, PDF p. 237 (printed p. 216). **Pass after correction.** The after-mixing heat-balance statement and equation are split across short centered lines within the panel.
- **#71 Complete Heating Curve: Ice to Steam** — `…:535–573, 583–588`, PDF p. 239 (printed p. 218). **Pass after correction.** Segment lengths and labels now use the stated 1 kg sample and specific/latent heats; the curve and labels are legible. Rebuilt and visually checked.

## Chapter 16 — Heat Transfer

- **#72 Conduction: Molecular Vibration Chain in a Solid** — `chapters/part2_fluids_thermal/ch16_heat_transfer.tex:91–172`, PDF p. 248 (printed p. 227). **Pass.**
- **#73 Fourier’s Law: Heat Flow Through a Slab** — `…:239–286`, PDF p. 250 (printed p. 229). **Minor issue remains.** Route arrows clear of the “Hot/Cold side” labels and enlarge or simplify the tiny rotated gradient annotation.
- **#74 Natural Convection Loop in a Liquid** — `…:394–454`, PDF p. 252 (printed p. 231). **Minor issue remains.** Separate the overlapping “Cool fluid returns” and “Heat source” labels.
- **#75 Sea Breeze and Land Breeze** — `…:464–536`, PDF p. 252 (printed p. 231). **Pass.**
- **#76 Good and Poor Emitters/Absorbers of Radiation** — `…:555–641`, PDF p. 253 (printed p. 232). **Pass.**
- **#77 The Greenhouse Effect** — `…:791–925`, PDF p. 255 (printed p. 234). **Pass after correction.** The short-wave, outgoing IR, greenhouse-gas, and atmospheric-window callouts have separate positions. The faint region label that still appeared behind the callouts was removed; the final rebuilt page was visually checked.
- **#78 Thermos-Flask Cross-Section** — `…:984–1023`, PDF p. 256 (printed p. 235). **Pass; inventory title corrected.** The thermos figure is clear. The comparison of heat-transfer mechanisms is a table, not this TikZ figure.

## Chapter 17 — Wave Motion

- **#79 Transverse vs Longitudinal Waves** — `chapters/part3_waves_optics/ch17_wave_motion.tex:98–177`, PDF p. 266 (printed p. 245). **Minor issue remains.** Move the “Direction of energy travel” label clear of the transverse waveform.
- **#80 Wave Profile: Key Parameters Labelled** — `…:214–328`, PDF p. 267 (printed p. 246). **Pass.**
- **#81 Wave Reflection** — `…:397–438`, PDF p. 268 (printed p. 247). **Pass.**
- **#82 Diffraction Through a Gap** — `…:478–546`, PDF p. 269 (printed p. 248). **Pass after correction.** Headings no longer overlap, and gap-size labels were removed from the wavefronts. Rebuilt and visually checked.
- **#83 Constructive and Destructive Interference** — `…:583–642`, PDF p. 270 (printed p. 249). **Pass after correction.** The phase offset is now added after radian-to-degree conversion, giving exact antiphase. Rebuilt and visually checked.
- **#84 Standing Wave: Nodes and Antinodes** — `…:680–740`, PDF p. 271 (printed p. 250). **Pass after correction.** Explanatory text and the λ/2 and λ/4 dimensions are separated from the plotted extrema. Rebuilt and visually checked.
- **#85 Harmonics on a String Fixed at Both Ends** — `…:794–867`, PDF p. 272 (printed p. 251). **Pass after correction.** Trough markers now sit on the actual extrema, and the Node/Antinode key is stacked on separate lines. Rebuilt and visually checked.
- **#86 Harmonics in Open and Closed Pipes** — `…:903–1001`, PDF p. 273 (printed p. 252). **Pass after correction.** Pipe labels and harmonics fit within the panel at the reduced drawing scale; the n=3 closed-pipe node/antinode markers are correct.

These results cover the specified diagram inventory, not a complete editorial, pedagogical, physics, or permissions sign-off. The full book builds to 507 pages, but its TeX log still contains missing-character and layout warnings; the book should not be described as publication-certified.
