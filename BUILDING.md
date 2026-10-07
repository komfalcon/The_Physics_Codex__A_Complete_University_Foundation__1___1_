# Building The Physics Codex

## Active source and output

Build from the repository root using `book_main.tex`. `main.tex` redirects to that entrypoint but also retains obsolete material, so it should not be treated as a separate manuscript source. Bibliography data is embedded directly in the TeX sources; the active entrypoint does not require BibTeX, Biber, or MakeIndex.

The source uses pdfLaTeX and packages including AMS math, geometry, graphics, xcolor, mdframed, tcolorbox, TikZ/PGFPlots, enumitem, fancyhdr, booktabs, longtable, siunitx, epigraph, wrapfig, lettrine, newunicodechar, and Latin Modern fonts. Install a TeX Live distribution that provides these packages, plus `latexmk`.

## Build command

Run this from the repository root to keep auxiliary files and the PDF outside the checkout:

```sh
OUTDIR="${TMPDIR:-/tmp}/physics-codex-build"
mkdir -p "$OUTDIR"
latexmk -pdf -outdir="$OUTDIR" -interaction=nonstopmode -halt-on-error -file-line-error \
  -pdflatex='pdflatex -no-shell-escape %O %S' book_main.tex
```

The PDF will be written to `$OUTDIR/book_main.pdf`. Shell escape is disabled; do not enable it unless the build requirements are reviewed and explicitly warrant it.

## Verified baseline

On 2026-10-06, the command succeeded on the `main` snapshot at commit `5d030daf46ff888c15bda204ea5c794819f81860` with `latexmk` 4.83 and pdfTeX/TeX Live 2023 (Debian), producing a 507-page PDF before the back-cover asset was wired into the active entry point. The current product build is 508 pages, with the supplied full-bleed back cover as the final page. The earlier 513-page audit count included blank pages that were later removed, per the owner; the additional page is the restored back cover, not an unexpected blank.

The publication-readiness build without the back cover completed at 507 pages; the follow-up product build including the back cover completed at 508 pages. The 2026-10-07 integrated diagram re-audit candidate also builds at 508 A4 pages, including the back cover as page 508 (SHA-256 `b8cef6c11222ec6a74e1ced0bc289473d0f7e4a18f15543f129b23b4c5bb2b92`). Its final log has no fatal errors or unresolved references/citations; it reports 177 overfull horizontal boxes, 14 underfull horizontal boxes, 2 overfull vertical boxes, 11 missing-character diagnostics for semicolons in `nullfont`, and 1 duplicate PDF destination. Treat these diagnostics as a QA backlog, not as proof of failure or as automatically harmless; inspect their locations before approving a release candidate.
