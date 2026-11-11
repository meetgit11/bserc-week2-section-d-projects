# Same Page, New Design — requirements and verification

Source: BSERC Week 2 PDF, Section D, Project 17 (Same Page, New Design).

## Requirements (from the PDF)

- Step 1, without a skill: build a simple page and save as `before.html`.
- Step 2: add a design skill (Impeccable, or frontend-design / ui-ux-pro from skills.sh).
- Step 3: redesign with the skill on the same page, save as `after.html`.
- Done when: both files exist; the words in both files match; the redesign works on a phone; you can name 3 design changes and why each one helps.

## What was built

- `before.html` — plain TECHNOVA 2026 event page, built without a skill.
- `design-skill.md` — a self-written design skill. Note: this is explicitly NOT the Impeccable skill from skills.sh; it was written for this project instead.
- `after.html` — the same page redesigned with the skill on.
- `README.md` — critique of `before.html`, 5 design changes with reasons, verification summary, honest limits.

## Verification

| Check | Result |
|---|---|
| Both files exist | Pass |
| Words in both files match | Pass — 63 words each, same order, identical text (re-checked 7 Nov 2026 by script) |
| Redesign works on a phone | Pass — 12 Nov 2026 (user-reported): after.html opens on his mobile, scrolls down properly, fits, no sideways sliding |
| 3 design changes named, with reasons | Pass — 5 changes documented in the README |

## Phone check — honest note

The browser phone-width render attempted on 7 Nov 2026 produced no result (file uploads to the viewer kept aborting, neither page loaded), so the phone verdict rests on the user's own phone, not on a render: on 12 Nov 2026 he reported the page opens on his mobile, slides down properly, fits, and does not slide sideways. Cards stacking in one column was not explicitly confirmed — it is inferred from no horizontal overflow plus the under-640px one-column media query in `after.html`, and is recorded as an inference, not a user report. The static audit supports a pass (viewport meta, border-box, no fixed widths wider than the viewport, `.cards` collapses to one column under 640px, hero type uses `clamp()`, `.highlights` / `.menu` use `flex-wrap`).
