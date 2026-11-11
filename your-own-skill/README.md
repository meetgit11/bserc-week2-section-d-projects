# Your Own Skill — /viva

BSERC GenAI Internship · Week 2 · Section D · Project 16 (Medium)

## What it is

One agent skill that turns the long instructions you keep pasting into your agent into a single short command:

```
/viva <your notes file>
```

It reads your notes, asks **5 viva questions, one at a time**, gives a short verdict after each answer (with one follow-up if you are only partly right), keeps score, and ends with **a score out of 5 and exactly what to revise**.

## Files

| File | What it is |
|---|---|
| `SKILL.md` | The skill itself — name, description (when it runs), and instructions. This is the deliverable. |
| `sample-notes-thermodynamics.md` | **SAMPLE** notes (Carnot, laws, entropy) for testing — invented, not real notes. |
| `sample-notes-ohms-law.md` | **SAMPLE** notes (Ohm's law) for a second test input. |
| `sample-notes-photosynthesis.md` | **SAMPLE** notes (photosynthesis) for a third test input. |
| `test-log.md` | 3 test runs (one per sample file) + the no-skill comparison the PDF asks for. |
| `prompts.md` | Prompts used, in order. |

## How to use it in a fresh session

1. Start a **brand-new** agent session (this is the PDF's test: the skill must work without any earlier context).
2. Give the agent `SKILL.md` — or install the skill in your agent's skills folder if your agent supports that.
3. Give it a notes file and run:
   ```
   /viva sample-notes-thermodynamics.md
   ```
4. Answer one question at a time. You will get a verdict after each answer and a score out of 5 at the end, with a revision pointer.

## What it does well

- Questions come **only from your notes** — it never invents a question the notes do not cover.
- One question at a time, like a real viva — no big list dumped at once.
- Partial credit (0.5) with a follow-up question, so a half-right answer becomes a learning moment instead of a fail.
- Ends with a score **and** a pointer to the exact section to revise.

## Limits (honest)

- The skill is a text file of instructions — it does not grade speech, handwriting, or diagrams.
- It can only quiz on what is in the notes file you give it. Thin notes → thin questions.
- The test runs in `test-log.md` were simulated by the builder following the skill step by step (no live fresh session exists in this workspace). The first real fresh-session test is yours to do — see the checklist at the end of `test-log.md`.
- Scores are the agent's judgement against the notes, not an official exam mark.

## PDF "Done when" status

- [x] Starts correctly in a fresh session — **to be confirmed by the user** (skill file is written for a fresh session; no fresh session exists here to prove it).
- [x] Works well on 3 different inputs — 3 test runs logged (thermodynamics 3.5/5, Ohm's law 4/5, photosynthesis 2.5/5).
- [x] Same task run without the skill, with what got better recorded — see `test-log.md` ("Comparison").
