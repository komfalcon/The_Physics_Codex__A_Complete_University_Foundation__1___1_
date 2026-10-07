# Chapters 15–21: Fresh Diagram Re-audit (2026-10-07)
## Result and counts
- **Diagrams checked:** 36/36, inventoried from source and individually inspected in the rendered publication PDF.
- **Confirmed defects requiring edits:** 7. **Edited:** 7. **Post-edit visual checks:** 7/7; physical pp.255, 290, and 329 were additionally rechecked in the final integrated r5 PDF.
- **Accepted without mandatory edits:** 29.
- **Residual author judgment:** one non-blocking choice for Chapter 16 D6—whether to include solar albedo/reflection; see its row. The current diagram omits the unsupported reflection path.
## Build and scope
- The final integrated candidate is `/tmp/physics-codex-diagram-reaudit-final-r5/book_main.pdf`: **508 A4 pages**, SHA-256 `b8cef6c11222ec6a74e1ced0bc289473d0f7e4a18f15543f129b23b4c5bb2b92`, built from the shared re-audit branch after all accepted diagram patches were integrated. Page 508 is the back cover.
- In r5, the latest Ch16-D6 fix is confirmed on physical p.255 (printed p.234), and the previously corrected Ch18-18.4 and Ch21-D2 figures remain clear at pp.290 and 329. The other four edited figures retain their earlier post-edit visual checks; no new issue was reported in r5.
- The r5 final log has no fatal TeX errors or unresolved references/citations. Whole-book warnings remain: 11 missing-semicolon glyph notices, 177 overfull hboxes, 14 underfull hboxes, 2 overfull vboxes, and 1 duplicate PDF destination. These are not all attributable to this range.
- The isolated builds listed in earlier audit history are retained as evidence for the focused edits; the shared branch now contains those changes. One optional author choice remains for Ch16-D6—whether to include solar albedo/reflection; see its row. The current diagram omits the unsupported reflection path.
- Source ranges below are the current one-based inclusive lines of each complete `tikzpicture` block in the stated file. PDF locations give physical PDF page index and printed book page. All 36 counted visuals are TikZ diagrams; explanatory tables were not counted.
## Seven edited figure IDs
| Figure | Current source range | Verified change |
|---|---|---|
| Ch16-D6 | `chapters/part2_fluids_thermal/ch16_heat_transfer.tex:794–908` | **Updated; PASS in final integrated r5.** The shortened “Back radiation” label sits beside the downward red ray, clear of both red paths; no ray crosses the text and the gold short-wave path is unobstructed. **Residual author decision:** whether this schematic should also depict solar albedo. The source does not identify a reflector; if albedo is wanted, specify surface or cloud reflection and label it separately from greenhouse-gas IR absorption. |
| Ch17-D5 | `chapters/part3_waves_optics/ch17_wave_motion.tex:587–635` | **Edited; final PDF page visually rechecked.** Put both component waves on a common equilibrium baseline and plotted their literal sum: constructive resultant amplitude 2A; equal-amplitude antiphase resultant zero. No residual science decision. |
| Ch18-18.4 | `chapters/part3_waves_optics/ch18_sound_waves.tex:783–848` | **Edited; final PDF page visually rechecked.** Replaced the step-shaped display with an amplitude-versus-time A-scan baseline and two time-ordered echo peaks; moved the time label fully inside the screen. No residual science decision. |
| Ch19-F19.1 | `chapters/part3_waves_optics/ch19_light_reflection.tex:91–141` | **Edited; final PDF page visually rechecked.** Adjusted both angle arcs to the ray geometry, measured equally from the normal. No residual science decision. |
| Ch20-F5 | `chapters/part3_waves_optics/ch20_light_refraction_optical_instruments.tex:888–959` | **Edited; final PDF page visually rechecked.** Rebuilt as a matched *uncorrected* parallel-ray comparison: myopia focuses before the retina; hypermetropia behind it. Captions sit outside the eye outlines, and the figure no longer implies an undrawn corrective lens. The correction table immediately following gives diverging/concave correction for myopia and converging/convex correction for hypermetropia; no residual science decision. |
| Ch21-D1 | `chapters/part4_electricity_magnetism/ch21_electrostatics.tex:105–159` | **Edited; final PDF page visually rechecked.** Removed the misleading dashed gold overlay from the force-only attraction/repulsion schematic; the arrows now show only forces. No residual science decision. |
| Ch21-D2 | `chapters/part4_electricity_magnetism/ch21_electrostatics.tex:189–323` | **Updated; PASS in final integrated r5.** Qualified friction transfer, raised/shifted the contact spheres, shortened the arrow, and placed “separate” below the contact row. Repositioned/reflowed the induction labels and caption. The full p.329 page and close detail crop show no overlap among the heading, spheres, Step 3 label, conductor/switch, open-ground note, Earth mark, or caption. No residual science decision. |

