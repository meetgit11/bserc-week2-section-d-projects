# prompts.md — Your Own Skill (/viva) (BSERC Week 2, Section D)

Prompts used, in order, as required by the Week 2 PDF.

## 1. Parent agent → builder (5 Nov 2026)
> Build BSERC Week 2 Section D Project 16, "Your Own Skill (/viva)": create one agent skill that works in a brand-new session — /viva asks viva questions from the user's notes, one at a time, then scores the answers. Deliver SKILL.md (frontmatter with name + description, then instructions), a fake sample notes file (thermodynamics: Carnot, laws, entropy — labelled SAMPLE, not the user's real notes), a test log with 3 runs on 3 different inputs plus the no-skill comparison, README.md, and prompts.md starting with this brief.

Result: `SKILL.md` written (name `viva`, description stating when it runs, 6-step instructions + rules); `sample-notes-thermodynamics.md` created; two extra sample inputs added (`sample-notes-ohms-law.md`, `sample-notes-photosynthesis.md`) for the 3-input test; `test-log.md` with 3 simulated runs (3.5/5, 4/5, 2.5/5) and the without-skill comparison; `README.md` with fresh-session install/use steps and limits.

## 2. Builder → itself (5 Nov 2026, honesty check)
> The test runs must be labelled as simulated (builder following the skill), not a live fresh agent session — no such session exists in this workspace.

Result: `test-log.md` and `README.md` both state this plainly, and the fresh-session check is left as a user to-verify item.
