# Test log — /viva skill (BSERC Week 2, Section D, Project 16)

**How this log was made (honest note):** Runs 1–3 (5 Nov 2026) were simulated by me, the builder, following `SKILL.md` step by step — I played both examiner and student, using only the sample notes files. Runs 4–7 (7 Nov 2026) are fresh-session runs by independent agents that read `SKILL.md` cold and had never seen it before; full transcripts are in `test-runs/`. In all runs the student role was played by the testing agent, not by a real student — so a live multi-turn viva with a real student is still the true test of step 3's "stop and wait". Nothing here claims a real student sat a viva.

## Run 1 — sample-notes-thermodynamics.md (5 Nov 2026)

Topics found in the notes: laws of thermodynamics, Carnot cycle, entropy, key terms.

- **Q1. What does the first law of thermodynamics say?**
  Student: "Energy is conserved — the change in internal energy equals heat added minus work done by the system."
  Verdict: Correct. (1)
- **Q2. Why can no engine beat Carnot efficiency?**
  Student: "Because of friction."
  Verdict: Partly. Friction lowers real engines, but what about an ideal one? → Student: "The second law — even a perfect engine can't beat it." (0.5)
- **Q3. What is entropy?**
  Student: "A measure of disorder — the entropy of an isolated system never decreases."
  Verdict: Correct. (1)
- **Q4. In the Carnot formula η = 1 − Tc / Th, what temperature scale must you use?**
  Student: "Celsius."
  Verdict: Wrong — temperatures must be in kelvin; 0 K = −273.15 °C. Revise §4, Key terms. (0)
- **Q5. What is the difference between an isothermal and an adiabatic process?**
  Student: "Isothermal is constant temperature; adiabatic is no heat exchange with the surroundings."
  Verdict: Correct. (1)

**Score: 3.5/5.** Strongest: the laws and entropy. Revise: Carnot efficiency — why even an ideal engine cannot beat it (§2), and always use kelvin in the formula (§4).
*(Note: the PDF preview shows a 3/5 run on the same Q2 — this run scored 3.5/5 because the follow-up was answered correctly, which is exactly the partial-credit rule in SKILL.md.)*

## Run 2 — sample-notes-ohms-law.md (5 Nov 2026)

- **Q1. State Ohm's law.** Student: "V = IR — current is proportional to voltage at constant temperature." Correct. (1)
- **Q2. A wire is made twice as long and twice as thick. What happens to its resistance?** Student: "R = ρL/A, so doubling L doubles R and doubling A halves it — resistance stays the same." Correct. (1)
- **Q3. Two resistors in parallel — what is the same across both?** Student: "The current." Verdict: Wrong — the voltage is the same; the current splits. Revise §3. (0)
- **Q4. How much power does a resistor dissipate?** Student: "P = VI, which is the same as I²R." Correct. (1)
- **Q5. Why does a resistor get hot?** Student: "It converts electrical energy into heat." Correct. (1)

**Score: 4/5.** Strongest: formulae and series/parallel reasoning. Revise: parallel circuits — voltage is shared, current splits (§3).

## Run 3 — sample-notes-photosynthesis.md (5 Nov 2026)

- **Q1. Write the overall equation for photosynthesis.** Student: "6CO₂ + 6H₂O → glucose + oxygen, using light." Correct. (1)
- **Q2. Where in the cell does photosynthesis happen?** Student: "In the mitochondria." Verdict: Wrong — in the chloroplasts (chlorophyll). Revise §1. (0)
- **Q3. What do the light-dependent reactions produce?** Student: "Oxygen and glucose." Verdict: Partly — oxygen is released and ATP + NADPH are produced; glucose is made later, in the Calvin cycle. (0.5)
- **Q4. Name one factor that limits the rate of photosynthesis.** Student: "Light intensity." Correct. (1)
- **Q5. What happens to the rate if the temperature gets very high?** Student: "I don't know." Verdict: The enzymes denature, so the rate falls. Revise §3. (0)

**Score: 2.5/5.** Strongest: the overall equation. Revise: where photosynthesis happens (§1), the two stages (§2), and temperature effects (§3).

## Comparison — the same task WITHOUT the skill (5 Nov 2026)

I did the thermo viva once without following `SKILL.md`, as a plain "quiz me on these notes" request.

What happened without the skill:
- All 5 questions were asked in one big list, with no waiting — the student had to answer them all at once, in writing, with no chance to think one at a time.
- Answers got a single short reply ("3/5, good effort") with no per-answer verdicts, no follow-up on the half-right Carnot answer, and no pointer to which section to revise.
- The score was given with no breakdown, so the student could not tell which topic was weak.

What got better **with** the skill:
1. **One question at a time** — the student thinks and answers before moving on, like a real viva.
2. **Immediate verdicts + one follow-up** — the partly-correct Carnot answer (Q2) was rescued to 0.5 instead of being marked wrong, and the student actually learned the second-law reason.
3. **A score with a revision pointer** — "Revise §2 and §4" tells the student exactly what to study next, instead of a bare "3/5".
4. **Coverage** — the 5 questions were deliberately spread across different topics instead of clustering on the first page.