## Figure-by-figure checklist

### Chapter 15 — Heat Energy and Calorimetry

Source: `chapters/part2_fluids_thermal/ch15_heat_energy_calorimetry.tex`. 3 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch15-F1 | Electrical method for measuring specific heat capacity: insulated calorimeter, heater, thermometer, voltmeter, ammeter, and supply. | `199–261` | PDF 235 (printed 214) | **Accepted as-is; no verified defect.** Optional/non-blocking: an explicit switch or a note that calorimeter and heater heat capacities are neglected would add context; neither omission makes the present visual incorrect because the process box states the no-loss assumption. |
| Ch15-F2 | Method of mixtures, shown before and after adding a hot solid to cold water in a calorimeter. | `335–401` | PDF 237 (printed 216) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: If revised for maximum beginner clarity, enlarge or reposition the compact blue equation in the after-mixing panel and explicitly draw/label a lid or insulation boundary; these are readability/pedagogy refinements, not verified defects. |
| Ch15-F3 | Complete heating curve for 1 kg of water from −20 °C ice to 120 °C steam, including sensible-heating slopes and fusion/vaporisation plateaux. | `527–580` | PDF 239 (printed 218) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: For a future edition, state ‘at approximately 1 atm’ directly in the figure caption and use a slightly larger font for the small interval labels; these would make the limiting assumption and print readability stronger but do not establish a current scientific error. |

### Chapter 16 — Heat Transfer

Source: `chapters/part2_fluids_thermal/ch16_heat_transfer.tex`. 7 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch16-D1 | Molecular vibration chain explaining conduction in a solid | `93–165` | PDF 248 (printed 227) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: If the pedagogical goal is specifically metal conduction, an optional future revision could add a distinct electron-energy/particle cue, but its omission is not a defect in this molecular-mechanism visual. |
| Ch16-D2 | Fourier-law heat flow through a slab | `241–285` | PDF 250 (printed 229) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: The equation is a scalar heat-flow magnitude; if a signed flux convention is later desired, state that separately rather than changing this diagram. |
| Ch16-D3 | Natural convection loop in a heated liquid | `397–453` | PDF 252 (printed 231) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: For a more advanced treatment, one could mark that the circulation is driven by buoyancy and pressure differences, but the current introductory visual is scientifically adequate. |
| Ch16-D4 | Daytime sea breeze and nighttime land breeze | `467–530` | PDF 252 (printed 231) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: The phrase about morning/afternoon navigation is a simplified practical summary, not a diagram error; if regional timing precision is important, qualify it as typically overnight/early morning versus afternoon. |
| Ch16-D5 | Good/poor emitters and absorbers; Kirchhoff relation | `558–640` | PDF 253 (printed 232) | **Accepted as-is; no verified defect.** The introductory contrast is adequate. If later coverage treats selective emitters/absorbers, qualify the black-versus-polished comparison as wavelength/spectral- and temperature-dependent rather than treating color alone as universal. |
| Ch16-D6 | Solar short-wave input; terrestrial IR absorption/re-emission, back radiation, and atmospheric window (optional albedo path omitted pending author choice) | `794–908` | PDF 255 (printed 234) | **Updated and PASS in the final isolated p.255 follow-up.** The two-line “Back radiation” label sits beside the downward red back-radiation arrow, with clear separation from both red shafts; no ray crosses the text and the gold short-wave path is unobstructed in the 300-dpi render/crop. The disconnected reflected-shortwave arrow remains removed. **Residual author decision:** whether this schematic should also depict solar albedo. The source does not identify a reflector; if albedo is wanted, specify surface or cloud reflection and label it separately from greenhouse-gas IR absorption. |
| Ch16-D7 | Vacuum flask design features suppressing conduction, convection, and radiation | `969–1007` | PDF 256 (printed 235) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: A minor optional enhancement would label which wall surfaces are silvered, but the existing ‘Silvered walls’ callout plus the solution is sufficient. |

