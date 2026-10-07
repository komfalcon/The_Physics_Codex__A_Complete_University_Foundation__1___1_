# Diagram re-audit — 7 October 2026

The fresh source/PDF audit covers **139 visual items**: 31 instructional diagrams in Chapters 1–7, 35 in Chapters 8–14, 36 in Chapters 15–21, 35 in Chapters 22–29, and two front-matter TikZ graphics. All 139 received an individual baseline disposition. **65 instructional diagrams were corrected** (20, 11, 7, and 27 by range); the remaining 72 instructional diagrams were accepted unchanged. The two front-matter graphics are decorative rather than teaching diagrams; neither was edited.

All 65 changed diagrams have post-edit rendered checks documented in their range reports. In the final integrated r5 PDF, the six latest source-correction pages—physical pp.87, 90, 111, 158, 192, and 255—were rechecked with no remaining collision or label-association issue. Pages 290 and 329 were also rechecked; the Chapter 22–29 final locator sweep confirms all 35 figure locations remain stable, including the seven pages supplied as screenshots. This does not mean every one of the 139 was re-rendered in a new, separate r5 pass: unchanged/source-stable figures rely on their individually documented baseline and prior final-render checks.

## Final integrated build

The candidate was built from branch `docs/diagram-reaudit-2026-10-07`, based on merged `main` commit `10ea81c`. The forced `book_main.tex` build completed successfully at **508 A4 pages**; the full-bleed back cover is page 508. The final PDF is `/tmp/physics-codex-diagram-reaudit-final-r5/book_main.pdf`, SHA-256 `b8cef6c11222ec6a74e1ced0bc289473d0f7e4a18f15543f129b23b4c5bb2b92`. The final log has no fatal TeX errors or unresolved references/citations.

The log still reports **177 overfull hboxes, 14 underfull hboxes, 2 overfull vboxes, 11 missing-semicolon glyph notices, and 1 duplicate PDF destination**. These are whole-book QA warnings; not all are caused by the diagrams in this review, and their causes are not all resolved. The warning count is not a publication certification.

## Range checklists

- [Chapters 1–7 and front matter](CH1-7_DIAGRAM_REVIEW_2026-10-07.md) — 33 items; 20 instructional edits; final r5 spot-checks on pp.87, 90, and 111.
- [Chapters 8–14](CHAPTER_08_14_DIAGRAM_REAUDIT_2026-10-07.md) — 35 items; 11 edited figures; final r5 checks on pp.158 and 192.
- [Chapters 15–21](CHAPTER_15_21_DIAGRAM_REAUDIT_2026-10-07.md) — 36 items; 7 edited figures; final r5 checks on pp.255, 290, and 329.
- [Chapters 22–29](CHAPTER_22_29_DIAGRAM_REAUDIT_2026-10-07.md) — 35 items; 27 edited figures; all 35 locations were reconfirmed in r5, and the seven supplied screenshot pages were checked.

## Items still requiring owner/release judgment

The decorative atom emblem remains unchanged; it could be mistaken for a planetary electron-orbit model, so replacing it with abstract geometry or explicitly marking it as decorative remains an editorial choice. The greenhouse figure still omits solar albedo because the source does not say whether reflection is at a cloud or the surface.

This diagram-only audit does not resolve the book’s other release decisions: the back-cover ISBN remains a placeholder; Chapter 10’s bicycle answer-key assumptions about pedal torque and input versus wheel-output power need an owner choice; Chapter 20’s real-object-positive optics convention awaits confirmation; and broader physics-accuracy, citation, and pedagogy sign-offs remain separate work. The covers’ existing design is retained; the displayed author email is `falcon@aurikrex.com`. No ISBN has been invented.
