# The Physics Codex

**The Physics Codex: A Complete University Foundation** is a LaTeX physics textbook project for Nigerian senior-secondary learners preparing for UTME and students beginning university physics. It builds concepts from the foundations and includes worked examples, exercises, diagrams, and an answer resource.

## Contents

The manuscript comprises 29 chapters in five parts:

1. **Mechanics** — Chapters 1–10
2. **Fluids and Thermal Physics** — Chapters 11–16
3. **Waves and Optics** — Chapters 17–20
4. **Electricity and Magnetism** — Chapters 21–26
5. **Modern Physics** — Chapters 27–29

The source tree also contains front matter, back matter, true-PNG front and back cover assets, an author-image asset, and diagram-review notes. `book_main.tex` places both covers in the product build.

## Build

Use `book_main.tex` from the repository root. See [BUILDING.md](BUILDING.md) for the tested `latexmk` command, toolchain notes, and current validation status. Build artifacts should be directed outside the source checkout.

## Publication status

This repository is an in-progress manuscript. The fresh 139-item diagram re-audit is complete, with 65 instructional figures corrected and checked after editing. The current 508-page A4 build succeeds, but retains TeX layout/glyph warnings; broader physics, citation, and pedagogical sign-offs and final publication decisions remain unfinished. Do not treat the current sources or PDF as a publication-certified edition. ISBN and other final publication metadata must be supplied by the author or publisher.