### Chapter 17 — Wave Motion

Source: `chapters/part3_waves_optics/ch17_wave_motion.tex`. 8 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch17-D1 | Transverse versus longitudinal waves | `100–175` | PDF 266 (printed 245) | **Accepted as-is; no residual issue identified.** |
| Ch17-D2 | Wave profile: crest, trough, amplitude, wavelength, period and wave equation | `216–326` | PDF 267 (printed 246) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: If maximum pedagogical precision is desired, label the lower quantity as ‘displacement = −A’ rather than only ‘−A’, but this is not a verified defect. |
| Ch17-D3 | Law of reflection | `399–436` | PDF 268 (printed 247) | **Accepted as-is; no residual issue identified.** |
| Ch17-D4 | Diffraction through wide and narrow gaps | `480–546` | PDF 269 (printed 248) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: For a more quantitative teaching graphic, add a visible wavelength marker or state explicitly that the two panels use the same λ while d changes; this is an optional improvement, not a verified error. |
| Ch17-D5 | Constructive and destructive interference | `587–635` | PDF 270 (printed 249) | **Edited; final PDF page visually rechecked.** Put both component waves on a common equilibrium baseline and plotted their literal sum: constructive resultant amplitude 2A; equal-amplitude antiphase resultant zero. No residual science decision. |
| Ch17-D6 | Standing-wave nodes, antinodes and separations | `677–729` | PDF 271 (printed 250) | **Accepted as-is; no residual issue identified.** |
| Ch17-D7 | First three harmonics of a string fixed at both ends | `787–856` | PDF 272 (printed 251) | **Accepted as-is; no residual issue identified.** |
| Ch17-D8 | Displacement patterns in open and closed pipes | `896–992` | PDF 273 (printed 252) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: An optional improvement would be to label ‘displacement’ versus ‘pressure’ directly beside the pipe panels, but the surrounding prose already states the convention. |

### Chapter 18 — Sound Waves

Source: `chapters/part3_waves_optics/ch18_sound_waves.tex`. 4 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch18-18.1 | Tuning fork producing a longitudinal sound wave: alternating compressions/rarefactions and pressure variation with distance | `76–180` | PDF 282 (printed 261) | **Accepted as-is; no verified defect.** Optional/non-blocking: small back-and-forth particle-displacement arrows or a note that the dots are an instantaneous snapshot could strengthen the motion cue without changing the physics. |
| Ch18-18.2 | Pitch, loudness, and timbre represented by waveforms | `307–377` | PDF 284 (printed 263) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: For maximum rigor, the horizontal axis could be labeled time on all three panels (currently only the quality panel visibly labels Time), but this is a clarity enhancement, not a verified defect. |
| Ch18-18.3 | Doppler effect from a source moving toward the right: compressed fronts ahead and expanded fronts behind | `555–592` | PDF 287 (printed 266) | **Accepted as-is; no verified defect.** No residual issue; the straight cross-sectional fronts are explicitly labeled schematic and are an appropriate abstraction. |
| Ch18-18.4 | Pulse-echo medical ultrasound: transducer, tissue boundaries, echo travel times, depth calculation, and display output | `783–848` | PDF 290 (printed 269) | **Edited; final PDF page visually rechecked.** Replaced the step-shaped display with an amplitude-versus-time A-scan baseline and two time-ordered echo peaks; moved the time label fully inside the screen. No residual science decision. |

