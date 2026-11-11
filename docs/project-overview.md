# Section D — project overview

Two projects, built for the BSERC GenAI Internship Week 2 (Section D: video, skills and design), and tested as described below.

## Your Own Skill (/viva)

An agent skill that quizzes the user from their notes.

- **Skill file:** `SKILL.md` (name: viva). Give it a notes file (Markdown, text, or PDF) and run `/viva`.
- **Flow:** reads the notes first and lists its main topics; picks 5 questions covering different topics, mixing recall and understanding, answerable from the notes alone; asks one question at a time and waits; judges each answer immediately (correct / partly with one follow-up / wrong with the correct answer); keeps a silent tally; ends with `Score: X/5`, one revision line per non-full-marks question, and one encouraging line.
- **Scoring:** 1 correct, 0.5 partly correct after the follow-up (a correct follow-up still scores 0.5), 0 wrong / not answered / failed follow-up.
- **Test inputs:** 3 fake sample notes (thermodynamics, Ohm's law, photosynthesis). No real exam material was used.
- **Key files:** `SKILL.md`, `sample-notes-*.md`, `test-log.md`, `test-runs/` (full transcripts).

## Same Page, New Design

A plain TECHNOVA 2026 event page redesigned with a written design skill, keeping the words identical.

- **Step 1:** `before.html` — a simple page built without a skill.
- **Step 2:** `design-skill.md` — a self-written design skill (explicitly NOT the Impeccable skill from skills.sh).
- **Step 3:** `after.html` — the same page redesigned with the skill on.
- **Words:** identical in both files — 63 words each, same order (re-checked 7 Nov 2026).
- **Key files:** `before.html`, `after.html`, `design-skill.md`.

## Shared facts

- **Stack:** plain text/Markdown for the skill; plain HTML/CSS for the pages. No build step, no dependencies, no server, no account, no login.
- **Status (12 Nov 2026):** both projects complete and verified as far as the PDF's lists allow. Open checks: a live multi-turn viva with a real student; a /viva run on a real notes file of the user's own. See `testing-report.md`.
