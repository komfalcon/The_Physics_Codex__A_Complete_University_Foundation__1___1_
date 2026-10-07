# The Physics Codex — Chapter 24–29 diagram review

## Summary

All 26 active TikZ diagrams in Chapters 24–29 were checked against source and rendered PDF; source counts matched in every chapter. Following the forced 507-page build, nine diagrams pass, including the corrected Chapter 25 Fleming, charged-particle orbit and DC motor figures, plus the Chapter 29 p–n junction diagram. Seventeen findings remain: 15 medium issues and 2 low layout issues; this is not a publication sign-off.

Page locators below are PDF pages. Source lines refer to the current chapter files at review time.

## Chapter 24 — Electrical Energy and Power

- **High Voltage Transmission: Reducing Power Loss** — line 357, PDF p. 378. **Medium.** Grid and transformer labels collide; the local 11 kV label is crowded; the power station is disconnected from the step-up transformer. Reposition or shorten labels and add a connector between the station and transformer.
- **Transformer Construction and Action** — line 486, PDF p. 379. **Medium.** Both flux arrows point downward, failing to show consistent closed circulation, and the flux label is too close to the equation. Reverse the lower arrow or draw a closed-loop path, and move the label clear.

## Chapter 25 — Magnetism and Electromagnetism

- **Magnetic Field Patterns (bar magnet and unlike poles)** — line 93, PDF p. 390. **Pass.** No issue found.
- **Magnetic Fields Around Current-Carrying Conductors** — line 182, PDF p. 390. **Pass.** No issue found.
- **Fleming’s Left-Hand Rule** — line 387, PDF p. 392. **Pass after correction.** The final diagram shows magnetic field left, conventional current into the page, and force upward; the labels are legible. The 507-page PDF was visually checked at print-page scale.
- **Circular Motion of a Charged Particle in a Magnetic Field** — line 546, PDF p. 394. **Pass after correction.** The field now points out of the page, consistent with the positive charge’s clockwise orbit and inward Lorentz force; the force label is separated from the radius annotation. Rebuilt and visually checked.
- **DC Motor schematic** — line 704, PDF p. 396. **Pass after correction.** With the field from N to S and the shown opposed coil currents, the left and right forces are now marked out of and into the page, respectively, producing the displayed motor torque. Rebuilt and visually checked.

## Chapter 26 — Electromagnetic Induction

- **Faraday’s Induction Experiments** — line 73, PDF p. 404. **Pass.** No issue found.
- **Lenz’s Law: Direction of Induced Current** — line 278, PDF p. 406. **Medium.** The “Current…” and “Creates B field…” annotations overlap above both coils. Separate them or reflow them as aligned two-line labels.
- **Motional EMF: Conductor Moving in a Field** — line 428, PDF p. 407. **Medium.** The external-circuit current arrow points from negative to positive; conventional current should flow from the positive end down the external rail. Reverse the rail arrow, clarify the prose, and move the rod-length label clear of the rod and field.
- **AC Generator: Construction and Output** — line 645, PDF p. 409. **Medium.** The axle runs through the title, while graph phase annotations crowd the curve and tick labels. Move the title clear and enlarge or reposition the phase annotations.
- **Eddy Currents in a Solid vs Laminated Core** — line 827, PDF p. 411. **Pass.** No issue found.

## Chapter 27 — Atomic Structure and Spectra

- **Rutherford’s Gold Foil Experiment** — line 120, PDF p. 420. **Low.** The “Nucleus” label obscures the central beam/foil area, and nearby detector annotations are crowded. Offset the label with a leader and move the others away from ray paths.
- **Energy Level Diagram of Hydrogen and Spectral Series** — line 297, PDF p. 422. **Medium.** Energy-value labels collide with the Balmer/Paschen annotations. Give values and series labels separate space, using leader lines or more spacing.
- **Emission and Absorption Spectra Compared** — line 435, PDF p. 423. **Medium.** The 410 nm and 434 nm labels overlap; white gaps also make the “continuous” spectrum appear segmented. Stagger the labels and close the gaps, or identify the drawing as schematic.
- **Photoelectric Effect: Experimental Setup and Graph** — line 603, PDF p. 425. **Medium.** The f₀ tick is at x=5, while the threshold point is at x=3. Align f₀ with the threshold point and move “Metal cathode” clear of the tube and wire.

## Chapter 28 — Radioactivity and Nuclear Physics

- **Alpha, Beta and Gamma in Electric and Magnetic Fields** — line 181, PDF p. 435. **Pass.** No issue found.
- **Radioactive Decay Curve and Half-Lives** — line 456, PDF p. 438. **Low.** The N₀ label is clipped at the plot’s top edge. Move it below or to the right of the initial point, or add plot margin.
- **Binding Energy per Nucleon vs Mass Number** — line 677, PDF p. 441. **Medium.** The fusion annotation is clipped at the left plot boundary. Move it inside the axes or shorten and reflow it.
- **Pressurised Water Reactor (PWR)** — line 866, PDF p. 443. **Medium.** The return-water arrow points toward the turbine rather than back to the heat exchanger, and some callouts crowd flow lines. Redraw and label the return path in the correct direction; move callouts clear of the lines.

## Chapter 29 — Electronics

- **n-type and p-type Silicon Crystals** — line 141, PDF p. 450. **Medium.** The two headings run together. Increase their horizontal separation or shorten/reposition them.
- **p-n Junction Diode: Forward and Reverse Bias** — line 271, PDF p. 451. **Pass after correction.** Forward conventional current now flows from battery positive through the p-side, junction and n-side to the negative terminal; reverse leakage is shown in the opposite direction across the junction. The 507-page rebuild was visually checked at print-page scale.
- **Semiconductor Diode Symbol (Anode/Cathode labels)** — line 389, PDF p. 452. **Medium.** The Anode and Cathode labels overlap beneath the symbol. Move them apart and align each with its terminal.
- **Half-Wave and Full-Wave Rectification Circuits and Waveforms** — line 432, PDF p. 452. **Medium.** The bridge does not use recognizable diode symbols, and its DC output is left open despite the described load. Draw four standard diodes and connect the output to a labelled load resistor; optionally show the smoothing capacitor.
- **n-p-n Transistor as Switch and Amplifier** — line 648, PDF p. 454. **Medium.** Both panel titles collide with the +VCC labels. Move the headings or supply labels to provide clear separation.
- **Op-Amp Configurations** — line 876, PDF p. 456. **Medium.** The Rf labels overlap both amplifier titles. Move the labels beside or below their feedback resistors, clear of the headings.

## Review status

The Fleming, charged-particle, DC motor, and p–n junction fixes were rebuilt and visually checked. No high-severity diagram issues remain in this range, but 15 medium and 2 low findings are still listed above. The broader book build still has missing-glyph and layout diagnostics; these changes are not a publication certification.
