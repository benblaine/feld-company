# Build prompt 29 — Civic institutions

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 29 — Civic institutions

| | |
|---|---|
| Route | `/industries/civic` |
| Story | `Pages/Civic` |
| Section | Industries |
| Rail | 29 / 50 |
| Posture | Case jacket |

## Copy

**Browser title:** Civic institutions — Feld Company

**Meta description:** Benefits intake and the case note. The applicant can see why. An agent may draft. A person releases. Appeal stays intact.

**Eyebrow:** Industries · Civic

**Headline:** The applicant can see why.

**Dek:** A public institution's queue is made of people who did not choose to be in it. The install is judged by whether those people can understand the decision, appeal it, and be spoken to in the language they already use.

### The jacket

A case jacket gathers documents, prior decisions, and the rule that applies. An agent may draft that gathering and a case note in the institution's plain style. A caseworker releases the note. The note distinguishes what the applicant said, what the document said, and what the rule did. Those three are never blended into a smooth paragraph.

### The reason

If a decision is adverse, the reason is a required artifact, written so a person without a lawyer can follow it, and pointing at the appeal that already exists in law and policy. The agent may draft the reason from the rule and the file. It may not invent a rule. It may not omit the appeal because the letter reads more cleanly without it. The eval's refusal cases include a missing appeal line. That case pauses the queue.

### Language and access

The interface a caseworker uses, and any letter the applicant receives, meet the accessibility floor of the institution and then the floor of this design system, whichever asks more. Languages are the institution's duty, not a phase two. If we cannot support the letter in the languages the desk already serves, we do not send the letter.

### What we decline

Scoring a person's risk as a character. Predicting fraud as a label the applicant cannot see. Anything that shortens a legally required wait by skipping a legally required step. Speed is not the highest good on this floor.

### Close

Begin with the adverse letter you already send. If it is unclear, the install starts by rewriting it with the people who receive it.

**Stamp:** Read the benefits record
**Text link:** Health systems, the neighboring duty

## Layout

Posture: **Case jacket.**

A jacket specimen: a folder-like plate (radius 0, double hairline) titled "Case jacket · specimen" containing three labeled blocks, stacked: "What they said", "What the document said", "What the rule did". Each block has one sentence:

- They asked for the support on the 2nd, in the form's own words.
- The wage document covers March, and does not cover April.
- The rule requires April. The gap is the reason. The appeal is listed under it.

Caption: "Composite. An adverse reason that still shows the appeal."

Prose in a letter measure, serious, no jokes, no patriotic decoration, no stock photo of a flag or a queue of people.

Stamp `/records/benefits`. Text link `/industries/health-systems`.

The page itself must be exemplary of the accessibility claims: headings in order, contrast tokens, link underlines, the specimen not an image of text.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/industries/civic`. Story: `Pages/Civic`, day, night, palm. Mast active: Industries. Rail 29 / 50. Crumb: Feld / Industries / Civic.

Posture: **Case jacket**, per Layout. Three blocks exact. Copy verbatim, including every refusal. No jokes in the UI. No imagery of claimants.

Stamp `/records/benefits`. Text link `/industries/health-systems`.

Acceptance: the appeal is visible inside the specimen; the three sources are separate blocks; both ledgers; page is text, not a picture of text; colophon; no hex; focus states intact.
