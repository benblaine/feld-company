# Build prompt 25 — Plants

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 25 — Plants

| | |
|---|---|
| Route | `/industries/plants` |
| Story | `Pages/Plants` |
| Section | Industries |
| Rail | 25 / 50 |
| Posture | Permit |

## Copy

**Browser title:** Plants — Feld Company

**Meta description:** Maintenance work orders and the permit to work. Tribal knowledge made legible. The agent does not close a permit.

**Eyebrow:** Industries · Plants

**Headline:** The permit stays a human act.

**Dek:** Plants run on work orders, on the knowledge inside people who are about to retire, and on permits that exist because someone was hurt before. We will touch the first two. We will not automate the closing of the third.

### The work order

A maintenance order gathers what is wrong, what was done last time, which parts the stores actually hold, and which machine is downstream of this one. An agent can draft that gathering from the system of record and from the notes the access design allows. A supervisor releases the order. The technician remains the person who says what they found, in their own words, after the job. We do not overwrite their finding with a cleaner paragraph.

### The knowledge that is about to leave

Some of the map lives in a person, not in the CMMS. Cartography sits with them before any binding. What they allow to be written down is a Train permission, in the sense of the access page: their judgment as example, asked for, not scraped from a career of notes they never offered. If they do not want a story used, it is not used. The install can be slower. It will be truer.

### The permit

The agent may assemble the permit pack: isolations, the last time this was done, the names the procedure asks for. The agent does not decide the isolation is sufficient. The agent does not close the permit. The agent does not nudge a signer. A pod that treats this as negotiable is a pod we will not field.

### Close

Bring one work order that went long for a reason the system did not contain. That reason is the start of the map.

**Stamp:** Begin from the plant
**Text link:** Energy, where the sentence meets a regulator

## Layout

Posture: **Permit.**

The permit is a visual object: a plate the width of the measure, hairline double rule (two hairlines, 3px apart) like a form's edge. Inside, mono fields with blank underscores and filled examples:

Permit no. — specimen
Asset — line 2 pump, illustrative
Assembled by — agent, pack only
Isolation sufficient — a blank line, labeled "a person writes this"
Closed by — a blank line, and the sentence "Not an agent." in `--fg`

The plate sits after the permit section's prose, as a figure with caption "Specimen. The blanks are the point."

The rest is a Measure. No hard-hat stock. No factory spark shower photograph. An engraving of a simple pump outline is allowed only if it adds nothing cute; prefer no illustration beyond the form.

Stamp `/begin`. Text link `/industries/energy`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/industries/plants`. Story: `Pages/Plants`, day, night, palm. Mast active: Industries. Rail 25 / 50. Crumb: Feld / Industries / Plants.

Posture: **Permit**, per Layout. The specimen form's blanks are real text, not input fields (this is not a form to submit). Copy verbatim. The prohibition on closing a permit is prominent.

Stamp `/begin`. Text link `/industries/energy`.

Acceptance: "Not an agent." is visible on the specimen; the figure has a caption; both ledgers; no industrial-hero photography; colophon; no hex.
