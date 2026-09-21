# Contributing Guide

Thank you for helping improve **Automate Your Business with AI**. This guide explains how to write for this book so every chapter feels clear, deep, and consistent. Please read it fully before you write or edit.

## 1. The golden rule: write for non-technicians

This is **not** a book for engineers. It is for business owners, managers, and professionals with no technical background.

- Use **simple, plain, international English**. Avoid slang, idioms, and culture-specific references that do not travel well.
- Prefer **short sentences**. One idea per sentence.
- When you must use a technical term, **explain it the first time** in plain words, then use it freely.
- Use **everyday analogies** (a recipe, a filing cabinet, a traffic light) to make abstract ideas concrete.
- Never assume the reader knows what a "model", "API", or "neural network" is. Define it simply.

If a smart non-technical reader could get stuck on a sentence, rewrite that sentence.

## 2. Depth: a real chapter, not a quick guide

Every chapter must be **thorough and complete**. This is not a blog post or a summary.

- A typical regular chapter runs **2,500–3,500 words**. This is an **indicative** range, **not a hard limit**. It exists so a first draft lands at a sensible size, not to cap the content.
- **The current book is a first pass (a draft).** Chapters may go **over** this range freely when new material genuinely adds value. Do not cut useful content just to hit a number, and do not pad to reach one.
- Every sub-part listed in the chapter outline must be covered **fully**, in its own subsection (use `###`).
- Give the reader enough to **act**, not just to nod along.
- "How to Do It" sections must contain real, ordered steps a reader can follow.

A chapter that only scratches the surface is not finished.

## 3. No repetition, no redundancy

This is the most common way a multi-author book loses quality. Follow these rules strictly.

- **Say each thing once.** Do not repeat the same explanation in two chapters.
- **Every anecdote, case study, and example has ONE canonical home.** Elsewhere, link to it with a single sentence, for example: *"We covered the Eliza effect in [Chapter 1](ch01-a-short-history-of-ai.md)."*
- **Every concept has one owner chapter.** If you need a concept owned by another chapter, link to it — do not re-explain it.
- Avoid restating the same idea with different words inside the same section.
- Do not pad. If a section is short because the topic is small, that is fine. Do not stretch it.

### Canonical home map (do not duplicate)

Each recurring topic lives in **one** chapter. Other chapters link to it.

| Topic | Canonical home |
|-------|----------------|
| Turing, "can machines think?" | Ch 1 |
| Dartmouth 1956, the term "AI" | Ch 1 |
| ELIZA and the Eliza effect | Ch 1 |
| AI winters | Ch 1 |
| Deep Blue (1997), Watson (2011) | Ch 1 |
| "AI panics when Pokémon die" | Ch 1 |
| Seoul taxi driver who taught AI not to lie | Ch 2 |
| Model trained on 1930s data that wrote Python | Ch 3 |
| 4 pillars of ethical governance, 6 principles of responsible adoption | Ch 4 |
| Bias, transparency, explainability, human responsibility | Ch 4 |
| EU AI Act (obligations, prohibited practices, high-risk, transparency) | Ch 5 |
| GDPR (principles, consent, rights, DPIA, anonymization, EDPB opinion) | Ch 10 |
| Prompt injection, data poisoning, inversion attacks, supply-chain risk | Ch 6 |
| Trustless, verifiable trust, agent-to-agent | Ch 7 |
| Self-hosting, Ollama, local models | Ch 8 |
| Third-party services, lock-in, shadow AI, ChatGPT data-exposure cases | Ch 9 |
| Digital sovereignty, open source vs proprietary | Ch 11 |
| Impact / ease matrix | Ch 12 |
| ROI method | Ch 16 |
| "Headcount Zero" book | Ch 17 |
| Elanco (procure-to-pay, ~99% time cut) | Ch 25 |
| mobilezone (two Copilot agents) | Ch 26 |
| TridentCare (96% planning automation) | Ch 27 |
| SOK Finance (multi-agent finance) | Ch 29 |
| IBM (vendor risk, ~50% time cut) | Ch 30 |

When you reference a topic owned elsewhere, write one linking sentence and move on.

## 4. Fixed chapter structure

Every regular chapter uses these exact H2 headings, in this order:

```markdown
# Chapter N — <Title>

## In Simple Words
## A Bit of History
## Curiosity
## A Real Business Example
## How to Do It
## Ethics and Responsibility
## Mistakes to Avoid
## Practical Exercise
## Checklist
## Key Takeaways
```

- Use `###` for the sub-parts inside each section.
- **Key Takeaways** = 3–5 bullet points, each a single clear sentence.
- **Checklist** = a list of checkboxes (`- [ ]`) the reader can act on.
- **Practical Exercise** = one concrete task the reader does for their own business.

Sector case-study chapters (31–36) use a different fixed structure:

```markdown
# Chapter N — <Sector>

## Context
## The Problem
## The Solution
## The Tools
## The Costs
## The Results
## Lessons Learned
```

## 5. File naming and location

- All chapter files live in `books/EN/`.
- Name them `chNN-short-slug.md` (two-digit number, kebab-case slug), for example `ch12-where-ai-can-help-your-business.md`.
- Appendices are `appendix-<letter>-<slug>.md`, for example `appendix-a-glossary.md`.
- Start each file with a single H1 title. Do **not** add YAML front matter.

## 6. Style details

- Use GitHub-flavored Markdown.
- Use tables for comparisons and checklists where they help.
- Numbers: write figures plainly ("about 90%", "3 hours a week").
- British or American spelling: pick one and stay consistent within a chapter; the book currently uses American spelling.
- No emoji in body text.
- Links between chapters use relative paths (same folder), e.g. `[Chapter 10](ch10-privacy-and-gdpr.md)`.

## 7. Accuracy and sources

- Do not invent statistics, quotes, or company results. If you cite a number, it must come from a real, checkable source.
- When a figure is approximate or illustrative, say so plainly ("a typical small team might save...").
- Legal content (GDPR, EU AI Act) must reflect the actual rules. If unsure, flag it rather than guess.

## 8. Adding or changing a chapter

1. Check the canonical home map so you do not duplicate an existing topic.
2. Draft the chapter with the fixed structure and full depth.
3. Run the self-review checklist below.
4. Open a pull request and note which chapters you touched and why.

### Self-review checklist before you submit

- [ ] Written in simple, plain, international English
- [ ] Every technical term explained on first use
- [ ] Fixed section structure present and complete
- [ ] Every outline sub-part covered in full
- [ ] No content duplicated from another chapter (linked instead)
- [ ] No padding or filler
- [ ] All numbers and claims are real and checkable
- [ ] Key Takeaways are 3–5 clear points
- [ ] Checklist uses `- [ ]` items
- [ ] File named and placed correctly

Thank you for keeping this book clear, honest, and useful.
