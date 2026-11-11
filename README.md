# BSERC Week 2 — Section D Projects

Two projects developed as part of the Bharat Space Education Research Centre (BSERC) GenAI Internship Week 2: **Your Own Skill (/viva)** and **Same Page, New Design**. Built with AI-assisted development, focusing on practical functionality, privacy, responsive UI/UX and software engineering fundamentals.

> This is an independently developed student project. **BSERC does not endorse it.** Everything below states what was actually built and tested; anything not yet tested is marked as such.

## The two projects

### 1. Your Own Skill — /viva

An agent skill that quizzes you from your notes. Give it a notes file, type `/viva`, and it reads the notes, asks 5 viva questions one at a time, judges each answer immediately, and ends with a score out of 5 plus one revision pointer per missed question.

- **Verified in fresh sessions (7 Nov 2026):** three independent sessions read the skill cold — thermodynamics, Ohm's law, photosynthesis — and each scored 3/5 with the proper flow (notes read first, one question at a time, immediate verdicts, score + revision pointers). A fourth run *without* the skill scored 3/5 too, but unstructured: it invented the marking, corrected answers mid-quiz, and gave loose tips instead of pointers. The skill's value is the structure, not the score.
- **Two one-line fixes came out of testing:** a failed follow-up now scores 0 (that was undefined), and revision pointers cite section headings when notes have no page numbers.
- **Still open:** a live multi-turn viva with a real student (the true test of "stop and wait" across turns), and a run on a real notes file of your own rather than the samples.

See [`your-own-skill/README.md`](your-own-skill/README.md), [`your-own-skill/SKILL.md`](your-own-skill/SKILL.md) and [`your-own-skill/test-log.md`](your-own-skill/test-log.md).

### 2. Same Page, New Design

A plain TECHNOVA 2026 event page (`before.html`) redesigned with a self-written design skill (`after.html`), keeping the words exactly the same.

- **Verified:** the visible text is identical in both files — 63 words each, same order (re-checked 7 Nov 2026). Five design changes with reasons in the README.
- **Phone check passed (12 Nov 2026, user-reported):** `after.html` opens on a phone, scrolls down properly, fits, no sideways sliding. Cards stacking in one column was not explicitly confirmed — inferred from no overflow plus the under-640px one-column rule, and recorded as such in the test checklist.

See [`same-page-new-design/README.md`](same-page-new-design/README.md).

## Repository structure

```
bserc-week2-section-d-projects/
├── README.md, prompts.md, LICENSE (MIT)
├── your-own-skill/               # SKILL.md + sample notes + test log + test runs
│   ├── SKILL.md, README.md, prompts.md, test-checklist.md, test-log.md
│   ├── sample-notes-thermodynamics.md, sample-notes-ohms-law.md, sample-notes-photosynthesis.md
│   └── test-runs/                # full transcripts of the 4 test runs
├── same-page-new-design/         # before.html, after.html, design-skill.md
│   └── README.md, prompts.md, test-checklist.md
└── docs/
    ├── project-overview.md
    ├── your-own-skill-requirements.md
    ├── same-page-new-design-requirements.md
    └── testing-report.md
```

## How to use

**/viva:** give the skill file to a fresh agent session (or install it as a skill), then run `/viva <notes-file>` — for example `/viva thermo-notes.pdf`. The notes file is the only source of questions; with no file it asks for one instead of quizzing from general knowledge.

**Same Page:** open `before.html` and `after.html` in any browser, on any device. No build step, no server, no dependencies.

## Testing

Full per-project checklists with honest pass/open status: [`your-own-skill/test-checklist.md`](your-own-skill/test-checklist.md), [`same-page-new-design/test-checklist.md`](same-page-new-design/test-checklist.md), [`your-own-skill/test-log.md`](your-own-skill/test-log.md), and the consolidated [`docs/testing-report.md`](docs/testing-report.md).

## Prompts

Every prompt used to build these projects, in order: [`prompts.md`](prompts.md) (plus the per-project `prompts.md` files inside each folder).

## License

MIT — see [`LICENSE`](LICENSE). It covers the original code and text only.
