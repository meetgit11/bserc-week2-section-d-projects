# Test checklist — Same Page, New Design (BSERC Week 2, Section D)

PDF "Done when": you have both before.html and after.html; the words in both files match; the redesign works on a phone; you can name 3 design changes and why each one helps.

## Verified in this workspace (5 Nov 2026)

- [x] **Both files exist** — `before.html` (951 bytes) and `after.html` (~3.8 KB) in this folder.
- [x] **Words match exactly** — strip-tags + normalise-whitespace script run on both files: full visible text **IDENTICAL**, 63 words each, same order; body-only text also identical. The one mismatch found on the first run (link/menu order inside the cards) was fixed and the diff re-run clean. No extra visible text was added in `after.html` (no footer, no extra labels, no CSS `content:` text).
- [x] **Offline** — zero external references in both files (no `http(s)://`, no external src/href/img/link, no external fonts); system font stacks only.
- [x] **No JavaScript** — neither file contains a `<script>`, so there is no JS to syntax-check.
- [x] **Design skill written, honestly labelled** — `design-skill.md` is my own written skill (`page-redesign`), explicitly **not** the "Impeccable" skill from skills.sh; it was not installed from anywhere.
- [x] **3+ design changes named with reasons** — 5 changes with reasons in `README.md` (hero + one action; card grouping; colour palette; type scale; mobile layout). The critique step (before redesigning) is also in the README.
- [x] **Mobile layout, by inspection** — `after.html` has a viewport meta tag, `box-sizing: border-box`, fluid layout (`max-width: 960px`, `width: 100%` via grid), and a `@media (max-width: 640px)` query that stacks the two cards into one column and shrinks the hero. No fixed pixel widths wider than the viewport; no element is positioned outside the flow.

## Still to verify on the user's phone (no browser in this VM)

- [ ] Open `after.html` on a real phone and confirm there is no horizontal scrolling/overflow, the hero headline fits, and the two cards stack in one column.
- [ ] Open `before.html` and `after.html` side by side and confirm the redesign reads as the same page with the same words.

## Live phone test (12 Nov 2026, user's phone)
- [x] **Redesign works on a phone — PASS (user-reported).** after.html opens on the user's mobile, slides downwards (vertical scroll only), page fits properly, no sideways sliding. Cards stacking in one column was not explicitly confirmed by the user, but no horizontal overflow on a phone-width screen plus the under-640px one-column media query in after.html supports it; recorded here as an inference, not a user report.
