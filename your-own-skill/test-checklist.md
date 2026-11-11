# Test checklist — Your Own Skill /viva (BSERC Week 2, Section D)

PDF "Done when": the skill starts correctly in a fresh session; it works well on
3 different inputs; run the same task without the skill and show what got better.

## Verified in this workspace (5 Nov 2026)

- [x] **Skill file exists** — `SKILL.md` (43 lines) plus `README.md`, `prompts.md`,
  and 3 sample notes files (thermodynamics, Ohm's law, photosynthesis).
- [x] **Works on 3 different inputs (simulated)** — see `test-log.md`: thermo 3.5/5,
  Ohm's law 4/5, photosynthesis 2.5/5. Each run asked 5 questions one at a time,
  gave per-answer verdicts with one follow-up on partly-correct answers, and
  ended with a score + revision pointer.
- [x] **Without-skill comparison done** — same thermo task run as a plain
  "quiz me" request: all 5 questions in one list, no waiting, bare "3/5, good
  effort" with no per-answer verdicts, no follow-up, no revision pointer.
  With the skill: one question at a time, follow-up rescued the half-right
  Carnot answer to 0.5, score carried a revision pointer, questions spread
  across topics.
- [x] **Offline / no paid API / no login** — plain skill text; nothing to install
  from anywhere, no external calls.

## Honest note on the runs above

The 3 runs in `test-log.md` were simulated by the builder following `SKILL.md`
step by step (examiner and student played by the same person, using only the
sample notes). They prove the skill's rules work as written — they do **not**
claim a real fresh agent session ran. The fresh-session test below is the one
that closes this project.

## Still to verify (user, in a fresh session — the Section D finish step)

- [ ] Open a brand-new agent session, give it `SKILL.md`, and run
  `/viva sample-notes-thermodynamics.md`. Confirm it reads the notes, asks
  5 questions one at a time, and ends with a score + revision pointer.
- [ ] Repeat with a real notes file of your own (not a sample) and check every
  question comes from your notes only.

## After the fresh-session test

- [ ] Push Section D to GitHub (same pattern as Sections B and C — user approval
  first), then Section D mini report, then the collective Week 2 report.
