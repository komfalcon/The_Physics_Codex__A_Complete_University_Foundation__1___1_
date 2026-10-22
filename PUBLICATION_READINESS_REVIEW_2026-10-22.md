# Publication Readiness Review — 22 October 2026

## Completed in this branch

- Replaced the ISBN placeholder in `front_matter/copyright.tex` with the registered ISBN **978-978-67-2377-8**.
- Confirmed the ISBN-13 check digit is valid.
- Confirmed the foreword supplied in `front_matter/foreword.tex` is included in the active `book_main.tex` build, with its remaining location and date placeholders removed.
- Confirmed the active entry point is `book_main.tex`; `main.tex` is only a redirect and contains obsolete archived material after its redirect.
- Confirmed the active source tree contains the 29 planned chapters, the existing front matter, answers, bibliography, author photo, and both cover assets.

## Remaining publication decisions or checks

### 1. Foreword — publication permission check

The foreword now contains named contributor details and is included in the active build. Before printing, confirm the contributor's approval of the final wording, credentials, attribution, and permission to publish.

### 2. Back-cover ISBN barcode — completed, printer proof still recommended

The back-cover placeholder barcode was replaced in `back_cover.png` with an ISBN-13 barcode for **9789786723778**, together with the printed text **ISBN 978-978-67-2377-8**. The edited artwork was visually checked and the placeholder label is gone. The printer should still verify barcode scanability, quiet zone, contrast, and final reproduction at proof size.

### 3. Build and PDF inspection

The repository's documented baseline reports a 508-page A4 build including the full-bleed back cover, with known non-fatal TeX layout and glyph diagnostics. A release candidate still needs a fresh build using the command in `BUILDING.md`, followed by inspection of:

- the copyright page and ISBN rendering;
- the table of contents and list of figures;
- the final answer, bibliography, and back-cover pages;
- overfull boxes, missing-character diagnostics, and duplicate PDF destinations; and
- page count and final-page placement.

### 4. Copyright and publication metadata

The copyright page contains the author, publisher, Lagos location, contact details, first-edition year, and ISBN. Confirm these details with the publisher before release, especially the copyright year, publisher imprint, email address, telephone number, and rights wording.

### 5. Editorial and technical sign-off

The repository's own status notes correctly identify further work beyond diagram review. Before publication, obtain final sign-off for:

- physics accuracy and notation across all 29 chapters;
- answer-key completeness and numerical verification;
- citations and recommended-reading details;
- typography, line breaks, widows/orphans, and diagram legibility at print size;
- accessibility and image descriptions if an accessible edition is planned; and
- print specifications such as trim size, bleed, cover spine calculation, paper stock, and printer proof.

No additional ISBN placeholders were found in the active source tree after the copyright-page update.