### Chapter 19 — Reflection of Light

Source: `chapters/part3_waves_optics/ch19_light_reflection.tex`. 4 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch19-F19.1 | Law of reflection at a plane surface: incident ray, reflected ray, normal, and equal angles | `91–141` | PDF 296 (printed 275) | **Edited; final PDF page visually rechecked.** Adjusted both angle arcs to the ray geometry, measured equally from the normal. No residual science decision. |
| Ch19-F19.2 | Plane-mirror virtual image formation, equal object/image distance, and backward ray extensions | `175–222` | PDF 297 (printed 276) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: If a future pedagogical revision is desired, a brief explicit note that the lower image endpoint is the reflected image of the object base could remove a minor possible ambiguity, but this is not a verified defect. |
| Ch19-F19.3 | Concave versus convex spherical-mirror geometry, pole P, centre C, focus F, R=2f, and virtual focus | `287–358` | PDF 298 (printed 277) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: Preserve the paraxial context implied by the nearly axial rays; if expanded in a later edition, explicitly state that the focus relation is paraxial/approximate for spherical mirrors, but the current diagram is not wrong in context. |
| Ch19-F19.4 | Concave-mirror ray diagram for an object beyond C: real, inverted, diminished image between C and F | `386–423` | PDF 298 (printed 277) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: For maximum instructional precision, extend the first reflected ray visually all the way to the image tip or add a tiny intersection marker at the image point; the existing line already passes through the image point, so this is optional presentation refinement, not a defect. |

### Chapter 20 — Refraction and Optical Instruments

Source: `chapters/part3_waves_optics/ch20_light_refraction_optical_instruments.tex`. 5 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch20-F1 | Refraction at a glass–air boundary and Snell's law | `94–156` | PDF 310 (printed 289) | **Accepted as-is; no verified defect.** Optional/non-blocking: reduce or reposition the right-side explanatory annotations if a less crowded composition is desired; this is not a scientific defect. |
| Ch20-F2 | Total internal reflection: below critical angle, at critical angle, and above critical angle | `291–378` | PDF 312 (printed 291) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: If revised for maximum beginner clarity, add an explicit arrowhead or a crossed-out symbol to the faint dashed 'no refraction' placeholder in case 3 so it cannot be mistaken for a physical transmitted ray; the existing label and dashed styling already make the intended meaning clear. |
| Ch20-F3 | Converging (convex) and diverging (concave) lenses | `458–559` | PDF 313 (printed 292) | **Accepted as-is; no verified defect.** No residual issue; the diagram is explicitly schematic and does not need scale correction. |
| Ch20-F4 | Compound microscope ray diagram: objective, intermediate image, eyepiece, and virtual final image | `758–815` | PDF 317 (printed 296) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: For a future pedagogical refinement, move the intermediate-image label slightly farther from the eyepiece rays; this is a readability/composition option, not a correctness issue. |
| Ch20-F5 | Uncorrected myopia and hypermetropia: focus of distant parallel rays relative to the retina | `888–959` | PDF 318 (printed 297) | **Edited; final PDF page visually rechecked.** Rebuilt as a matched *uncorrected* parallel-ray comparison: myopia focuses before the retina; hypermetropia behind it. Captions sit outside the eye outlines, and the figure no longer implies an undrawn corrective lens. The correction table immediately following gives diverging/concave correction for myopia and converging/convex correction for hypermetropia; no residual science decision. |

### Chapter 21 — Electrostatics

Source: `chapters/part4_electricity_magnetism/ch21_electrostatics.tex`. 5 diagrams.

