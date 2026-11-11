---
name: page-redesign
description: Redesigns a plain web page with the same words — critique first, then fix the biggest problems one at a time (hierarchy, spacing, colour, typography, mobile layout). Use when the user asks to redesign, restyle, or improve the look of an existing page without changing its text.
---

# Page Redesign — a small design skill

> **This is my own written design skill** (BSERC Week 2, Section D, Project 17). It is **not** the "Impeccable" skill from skills.sh and it was not installed from anywhere — it was written for this project, following the PDF's hint to critique first, then fix the biggest problems one at a time.

## When to run
Run this skill when the user gives you a page (an HTML file) and asks you to redesign it, make it look better, or apply a design skill to it — while keeping the words the same.

## Instructions

1. **Critique first, before changing anything.** Read the page and write a short critique naming the biggest problems, in this order:
   - **Hierarchy:** can a visitor tell in 3 seconds what the page is about and what to do next? Is there one clear headline and one clear action, or do all the lines shout at the same volume?
   - **Spacing and grouping:** are related things grouped together, and unrelated things separated? Or is everything one long undifferentiated list?
   - **Colour:** is there a deliberate palette (one dark, one light, one accent), or is everything black-on-white with default blue links?
   - **Typography:** is there a clear scale (big headline, medium sub-headings, readable body), or is everything roughly the same size?
   - **Mobile layout:** does anything overflow, or squeeze, on a 360 px wide phone screen?

2. **Fix the biggest problems one at a time, in this order:** hierarchy → spacing/grouping → colour → typography → mobile layout. Do one, check it, then do the next. Do not try to fix everything in a single pass.

3. **Keep the words identical.** Do not add, remove, or reword any visible text. You may change markup, classes, and CSS — never the words. (Splitting a line into spans for layout is allowed only if the visible text, in order, stays exactly the same.)

4. **Make it work on a phone.** Use a viewport meta tag, a fluid layout (`max-width` + `width: 100%`), `box-sizing: border-box`, and a media query that stacks multi-column rows into one column below ~640 px. Nothing may overflow horizontally at 360 px wide.

5. **Stay offline.** Use system font stacks only. No external fonts, images, scripts, or stylesheets.

## After the redesign
Report the changes as a short list, one line per change, each with **why** it helps (for example: "Grouped the fest details into a hero card, so a visitor sees what the event is and what to do next in one glance"). Then verify: extract the visible text of the old and new pages and confirm it is identical, and confirm there are no external references.
