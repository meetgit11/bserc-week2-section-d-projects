# prompts.md — Same Page, New Design (BSERC Week 2, Section D)

Prompts used, in order, as required by the Week 2 PDF.

## 1. Parent agent → builder (5 Nov 2026)
> Build BSERC Week 2 Section D Project 17, "Same Page, New Design": Step 1 without a design skill — build a simple plain page for a college fest (TECHNOVA 2026, as in the PDF preview) as before.html, containing the exact words/content blocks from the PDF preview (TECHNOVA 2026; "Three days of robotics, code and music."; "Robotics · Hackathon · Music night"; "Register now"; Chai and Co. strip; Bright Path Classes strip). Step 2 — write a design skill file design-skill.md (SKILL.md shape: critique first, then fix biggest problems one at a time); do NOT claim it is the "Impeccable" skill unless actually installed — this is your own written design skill, labelled as such. Step 3 — redesign the same page using that skill as after.html, words matching exactly, responsive on a phone. Deliver README.md (3+ design changes with reasons), prompts.md, test-checklist.md. Verify text identity with a script, no external references, and report what remains unverified.

Result: `before.html` (plain, PDF's words in PDF order); `design-skill.md` (own skill `page-redesign`, labelled as written, not installed); `after.html` (hero + cards, same words).

## 2. Builder → itself (5 Nov 2026, text-match fix)
> First text-extraction diff failed: the words were the same but in a different order — in after.html the menu line came before the action link in each card, while before.html (following the PDF preview) has the link first. "Words match" means order too.

Result: reordered `after.html` so each card follows the before.html order (lede → link → menu), and re-ran the diff — visible text now identical (63 words, same order, body text identical).
