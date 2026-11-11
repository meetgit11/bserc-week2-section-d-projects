# /viva — Fresh-session test run (thermodynamics)

- **Date:** 7 November 2026
- **Skill:** `/viva` (`SKILL.md`), run cold in a brand-new session that had never seen the skill before.
- **Notes file:** `sample-notes-thermodynamics.md` (sample notes, invented for testing).
- **Student ability simulated:** mixed — 2 correct, 2 partial, 1 wrong.
- **Interviewer note:** the skill was followed step by step as written. The "student" answers below are the simulated answers given in this test run.

## Setup (skill step 1)

**Interviewer:** Reading notes. Asking 5 questions, one at a time.

Main topics in the notes:
1. The laws of thermodynamics (zeroth, first, second)
2. Heat engines and the Carnot cycle
3. Entropy
4. Key terms (isothermal, adiabatic, internal energy, kelvin)

---

## Q1 — Zeroth law (recall, §1)

**Interviewer:** What does the zeroth law say, and why does it matter?

**Student:** If two bodies are each in thermal equilibrium with a third body, they are in thermal equilibrium with each other. It matters because that is what makes temperature a meaningful, measurable quantity.

**Interviewer:** Correct. **[Score so far: 1]**

---

## Q2 — Carnot efficiency (understanding, §2)

**Interviewer:** A heat engine works between a hot reservoir at Th and a cold reservoir at Tc. If you raise Th, what happens to the Carnot efficiency, and why?

**Student:** The efficiency goes up, because the hot reservoir can supply more heat to the engine.

**Interviewer:** Partly. You are right that it rises — but what is the formula, and which temperatures go in it?

**Student:** η = 1 − Tc / Th, with both temperatures in kelvin. Raising Th makes Tc/Th smaller, so η gets closer to 1.

**Interviewer:** That's it. **[Score so far: 1.5]**

---

## Q3 — Entropy of melting ice (understanding, §3)

**Interviewer:** Ice melts in a warm room. What happens to the total entropy, and why?

**Student:** The total entropy rises. The entropy of the ice increases more than the entropy of the room decreases, so overall it goes up — that's the second law.

**Interviewer:** Correct. **[Score so far: 2.5]**

---

## Q4 — First law (recall, §1)

**Interviewer:** State the first law as it is written in your notes, including what each symbol means.

**Student:** ΔU = Q + W, where W is the work done on the system.

**Interviewer:** Wrong — the notes write it as ΔU = Q − W, where W is the work done *by* the system. Noted as a point to revise. **[Score so far: 2.5]**

---

## Q5 — Why no engine is 100% efficient (understanding, §2)

**Interviewer:** Why can no engine ever be 100% efficient?

**Student:** Because of friction and heat loss in real engines.

**Interviewer:** Partly. Friction lowers real engines, but what about an ideal one?

**Student:** Even a perfect, frictionless engine can't beat Carnot efficiency, because the second law forbids it.

**Interviewer:** That's it. **[Score so far: 3]**

---

## Final report (skill step 6)

Score: 3/5.

- Revise §1 — First law: ΔU = Q − W, with W = work done *by* the system (not on it).
- Revise §2 — Carnot efficiency: η = 1 − Tc/Th in kelvin, and why raising Th (or lowering Tc) raises it.
- Revise §2 — Why even a perfect, frictionless engine cannot be 100% efficient (the second law, not just friction).

Strongest part: your recall of the laws and entropy was spot on — Q1 and Q3 were both fully correct.

---

## Verdict (test-run assessment)

- **Did the skill start correctly in a fresh session?** Yes. Read cold, the skill was self-contained: it said when to run, what the input is, and gave numbered steps. No prior context was needed. It read the notes first, listed the 4 main topics, and announced the format before asking anything.
- **Did it ask one question at a time?** Yes. Each question was asked, answered, and judged before the next one appeared. All 5 questions were asked, none in advance, and no extra questions were added.
- **Did the stated flow happen?** Yes: questions one at a time; verdict after each answer (correct / partly with follow-up / wrong with correction); running tally kept silent until the end; final `Score: 3/5.`; one revision line per question without full marks, each pointing at the notes section; one encouraging line about the strongest part.
- **Answer labels:** Q1 correct (1), Q2 partial (0.5), Q3 correct (1), Q4 wrong (0), Q5 partial (0.5). Total 3/5.

### Ambiguities / gaps found when reading cold

1. **Follow-up failure is undefined.** Step 4 says a partly-correct answer gets one short follow-up, and step 5 scores 0.5 for "partly correct after the follow-up". It never says what the score is if the student *also* fails the follow-up — still 0.5, or 0? In this run both follow-ups were answered correctly, so it did not matter, but a strict reader would have to guess. Suggested fix: one line, e.g. "If the follow-up is also wrong, score 0."
2. **"Correct" vs "partly" is left entirely to the interviewer's judgement.** That is probably unavoidable in a viva, but the skill gives no examples of where the line falls (e.g. right idea but wrong formula = partly, as used here). A one-line example would help a fresh reader.
3. **No instruction for a mid-viva student question.** If the student asks "can you repeat that?" or answers with a question, the skill does not say what to do. Minor — the natural reading is to re-ask or clarify and continue — but it is not written down.
4. **"Say briefly what you are about to do" gives one example phrase only.** The example ("Reading notes. Asking 5 questions, one at a time.") was usable as-is, so this is not a blocker, just a note that the opener is left to the reader's wording.

### Things I had to guess

- The exact wording of the opening line (used the skill's example verbatim).
- The Q2/Q5 follow-up questions (the skill gives one example follow-up for the friction case, which I reused for Q5; for Q2 I invented one in the same style: "what is the formula, and which temperatures go in it?").
- Whether a correct follow-up after a partial answer earns 0.5 (assumed yes, per step 5's wording "partly correct after the follow-up").
- What "where it is in the notes" means for the revision pointer — the notes have numbered sections, so I cited §1/§2. A notes file without sections would make this harder; page numbers are suggested in the skill's example, but these notes have no pages.

### What the skill did well (observed, not assumed)

- Self-contained and runnable cold: no missing inputs, no undefined terms, no step that could not be executed.
- The "one question at a time, stop and wait" rule is stated twice (steps 3 and the Rules), and it worked.
- The verdict format (correct / partly + follow-up / wrong + correction) is concrete enough to follow mechanically.
- The ban on inventing answers ("If the notes do not contain an answer, do not invent one") is explicit and was not triggered here, since all 5 questions were answerable from the notes alone.
