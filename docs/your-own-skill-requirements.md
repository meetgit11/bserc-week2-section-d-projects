# Your Own Skill (/viva) — requirements and verification

Source: BSERC Week 2 PDF, Section D, Project 16 (Your Own Skill).

## Requirements (from the PDF)

- One agent skill that works in a brand-new session.
- /viva: asks viva questions from your notes, one at a time, then scores you.
- Done when: it starts correctly in a fresh session; works well on 3 different inputs; run the same task without the skill and show what got better.

## What was built

- `SKILL.md` — name: viva; description and trigger; input (the notes file, the only source of questions); 6 instruction steps (read notes first; pick 5 questions; ask one at a time; judge immediately; keep score; end with score + revision pointer); rules (questions and correct answers only from the notes; never reveal the next question; max 5 questions unless asked; plain language; reply in the user's language).
- 3 fake sample notes: thermodynamics, Ohm's law, photosynthesis.
- `test-log.md` + `test-runs/` — 3 builder-simulated runs (5 Nov 2026) + 3 fresh-session runs and 1 no-skill comparison (7 Nov 2026), all with full transcripts.

## Verification

| Check | Result |
|---|---|
| Starts correctly in a fresh session | Pass — 7 Nov 2026: 3 independent sessions read SKILL.md cold; all read the notes first, listed topics, asked 5 questions one at a time, ended with score + revision pointers |
| Works well on 3 different inputs | Pass — thermodynamics 3/5, Ohm's law 3/5, photosynthesis 3/5 (7 Nov 2026, fresh sessions) |
| Same task without the skill, show what got better | Pass — 7 Nov 2026: no-skill run on the same thermo notes also scored 3/5 but unstructured (invented marking, mid-quiz corrections, loose tips); the skill added one-at-a-time as a rule, an explicit scoring scheme, feedback timing, a fixed revision format, coverage and answer-checking against the notes |
| Questions and answers only from the notes | Pass in all fresh runs — nothing invented |
| Score format X/5 + revision pointer | Pass in all fresh runs |

## Fixes made after the fresh runs (7 Nov 2026)

Two gaps were found independently by two of the three fresh-session agents, so both were fixed with one-line clarifications in `SKILL.md`:
1. **Step 5** — added: "If the follow-up is also wrong or not answered, the question scores 0 — a correct follow-up after a partial answer still scores 0.5."
2. **Step 6** — the revision-pointer example now says to cite the section heading for notes without page numbers ("Revise §2 — Carnot efficiency").

Smaller notes from the fresh runs, not fixed (judgement calls, not errors): the skill does not say whether to show the topic list to the user or keep it internal; it gives no guidance for a student asking for a hint or answering with a question; five questions across three short topics forces doubling up on one topic.

## Still open

- A live multi-turn viva with a real student — the true test of step 3's "stop and wait" across turns. The fresh runs played both interviewer and student inside one session.
- A run on a real notes file of the user's own (not a sample), checking every question comes from those notes only.
