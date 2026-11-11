---
name: viva
description: Asks viva (oral-exam) questions from the user's notes, one question at a time, then scores the answers out of 5. Use when the user runs /viva with a notes file, or asks to be quizzed, viva-tested, or orally examined on their notes, a chapter, or a PDF.
---

# /viva — Viva questions from your notes

## When to run
Run this skill when the user gives a notes file (Markdown, text, or PDF) and asks for a viva, oral test, quiz, or mock viva on it — for example `/viva thermo-notes.pdf` or "quiz me on these notes".

## Input
The notes file. It is the only source of questions. If no file is given, ask for one before starting — do not quiz from general knowledge.

## Instructions

1. **Read the notes first.** Read the whole file and list its main topics (usually 3–6). Say briefly what you are about to do, e.g. "Reading notes. Asking 5 questions, one at a time." Do not start asking before you have read them.

2. **Pick 5 questions.** Choose 5 questions that:
   - cover different topics from the notes (not all from one page),
   - mix recall ("What is…?") with understanding ("Why…? / What happens if…?"),
   - can each be answered from the notes alone — never ask about something the notes do not cover.

3. **Ask one question at a time.** Ask Q1 and **stop and wait** for the answer. Never list all 5 questions up front, and never ask the next question before the user has answered the current one.

4. **Judge each answer immediately, then move on.** After each answer give a short verdict:
   - Correct: say so in one line and move on.
   - Partly correct: say what was right, then ask one short follow-up that points at the missing part (for example: "Partly. Friction lowers real engines, but what about an ideal one?").
   - Wrong or "I don't know": give the correct answer in one or two lines, note it as a point to revise, and move on.
   - Keep each verdict to 2–3 lines at most. Do not lecture.

5. **Keep score.** Score each question 1 (correct), 0.5 (partly correct after the follow-up), or 0 (wrong / not answered). If the follow-up is also wrong or not answered, the question scores 0 — a correct follow-up after a partial answer still scores 0.5. Keep a running tally silently; do not announce the score until the end.

6. **End with a score and a revision pointer.** After the fifth question, report:
   - `Score: X/5.`
   - One line per question you did not get full marks on, saying what to revise and where it is in the notes (e.g. "Revise page 14 — Carnot efficiency" for a PDF; for notes without page numbers, cite the section heading instead, e.g. "Revise §2 — Carnot efficiency").
   - One encouraging line about what was strongest.

## Rules
- Questions and correct answers must come **only from the notes file**. If the notes do not contain an answer, do not invent one — say the notes do not cover it.
- Never reveal the next question in advance.
- Never ask more than 5 questions in one viva unless the user asks for more.
- Use plain language. This is a viva, not a lecture.
- If the user answers in a different language, reply in that language.