| Figure | Diagram / teaching point | Source lines | Final PDF page | Disposition, residual ambiguity, or recommendation |
|---|---|---:|---:|---|
| Ch21-D1 | Attraction and repulsion of unlike and like charges | `105–159` | PDF 328 (printed 307) | **Edited; final PDF page visually rechecked.** Removed the misleading dashed gold overlay from the force-only attraction/repulsion schematic; the arrows now show only forces. No residual science decision. |
| Ch21-D2 | Charging by friction, contact, and induction | `189–320` | PDF 329 (printed 308) | **Edited; final PDF page visually rechecked.** Qualified friction transfer as material-pair dependent and spaced/wrapped the induction sequence: bring the positive rod near, ground the conductor, disconnect ground while the rod remains, then remove the rod. The four-step induction strip remains compact, but its labels are separated and readable in the final render; enlarging/splitting it is optional if a later layout allows more prominence. No residual science decision. |
| Ch21-D3 | Electric-field patterns for a positive charge, negative charge, dipole, and parallel plates | `518–604` | PDF 332 (printed 311) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: If desired in a future refinement, label the dipole subpanel explicitly as “idealized field lines” and keep the plate-edge idealization understood as the interior-region approximation; neither is necessary for this audit. |
| Ch21-D4 | Radial electric field lines and concentric equipotential lines around a positive point charge | `692–728` | PDF 333 (printed 312) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: The labels are relatively small in print, but they remain readable in the rendered page and this is a readability observation, not a verified defect. |
| Ch21-D5 | Gold-leaf electroscope: uncharged versus charged leaves | `794–866` | PDF 335 (printed 314) | **Accepted as-is; no verified defect.** Optional/non-blocking refinement: A possible pedagogical enhancement would be to add a small note that sign testing requires a known reference charge, but that belongs to the accompanying explanation rather than being necessary to correct the diagram. |

## Notes for editorial follow-up
- The single outstanding choice is whether the greenhouse-effect teaching visual should also depict solar albedo. The current source establishes transmission of incoming short-wave radiation and greenhouse-gas absorption/re-emission of long-wave IR, but does not identify what reflects the optional short-wave ray. Keeping that path omitted avoids guessing; add it only if the author specifies a surface or cloud reflector.
- Optional refinements recorded in the table (such as stating the approximate 1-atm assumption on the water heating curve, adding a wavelength marker to the diffraction comparison, or labeling pipe displacement versus pressure) are not verified defects and are not blockers.


## Focused three-page follow-up — final isolated candidate (2026-10-07)
This follow-up supersedes the earlier Ch21-D2 print-clearance note and records the current dispositions for all three requested figures. Final isolated build: `/tmp/physics-codex-three-fixes/build/book_main.pdf` (508 pages, A4; SHA-256 `1f0fb8039fda190cf99e7c9200149827aa9ce753b5512808f6f18810fa69a606`). Each page was rendered at 300 dpi (2481 × 3508 px); p.329 was also reviewed as a complete figure-panel crop and a close detail crop.

| PDF page (printed page) | Figure | Final disposition |
|---|---|---|
| 255 (234) | Ch16-D6 | **UPDATED; PASS in the final p.255 follow-up.** Shortened the label to “Back radiation” and placed it immediately right of the downward red ray. The 300-dpi detail crop shows clear separation from the adjacent upward red path; no ray crosses the text. |
| 290 (269) | Ch18-18.4 | **PASS.** “A-scan display” and the two-line “amplitude vs time” subtitle remain fully inside the black display panel. |
| 329 (308) | Ch21-D2 | **PASS.** The contact-row spheres and arrow are separated; “separate” sits below the contact row in the intervening white space. The induction heading, Step 3 caption, conductor/switch, open-ground note, Earth mark, and explanatory caption are distinct in both the full-page and close crops. |

The integration patch contains only the three requested chapter source files and passes `git apply --check` against the shared worktree. The shared worktree itself was not modified.
