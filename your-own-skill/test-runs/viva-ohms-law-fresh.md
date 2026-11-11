# Fresh-session test run — /viva on Ohm's Law notes

- **Date:** 7 November 2026
- **Skill:** `/viva` (`SKILL.md` in this folder)
- **Notes file:** `sample-notes-ohms-law.md`
- **Tester role:** brand-new session; the skill had never been seen before. The tester played both parts: interviewer (following `SKILL.md` step by step) and student (mixed ability).
- **Target student mix:** 2 correct, 2 partial, 1 wrong.

---

## 1. Full question-and-answer transcript

**Interviewer:** Reading your notes on Ohm's law. I found three main topics: Ohm's law (V = IR), resistance (what it depends on, and power), and series and parallel circuits. Asking 5 questions, one at a time.

**Interviewer — Q1:** What is Ohm's law? State the formula and what each letter stands for.

**Student:** V = IR. V is voltage in volts, I is current in amps, and R is resistance in ohms.

**Interviewer:** Correct. That is exactly what the notes say.

**Interviewer — Q2:** If you double the length of a wire, what happens to its resistance — and why?

**Student:** It goes up.

**Interviewer:** Partly. You are right that it goes up — but by how much, and which formula in your notes tells you that?

**Student:** It doubles, because R = ρL/A. Doubling L doubles R if everything else stays the same.

**Interviewer:** Right, that completes it.

**Interviewer — Q3:** In a series circuit, what is the same for every resistor — the current or the voltage? And how do you find the total resistance?

**Student:** The current is the same through each resistor, and the total resistance is R1 + R2.

**Interviewer:** Correct. Both parts are right.

**Interviewer — Q4:** Two resistors in parallel — is the total resistance bigger or smaller than the smallest resistor?

**Student:** Bigger, because you are adding more resistors, so there is more resistance.

**Interviewer:** Wrong. It is smaller — the total resistance in parallel is less than the smallest resistor: 1/R = 1/R1 + 1/R2. Note that one to revise.

**Interviewer — Q5:** A resistor converts electrical energy into what? And how much power does it dissipate — give one formula.

**Student:** It converts electrical energy into heat.

**Interviewer:** Partly. Heat is right — but what is the power formula?

**Student:** P = I²R… I think? Or P = VI.

**Interviewer:** Yes — P = VI = I²R = V²/R. That completes it.

---

## 2. Final score and revision pointer (as the skill formats them)

**Score: 3/5.**

- Q1 — Correct (1)
- Q2 — Partly correct (0.5)
- Q3 — Correct (1)
- Q4 — Wrong (0)
- Q5 — Partly correct (0.5)

**Revise:**
- Revise "Resistance" (R = ρL/A) — doubling the length doubles the resistance.
- Revise "Series and parallel" — in parallel, total resistance is less than the smallest resistor (1/R = 1/R1 + 1/R2).
- Revise "Resistance" — power dissipated by a resistor: P = VI = I²R = V²/R.

**Strongest:** the basics were spot on — Ohm's law itself and series circuits were both fully correct.

---

## 3. Verdict: did the skill work when read cold?

**Did the skill start correctly in a fresh session?** Yes. Step 1 was followed literally: the notes were read first, the main topics were listed (three topics), and the interviewer announced the plan ("Asking 5 questions, one at a time") before asking anything. No question was asked before the notes were read.

**Did it ask one question at a time?** Yes. Each question was asked, answered, and judged before the next one appeared. The next question was never revealed in advance, and all 5 questions were never listed up front.

**Was any instruction ambiguous, missing, or unworkable?** Nothing was unworkable, and no instruction was missing. Three small things had to be interpreted, not guessed blindly:

1. **Revision pointers assume page numbers.** Step 6's example says "Revise page 14 — Carnot efficiency", but these notes are a Markdown file with no page numbers. The tester used section headings instead ("Revise 'Resistance'…"). The skill never says what to use when the notes have no pages. Minor gap; the fix is one sentence (e.g. "give the section name for Markdown/text notes, the page number for PDFs").
2. **A perfect follow-up answer still scores 0.5.** Step 5 does define this ("0.5 (partly correct after the follow-up)"), so it is not a contradiction — but a first-time reader could wonder whether answering the follow-up correctly should earn the full mark. The wording is clear enough once you read step 5, just easy to second-guess in the moment.
3. **"Answerable from the notes alone" vs formula inference.** Step 2 says each question must be answerable from the notes alone. Q2 ("by how much?") is only answerable by applying the formula R = ρL/A from the notes, not by quoting a sentence. The tester treated formula-based inference as in scope. That is a judgment call the skill does not spell out.

**Anything else the tester had to guess?** No. Question selection (different topics, recall + understanding mix, 5 questions, plain language), the verdict wording, the silent running tally, and the final format all worked exactly as written. The score arithmetic (1 + 0.5 + 1 + 0 + 0.5 = 3/5) follows step 5 directly.

---

## 4. Did the skill's stated flow actually happen?

| Stated flow | Happened? |
|---|---|
| Read notes first, list main topics | Yes — 3 topics listed before Q1 |
| Pick 5 questions, different topics, recall + understanding mix | Yes — Q1 recall (Ohm's law), Q2 understanding (resistance/length), Q3 recall (series), Q4 understanding (parallel), Q5 recall (power) |
| One question at a time, wait for the answer | Yes — sequential turns, no batching |
| Judge each answer immediately (correct / partly + follow-up / wrong + correct answer) | Yes — all three verdict types used, each within 2–3 lines |
| Keep score silently, announce only at the end | Yes — no score was mentioned until after Q5 |
| End with `Score: X/5`, one revision line per non-full-marks question, one encouraging line | Yes — Score: 3/5, three revision lines (Q2, Q4, Q5), encouraging line about the basics |
| Questions and answers only from the notes | Yes — every question and correct answer traces to the notes file; nothing was invented |

**Bottom line:** the skill works as written in a fresh session. It started correctly, asked one question at a time, and produced the score and revision pointer in its own format. The only improvements worth making are the two one-sentence clarifications above (section names instead of page numbers for non-PDF notes; confirming that a correct follow-up still scores 0.5).