## Still to verify (user, in a fresh session)
- [x] Open a brand-new agent session, give it `SKILL.md` (or install the skill), and run `/viva sample-notes-thermodynamics.md`. Confirm it reads the notes, asks 5 questions one at a time, and ends with a score + revision pointer. — **Done 7 Nov 2026:** three independent fresh sessions (Runs 4–6) read the skill cold; all three read the notes first, asked 5 questions one at a time with immediate verdicts, and ended with `Score: X/5` + revision pointers. Full transcripts in `test-runs/`.
- [ ] Repeat with a real notes file of your own (not a sample) and check every question comes from your notes only.
- [ ] A live multi-turn viva with a real student, to truly test step 3's "stop and wait" across turns.

## Run 4 — sample-notes-thermodynamics.md, FRESH session (7 Nov 2026)

Independent agent, read `SKILL.md` cold. Full transcript: `test-runs/viva-thermodynamics-fresh.md`.

- Q1 Zeroth law — Correct. (1)
- Q2 Carnot efficiency — Partly (right idea, missing the formula); follow-up answered correctly. (0.5)
- Q3 Entropy of melting ice — Correct. (1)
- Q4 First law — Wrong (student used ΔU = Q + W, W done *on* the system; notes say ΔU = Q − W, W done *by* the system). (0)
- Q5 Why no engine is 100% efficient — Partly ("friction and heat loss"); follow-up (the skill's own example: "what about an ideal one?") answered correctly. (0.5)

**Score: 3/5.** Revise: §1 first-law sign convention, §2 Carnot formula (η = 1 − Tc/Th, kelvin), §2 second law. Strongest: Q1/Q3 spot on.

## Run 5 — sample-notes-ohms-law.md, FRESH session (7 Nov 2026)

Independent agent, read `SKILL.md` cold. Full transcript: `test-runs/viva-ohms-law-fresh.md`.

- Q1 State Ohm's law — Correct. (1)
- Q2 Doubling a wire's length — Partly (right that R rises); follow-up (R = ρL/A, R doubles) answered correctly. (0.5)
- Q3 Series circuit — Correct (same current; total R = R1 + R2). (1)
- Q4 Parallel resistors — Wrong (student said total R is bigger; it is smaller than the smallest resistor). (0)
- Q5 Energy conversion + power formula — Partly (heat, right); follow-up (P = VI = I²R = V²/R) answered correctly. (0.5)

**Score: 3/5.** Revise: "Resistance" (R = ρL/A), "Series and parallel" (parallel total < smallest), "Resistance" (power formulae). Strongest: Ohm's law itself and series circuits.

## Run 6 — sample-notes-photosynthesis.md, FRESH session (7 Nov 2026)

Independent agent, read `SKILL.md` cold. Full transcript: `test-runs/viva-photosynthesis-fresh.md`.

- Q1 Overall equation — Correct. (1)
- Q2 Calvin cycle inputs — Partly (ATP only); follow-up (NADPH) answered correctly. (0.5)
- Q3 Where photosynthesis happens + pigment — Correct (chloroplasts + chlorophyll). (1)
- Q4 Very high temperature — Wrong (student said the rate speeds up; too hot denatures the enzymes, rate falls). (0)
- Q5 Limiting factor — Partly (vague); follow-up ("shortest supply") completed it. (0.5)

**Score: 3/5.** Revise: §2 Calvin cycle inputs (ATP and NADPH), §3 temperature (enzymes denature), §3 limiting factor. Strongest: the equation and the location/pigment.

## Run 7 — sample-notes-thermodynamics.md, WITHOUT the skill (7 Nov 2026)

Independent agent, no `SKILL.md` read, same notes as Run 4. Full transcript: `test-runs/viva-thermodynamics-no-skill.md`.

- Q1 Zeroth law — Correct. (1)
- Q2 First law — Partly (right formula, mixed up work done *by* vs *on*). (0.5)
- Q3 Carnot efficiency — Correct. (1)
- Q4 Entropy + ΔS formula — Partly (good definition, ΔS = Q/T without the reversibility condition). (0.5)
- Q5 Isothermal vs adiabatic — Wrong (swapped the two). (0)

**Score: 3/5**, with loose revision tips and no fixed format.

What got better **with** the skill (comparing Run 4 with Run 7, same notes, same mixed-ability student):
1. **One question at a time as a rule** — without the skill it happened by habit only; nothing stopped the interviewer from dumping all five questions at once.
2. **An explicit scoring scheme** — without the skill the marking (1 / 0.5 / 0) was invented on the spot and the partial/wrong boundary was a judgement call with no definition.
3. **Feedback timing decided** — without the skill the interviewer corrected answers immediately mid-quiz, so the student heard right answers before the quiz ended.
4. **A fixed revision format** — without the skill the guidance was loose tips in the order mistakes came up, not one pointer per missed question; with the skill each non-full-marks question got one revision line pointing at the notes.
5. **Coverage and verification** — without the skill nothing forced the questions to spread across the notes, and borderline answers were judged from memory, never re-checked against the file.

## Fixes made to SKILL.md after the fresh runs (7 Nov 2026)

Two gaps were found independently by two of the three fresh-session agents, so both were fixed with one-line clarifications:
1. **Step 5** — added: "If the follow-up is also wrong or not answered, the question scores 0 — a correct follow-up after a partial answer still scores 0.5."
2. **Step 6** — the revision-pointer example now says to cite the section heading for notes without page numbers ("Revise §2 — Carnot efficiency").

Smaller notes from the fresh runs, not fixed (judgement calls, not errors): the skill does not say whether to show the topic list to the user or keep it internal; it gives no guidance for a student asking for a hint or answering with a question; five questions across three short topics forces doubling up on one topic.
