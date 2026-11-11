# Viva test run — Thermodynamics, WITHOUT a skill file

- **Notes used:** `sample-notes-thermodynamics.md`
- **Session type:** brand-new session, no SKILL.md read, no skill loaded. The assistant quizzed the student the way it naturally would.
- **Format note:** the interviewer asked one question at a time and waited for each answer before moving on. Student answers were played by the assistant with deliberately mixed ability (roughly 2 correct, 2 partial, 1 wrong), each labelled as it was given.

---

## Transcript

**Interviewer:** Let's start with something basic. What does the zeroth law of thermodynamics say, and why does it matter?

**Student:** The zeroth law says if two bodies are each in thermal equilibrium with a third body, then they're in thermal equilibrium with each other. It matters because that's what makes temperature a real, measurable thing — without it, thermometers wouldn't make sense.

**Interviewer:** Good, that's exactly right. Next one: the first law. Can you write down the formula and explain what each term means?

**Student:** The first law is about conservation of energy — energy can't be created or destroyed, it just changes form. The formula is ΔU = Q − W, where ΔU is the change in internal energy and Q is the heat added. W is the work done… I think W is the work done *on* the system? Or is it by the system? I always mix that up.

**Interviewer:** You're nearly there. W is the work done *by* the system — that's why it's subtracted. If the system does work on its surroundings, its internal energy drops. Keep that sign straight and you've got it. Okay, third question: what's the Carnot efficiency formula, and what could you change to make an engine more efficient?

**Student:** Efficiency is η = 1 − Tc / Th, and the temperatures have to be in kelvin, not Celsius. To make it more efficient you can raise the hot reservoir temperature Th, or lower the cold reservoir temperature Tc. Raising Th usually helps more in practice because Tc can't go below room temperature easily.

**Interviewer:** Spot on — formula, kelvin, and both levers. Nice. Fourth question: what is entropy, and can you give me the formula for the change in entropy?

**Student:** Entropy is a measure of disorder — like, how spread out the energy is. The more disordered a system is, the higher its entropy. The second law says entropy in an isolated system never decreases. As for a formula… I think it's something like ΔS = Q / T? I'm not sure about the exact conditions though.

**Interviewer:** That's mostly right. Entropy is disorder, or spread-out energy, yes. The formula is ΔS = Qrev / T — it only holds for a *reversible* process, and the Q has to be the reversible heat. For irreversible processes, total entropy just increases. Last one: what's the difference between an isothermal process and an adiabatic process?

**Student:** Isothermal means no heat exchange with the surroundings, and adiabatic means the temperature stays constant.

**Interviewer:** Hmm, no — you've got those swapped. Isothermal means constant temperature, and adiabatic means no heat exchange. That's a definitions question, so worth drilling. Okay, that's five — let me score you.

---

## Score

**3 / 5**

| # | Question | Verdict | Marks |
|---|----------|---------|-------|
| 1 | Zeroth law + why it matters | Correct | 1 |
| 2 | First law formula + terms | Partial — right formula and idea, wrong on the sign/meaning of W | 0.5 |
| 3 | Carnot efficiency + how to raise it | Correct | 1 |
| 4 | Entropy + ΔS formula | Partial — good definition, formula given without the reversibility condition | 0.5 |
| 5 | Isothermal vs adiabatic | Wrong — the two definitions were swapped | 0 |

## Revision guidance given

- **Drill the first-law sign convention.** You know ΔU = Q − W, but you hesitated on W. Remember it as: work the system *does* costs it internal energy, so it subtracts. Do a couple of quick numerical examples where the system expands and does work.
- **Entropy: attach the condition to the formula.** ΔS = Qrev / T only works for reversible processes. Practice saying the full sentence: "in a reversible process, the entropy change equals the reversible heat divided by temperature." And use the ice-melting example to explain why total entropy still rises in an irreversible process.
- **Isothermal vs adiabatic — learn them as a pair.** Isothermal = same temperature (iso = same, thermal = temperature). Adiabatic = no heat passes (the system is insulated). Make a two-column flashcard and test yourself until you can't swap them.
- You were solid on the zeroth law and Carnot — don't spend much more time there.

---

## How this session differed from a structured one

This is an honest record of what actually happened in the session, not what should have happened.

1. **Question pacing: one at a time, but not by rule.** I asked one question, waited for the answer, reacted, then asked the next. That happened because it's the natural conversational shape, not because a rule told me to — nothing in this session stopped me from dumping all five questions at once, and on a different day I might have. A skill would have to *specify* one-at-a-time (and specify what to do if the student answers several at once).
2. **Score: I gave a score out of 5, but I invented the marking.** Correct = 1, partial = 0.5, wrong = 0. That felt obvious to me, but nothing in the session defined it — no rule said partial answers get half marks, and no rule said what counts as "partial" versus "wrong" (Q2 vs Q5 was a judgement call). A skill would need to state the scoring scheme and the partial/wrong boundary explicitly.
3. **Feedback between questions: I corrected answers immediately.** After Q2, Q4 and Q5 I gave the right answer straight away before moving on. That helps learning, but it also means the student heard the correct answer mid-quiz — a skill would need to decide whether feedback is immediate or saved until the end, because those are different quiz designs.
4. **Revision guidance: I gave it, but in my own format.** The pointers above are a loose list of tips, ordered by how the mistakes came up, not by topic or priority. There was no fixed structure like "one pointer per missed question" or "revise X first". A skill would need to fix the format — e.g. score first, then one revision pointer per question scored under full marks, in priority order.
5. **Question selection: I picked what felt like the core ideas.** I chose the zeroth law, first law, Carnot, entropy and isothermal/adiabatic because they cover the four sections of the notes. But nothing forced coverage of all four sections — I could easily have asked three questions about the laws and skipped entropy entirely. A skill would need a coverage rule (e.g. at least one question per section of the notes).
6. **No verification of the answers against the notes.** I judged answers from the notes' content as I remembered them, but I never re-checked a borderline answer (Q4's "ΔS = Q / T") against the file mid-session. A skill would need to say: check each answer against the notes before marking it.
7. **Tone and length were unregulated.** The session reads like a friendly tutor chat — short reactions, a bit of praise, casual phrasing. Nothing constrained how long questions, hints or feedback could be. A skill that wants a consistent viva experience would need to pin down tone and how much help the interviewer gives before marking an answer wrong.
