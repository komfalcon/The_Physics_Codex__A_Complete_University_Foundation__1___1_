# Continuation Prompt — Physics Codex Diagram Review from Batch 3

## Role

You are continuing an active repository task as a senior physics textbook editor, scientific illustrator, LaTeX/TikZ engineer, and publication-quality reviewer.

Do not assume that the diagrams are already publication-ready. Your job is to review them individually for:

1. **Scientific accuracy** — geometry, equations, arrows, vector directions, graph relationships, units, conventions, and physical interpretation.
2. **Label accuracy** — every label must refer to the correct object, quantity, direction, axis, point, or construction line.
3. **Readability** — labels must remain legible at normal printed-book size and must not overlap lines, arrows, axes, legends, or other labels.
4. **Pedagogical clarity** — a first-year university or advanced secondary-school student should understand what the figure demonstrates without guessing.
5. **TikZ/PGFPlots geometry** — no clipped annotations, escaped markers, incorrect scopes, bad bounding boxes, misleading scales, or overflow outside a panel/page.

Use conservative, minimal source changes. Do not rewrite unrelated prose or alter global layout merely to hide local diagram problems.

## Repository and current state

Repository:

```text
komfalcon/The_Physics_Codex__A_Complete_University_Foundation__1___1_
```

Working directory in the Sandbox:

```text
/home/ubuntu/The_Physics_Codex__A_Complete_University_Foundation__1___1_
```

The previous pull request containing the earlier batches has already been merged. Do **not** continue on the old branch and do **not** create another commit on the merged pull request.

Start from the current remote `main` branch:

```bash
cd /home/ubuntu/The_Physics_Codex__A_Complete_University_Foundation__1___1_
git fetch origin --prune
git switch main
git pull --ff-only origin main
git switch -c audit-diagrams-batch3
```

If the local checkout is not available, clone the repository first with:

```bash
gh repo clone komfalcon/The_Physics_Codex__A_Complete_University_Foundation__1___1_
```

The next AI must create a **new pull request** from `audit-diagrams-batch3` into `main`. Use a focused title such as:

```text
Review and repair diagrams batch 3
```

Do not reuse the old pull-request number or old branch. Verify the new branch and clean status before editing:

```bash
git status --short --branch
git log -3 --oneline
```

The repository is currently clean after the pushed Batch 2 commit. Verify with:

```bash
cd /home/ubuntu/The_Physics_Codex__A_Complete_University_Foundation__1___1_
git status --short --branch
git log -3 --oneline
```

Do not reset, rebase, force-push, or discard the existing Batch 1 or Batch 2 work.

## Completed work

### Batch 1 — diagrams 1–10

Report:

```text
BATCH1_DIAGRAM_REVIEW.md
```

Commit:

```text
1616e20 Review and repair diagrams batch 1
```

Important fixes included:

- Corrected the Vernier calliper geometry so 10 vernier divisions represent 9 mm as stated.
- Clarified the chapter’s “parallel” versus “anti-parallel” convention.
- Corrected the vector-representation scale and added units to the 4 N label.
- Removed a redundant zero-length segment from the polygon-rule diagram.
- Corrected a dedication typography typo.

### Batch 2 — diagrams 11–20

Report:

```text
BATCH2_DIAGRAM_REVIEW.md
```

Commit:

```text
3bfcc99 Review and repair diagrams batch 2
```

Important fixes included:

- Corrected the left cable in the equilibrium example to actually be 30° from the vertical.
- Replaced a misleading in-page arrow in the right-hand-rule diagram with the standard circled-dot “out of page” convention.
- Corrected the cyclic cross-product caption to match the displayed positive cycle.

### Master inventory

Report:

```text
DIAGRAM_AUDIT_THROUGH_PRINTED_PAGE_246.md
```

This contains 86 TikZ blocks across the included front matter and Chapters 1–17. Entries 1–20 are marked `REVIEWED`. Entries 21–86 remain to be individually reviewed.

The master report is an inventory and progress record, **not** a blanket publication certification.

## Start here: Batch 3, items 21–30

Review exactly these ten inventory entries next:

| # | Source file | Lines | Diagram |
|---:|---|---:|---|
| 21 | `chapters/part1_mechanics/ch03_kinematics.tex` | 593–639 | Projectile Motion Trajectory |
| 22 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 363–398 | Connected Bodies and Pulleys |
| 23 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 434–469 | Forces on an Inclined Plane |
| 24 | `chapters/part1_mechanics/ch04_newtons_laws_dynamics.tex` | 597–628 | Velocity-Time Graph for Terminal Velocity |
| 25 | `chapters/part1_mechanics/ch05_work_energy_power.tex` | 65–96 | Work Done at an Angle |
| 26 | `chapters/part1_mechanics/ch05_work_energy_power.tex` | 329–349 | Work Done by a Spring Force |
| 27 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 121–154 | Angular and Linear Quantities |
| 28 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 248–278 | Centripetal Acceleration and Force |
| 29 | `chapters/part1_mechanics/ch06_circular_motion.tex` | 406–439 | Vertical Circle — Forces at Key Points |
| 30 | `chapters/part1_mechanics/ch07_simple_harmonic_motion.tex` | 144–198 | SHM Graphs — Displacement, Velocity, Acceleration |

Do not move to item 31 until items 21–30 have review entries and the batch report is complete.

## Required workflow for each batch

### 1. Inspect source and context

For each diagram:

- Read the entire TikZ/PGFPlots block, not only the `\begin{tikzpicture}` line.
- Read the surrounding explanatory text, equations, worked example, and definitions.
- Check whether the diagram’s labels agree with the text and calculations.
- Check coordinate values, slopes, angles, units, and arrow directions mathematically.
- Look for common errors:
  - A label says one angle or value while the coordinates draw another.
  - A force or velocity arrow points in the wrong direction.
  - A graph’s curve contradicts its legend or caption.
  - A spring, pulley, circular-motion, or projectile diagram violates the stated model.
  - A vector is drawn with inconsistent magnitude or scale.
  - A quantity lacks units or uses an ambiguous symbol.
  - A label is technically true but too vague for a learner.
  - A line, arrow, marker, legend, or annotation is clipped or overlaps another element.
  - A coordinate is defined outside a transformed TikZ scope.
  - PGFPlots axes, domains, ticks, or shaded regions do not match the physics.

### 2. Make a verdict

Use one of:

- `PASS` — scientifically accurate, readable, and no justified source change needed.
- `NEEDS FIX` — a definite scientific, labeling, readability, or geometry defect exists and should be fixed now.
- `REVIEW` — a potential issue needs a clearer visual or physics check before deciding; do not silently guess.

### 3. Apply minimal fixes

Preferred techniques:

- Correct the local coordinate or endpoint rather than changing global scale.
- Define named coordinates inside the scope that applies scaling or transformations.
- Use explicit `\path[use as bounding box]` or safe margins for annotations.
- Derive labels and geometry from shared macros where a numeric relationship matters.
- Add units and clarifying words when the symbol alone is ambiguous.
- Use `anchor`, `xshift`, and `yshift` for local label placement.
- Keep labels large enough for print; do not use tiny fonts to conceal crowding.
- Avoid global `\sloppy`, `\hfuzz`, layout changes, or unrelated prose edits.

### 4. Compile and render

Use a clean build:

```bash
cd /home/ubuntu/The_Physics_Codex__A_Complete_University_Foundation__1___1_
rm -f book_main.aux book_main.log book_main.out book_main.toc book_main.lof \
      book_main.idx book_main.ilg book_main.ind book_main.pdf \
      book_main.fdb_latexmk book_main.fls
latexmk -pdf -interaction=nonstopmode -file-line-error -halt-on-error book_main.tex
pdfinfo book_main.pdf | grep -E 'Pages|Page size'
```

The expected page count is currently **513 pages**, but record any intentional change.

Find the PDF pages containing each diagram using `pdftotext -f N -l N -layout` and distinctive nearby text, then render the affected pages at print-review resolution:

```bash
mkdir -p /tmp/batch3-renders
pdftoppm -f PAGE -l PAGE -png -r 120 -singlefile book_main.pdf /tmp/batch3-renders/page-PAGE
```

Inspect the page containing each changed diagram plus one adjacent page where possible. Do not rely on compilation success alone.

### 5. Record the batch

Create:

```text
BATCH3_DIAGRAM_REVIEW.md
```

It must contain, for all ten items:

- Item number.
- Source file and line range.
- Diagram name.
- Scientific verdict.
- Specific issue, if any.
- Exact fix made, if any.
- Visual/readability result.
- PDF page inspected when known.
- Any unresolved uncertainty.

Use the same style as `BATCH1_DIAGRAM_REVIEW.md` and `BATCH2_DIAGRAM_REVIEW.md`.

Update `DIAGRAM_AUDIT_THROUGH_PRINTED_PAGE_246.md` so entries 21–30 say:

```text
REVIEWED — see BATCH3_DIAGRAM_REVIEW.md
```

Do not mark an item `REVIEWED` merely because it compiled. It must have an explicit scientific/readability outcome.

### 6. Commit and push

Remove generated build artifacts before committing:

```bash
rm -f book_main.aux book_main.fdb_latexmk book_main.fls book_main.lof \
      book_main.log book_main.out book_main.pdf book_main.toc \
      book_main.idx book_main.ilg book_main.ind
```

Review the diff carefully:

```bash
git status --short
git diff --check
git diff --stat
git diff
```

Commit only the batch source fixes, the batch report, and the updated master audit:

```bash
git add <changed-source-files> BATCH3_DIAGRAM_REVIEW.md \
        DIAGRAM_AUDIT_THROUGH_PRINTED_PAGE_246.md
git commit -m "Review and repair diagrams batch 3"
git push
```

Do not merge the new pull request automatically. Leave the work on the new Batch 3 branch and new PR for the user to review.

## Build-warning policy

The repository currently has pre-existing unresolved references, including references such as:

```text
tab:si_base
tab:prefixes
tab:instruments
sec:unit_vectors
sec:position_vectors
sec:component_method
tab:densities
tab:viscosity
tab:expansion
```

Do not claim a perfect build if those remain. Record them as pre-existing reference-integrity work unless a diagram change introduces a new warning. The diagram batches are not permission to silently repair unrelated table/reference problems.

## Important truthfulness rule

Do not tell the user that all diagrams are publication-perfect after completing a batch. State exactly:

- how many diagrams were individually reviewed;
- which ones passed;
- which ones were changed;
- which issues remain uncertain;
- whether the book compiled;
- what warnings remain;
- how many diagrams are still unreviewed.

After Batch 3, the correct progress count should be **30 of 86 individually reviewed**, assuming all ten items are completed and recorded. The new PR should contain only the Batch 3 changes and reports on top of the already-merged `main`.

## Continuation after Batch 3

Proceed in batches of ten using the master inventory:

- Batch 4: items 31–40.
- Batch 5: items 41–50.
- Batch 6: items 51–60.
- Batch 7: items 61–70.
- Batch 8: items 71–80.
- Batch 9: items 81–86 (six remaining items).

For every batch, preserve the same standards and report structure. Scientific accuracy and reader comprehension take priority over simply making the PDF compile.
