# Section D — testing report

Test dates: 5–12 November 2026. Builder-simulated runs were done by the author following `SKILL.md`; fresh-session runs were done by independent agents that read `SKILL.md` cold on 7 Nov 2026; the phone check was done by the user on his own phone on 12 Nov 2026.

## Your Own Skill (/viva)

| Check | Result |
|---|---|
| Starts correctly in a fresh session | Pass — 7 Nov 2026: 3 independent fresh sessions, skill read cold |
| Works well on 3 different inputs | Pass — thermodynamics 3/5, Ohm's law 3/5, photosynthesis 3/5 |
| Same task without the skill, show what got better | Pass — 7 Nov 2026: no-skill run (same notes) scored 3/5 but unstructured; the skill added one-at-a-time as a rule, an explicit scoring scheme, feedback timing, a fixed revision format, coverage and answer-checking |
| Questions and answers only from the notes | Pass in all fresh runs |
| Score format X/5 + revision pointer | Pass in all fresh runs |
| Live multi-turn viva with a real student | Not yet — the fresh runs played both interviewer and student inside one session |
| Run on a real notes file of the user's own | Not yet |

Fresh-session scores (7 Nov 2026, full transcripts in `your-own-skill/test-runs/`):
- Thermodynamics: 3/5 — strongest on the zeroth law and entropy; revise first-law sign convention, Carnot formula, second law.
- Ohm's law: 3/5 — strongest on Ohm's law and series circuits; revise R = ρL/A, parallel total resistance, power formulae.
- Photosynthesis: 3/5 — strongest on the equation and location/pigment; revise Calvin cycle inputs (ATP + NADPH), temperature (enzymes denature), limiting factor.
- Thermodynamics without the skill: 3/5 — loose revision tips, no fixed format.

Builder-simulated runs (5 Nov 2026, in `test-log.md`): thermodynamics 3.5/5, Ohm's law 4/5, photosynthesis 2.5/5, plus a no-skill comparison. These were the builder playing both parts and are kept in the log as simulated runs; the 7 Nov fresh runs are the evidence for the PDF's "fresh session" item.

## Same Page, New Design

| Check | Result |
|---|---|
| Both files exist | Pass |
| Words in both files match | Pass — 63 words each, same order, identical text (re-checked 7 Nov 2026 by script) |
| Redesign works on a phone | Pass — 12 Nov 2026 (user-reported): opens on his mobile, scrolls down properly, fits, no sideways sliding |
| 3 design changes named, with reasons | Pass — 5 changes documented in the README |

Honest note on the phone check: a browser phone-width render attempted on 7 Nov 2026 produced no result (uploads kept aborting, neither page loaded). The verdict rests on the user's phone. Cards stacking in one column was not explicitly confirmed — inferred from no horizontal overflow plus the under-640px one-column media query, recorded as an inference.

## Static checks (author's workspace)

- `SKILL.md` is valid frontmatter + Markdown; the skill name is `viva`.
- All sample notes and test-run transcripts are plain Markdown, no external references.
- `before.html` / `after.html`: visible text extracted by stripping tags is identical (63 words, same order); both files carry a viewport meta tag; `after.html` has one `@media` rule (under 640px, `.cards` to one column).
- No JavaScript, no external resources, no network calls in either page.
