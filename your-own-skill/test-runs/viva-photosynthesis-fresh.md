# Fresh-session test run — /viva on photosynthesis notes

- **Test date:** 7 November 2026
- **Tester:** a brand-new session that had never seen this skill before
- **Notes file:** `sample-notes-photosynthesis.md` (sample notes, invented for testing)
- **Skill file:** `SKILL.md` (command `/viva`)

## Interviewer setup (skill step 1)

Main topics found in the notes (3):

1. What photosynthesis is — equation, chloroplasts, chlorophyll
2. Two stages — light-dependent reactions and the Calvin cycle
3. Factors that affect the rate — light intensity, CO₂ concentration, temperature, limiting factor

Interviewer opening line: "Reading notes. Asking 5 questions, one at a time."

## Transcript (skill steps 3–5: one question at a time, verdict after each answer)

**Interviewer — Q1:** What is the overall equation for photosynthesis?

**Student:** 6CO₂ + 6H₂O + light energy → C₆H₁₂O₆ + 6O₂.

**Interviewer:** Correct.

**— Answer label: CORRECT (1 point) —**

**Interviewer — Q2:** The Calvin cycle builds glucose from carbon dioxide — but what does it need from the light-dependent reactions to do that?

**Student:** It needs ATP for energy.

**Interviewer:** Partly. ATP is right, but the light reactions make a second product the Calvin cycle also uses. What is it?

**Student:** NADPH.

**Interviewer:** That's it — ATP and NADPH.

**— Answer label: PARTIAL (0.5 points) —**

**Interviewer — Q3:** Where in the leaf does photosynthesis take place, and which pigment is involved?

**Student:** In the chloroplasts, and the pigment is chlorophyll.

**Interviewer:** Correct.

**— Answer label: CORRECT (1 point) —**

**Interviewer — Q4:** What happens to the rate of photosynthesis if the temperature gets very high — and why?

**Student:** It speeds up, because more heat means more energy for the reactions.

**Interviewer:** Wrong. Too hot denatures the enzymes, so the rate falls — that's a point to revise.

**— Answer label: WRONG (0 points) —**

**Interviewer — Q5:** What is a limiting factor?

**Student:** It's the factor that limits the rate — like when there isn't enough light.

**Interviewer:** Partly. That's the idea — but how does the factor in shortest supply relate to the overall rate?

**Student:** The one there's least of decides the overall rate.

**Interviewer:** Right — the factor in shortest supply controls the overall rate.

**— Answer label: PARTIAL (0.5 points) —**

## Final result (skill step 6, in the skill's format)

Score: 3/5.

- Revise section 2 — Calvin cycle inputs: the light-dependent reactions supply ATP and NADPH.
- Revise section 3 — temperature: too hot denatures the enzymes, so the rate falls.
- Revise section 3 — limiting factor: the factor in shortest supply controls the overall rate.

Strongest: the equation and the location and pigment — both spot on.

## Verdict — did the skill work as written?

**Did it start correctly in a fresh session?** Yes. The skill was read cold, the notes were read first, the main topics were listed, the brief intro line was given, and questioning started only after that. Nothing in the skill required prior knowledge of it.

**Did it ask one question at a time?** Yes. Each question was asked, answered, and judged before the next one appeared, and all 5 questions were never listed up front. (Caveat: in this test one agent played both parts in a single session, so "stop and wait" was simulated inside the transcript rather than across real turns. The one-at-a-time property held in the transcript, but a real multi-turn run with the actual user is still the true test of step 3.)

**Was anything in SKILL.md ambiguous, missing, or unworkable when read cold?**

1. **Partial scoring is ambiguous.** Step 4 says a partly-correct answer gets a follow-up pointing at the missing part; step 5 scores "0.5 (partly correct after the follow-up)". It never says what happens if the follow-up is also wrong — still 0.5, or 0? I had to guess: I awarded 0.5 when the student answered the follow-up correctly. If the follow-up had also been wrong, I would have had to guess again.
2. **The revision-pointer example assumes paginated notes** ("Revise page 14 — Carnot efficiency"). These notes are Markdown with sections, not pages. I used section references instead — workable, but the example doesn't match non-PDF notes.
3. **"List its main topics" doesn't say whether to show the list to the user** or keep it internal. I stated it briefly; a fresh reader could reasonably do either.
4. **No guidance for a student who asks for a hint** or answers with a question of their own.
5. **Five questions across three short topics forces doubling up.** The skill wants different topics per question, but with only 3 topics in short notes, two questions had to come from one topic (factors, here). Workable, but the skill doesn't acknowledge that.

**Did anything have to be invented?** No. Every question and every correct answer came from the notes alone, as the skill requires.

**Did the stated flow actually happen?** Yes: read notes → brief intro → 5 questions one at a time → immediate short verdicts (2–3 lines each) → silent running tally → final `Score: 3/5` + one revision line per question that did not get full marks + one encouraging line about the strongest part. All of it happened as written.
