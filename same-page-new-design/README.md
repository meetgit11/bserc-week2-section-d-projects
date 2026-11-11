# Same Page, New Design

BSERC GenAI Internship · Week 2 · Section D · Project 17 (Medium)

## What it is

The same page, built twice with the **exact same words**: once plain, without any design skill (`before.html`), then redesigned with a design skill (`after.html`). The page is for a college fest, **TECHNOVA 2026**, with a café strip (Chai and Co.) and a coaching strip (Bright Path Classes) — the content from the PDF preview.

## Files

| File | What it is |
|---|---|
| `before.html` | Step 1 — plain page, no design skill. Stacked headings, default blue links, no layout. |
| `design-skill.md` | Step 2 — **my own written design skill** (`page-redesign`). It is **not** the "Impeccable" skill from skills.sh and was not installed from anywhere; it is written for this project in SKILL.md shape (critique first, then fix the biggest problems one at a time). |
| `after.html` | Step 3 — the same page, redesigned using that skill. Same words, new design. |
| `test-checklist.md` | PDF Done-when checks with evidence. |
| `prompts.md` | Prompts used, in order. |

## How to view

Open `before.html` and `after.html` in a browser (double-click, or serve the folder). No internet needed — system fonts only, no external files. Open `after.html` on a phone, or shrink the browser window below 640 px, to see the mobile layout.

## Critique of `before.html` (step 1 of the skill, applied before redesigning)

1. **Hierarchy:** everything is the same size and weight, so nothing tells you what the page is about or what to do next in the first 3 seconds.
2. **Spacing / grouping:** all three blocks (fest, café, coaching) run into one long list separated only by thin rules — nothing groups related things together.
3. **Colour:** black on white with default blue links — no palette, no mood, no difference between the fest and the two businesses.
4. **Typography:** one size for headings, one for body, no scale — the fest name looks no more important than a menu line.
5. **Mobile layout:** it happens to fit a phone only because it is one plain column; there is no deliberate mobile design.

## Design changes in `after.html` — and why each one helps

1. **A hero section with one headline and one action.** The fest name is now a large, bold headline on a dark gradient, with the tagline under it and a single amber "Register now" button. *Why: a visitor understands what the event is and what to do next in one glance, instead of reading a list to find the action.*
2. **Content grouped into cards.** The fest, the café, and the coaching institute are now separate, clearly bounded groups — a hero card for the fest, two cards side by side below it. *Why: grouping tells the eye which lines belong together; the page stops being one undifferentiated list and becomes three scannable blocks.*
3. **A deliberate colour palette.** Dark navy hero, warm amber accent for the café card's top edge and the main button, teal for the coaching card. *Why: colour separates the three blocks at a glance and gives the page a mood; the amber button draws the eye to the one action that matters most.*
4. **A real type scale.** Headline ~3.4 rem, card headings 1.45 rem, body ~1 rem, menu lines bold at 0.98 rem. *Why: size now signals importance — the fest name is unmistakably the most important line, and prices are readable without competing with it.*
5. **A deliberate mobile layout.** Below 640 px the two cards stack into one column, the hero padding shrinks, and the headline scales with `clamp()`. *Why: on a phone the page stays readable with no horizontal scrolling, instead of relying on the accident that a plain list happens to fit.*

## Verification (summary — see `test-checklist.md`)

- Visible text of `before.html` and `after.html` is **identical** (63 words, same order) — verified by a strip-tags-and-compare script.
- Both files are offline: zero external references, no JavaScript at all.
- Mobile layout: viewport meta + 640 px media query + fluid widths verified by inspection. **Still to verify on a real phone** — open `after.html` on the user's phone and confirm no horizontal overflow (no browser in this VM to render it).

## Limits (honest)

- The design skill is my own written file, not the "Impeccable" skill from skills.sh named in the PDF — the PDF allows other skills, and this one is labelled as written, not installed.
- The links (`Register now`, etc.) are placeholders (`href="#"`) — the page is a design exercise, not a live fest site.
- The phone check is inspection-based here; the real-phone check is the user's to do.
