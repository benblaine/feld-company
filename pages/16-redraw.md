# 16 — Redraw

| | |
|---|---|
| Route | `/work/redraw` |
| Story | `Pages/Redraw` |
| Section | The Work |
| Rail | 16 / 50 |
| Posture | Two lanes |

## Copy

**Browser title:** Redraw — Feld Company

**Meta description:** Workflows reengineered so an agent has a job, a human has a judgment, and a wrong draft has a place to sit. The current path is not sacred, and it is not trash.

**Eyebrow:** Labor 04 · Redraw

**Headline:** Give the agent a job, not the whole path.

**Dek:** Reengineering a workflow is not a purification ritual. The current path contains superstition and it contains scars from real failures. A redraw keeps the scars, drops the superstition, and writes the agent's job in one sentence a handler can repeat.

### Lane one · As it is run

A file arrives in a pile. A person skims, opens the unofficial workbook to check a thing the system will not show, writes a note from scratch, asks a neighbor if the note "sounds right," and releases it under their name. The neighbor's check is invisible. The workbook is invisible. The time this takes is visible, and someone is measured on it.

### Lane two · As it will be run

A file arrives and is given a draft, or a refusal to draft. The refusal goes to the exception desk with a reason. The person reads the draft against the file, not against a blank page. They change what is wrong. They release under their name, and the attestation keeps both versions. The neighbor's check remains for the cases the eval calls unsure. The workbook is either brought into the binding, with an owner, or explicitly retired.

### The job sentence

Example, for a reserve note: "Prepare the note from the file and the prior ruling, list what you do not know, and never state a coverage that was ruled out."

If the job sentence needs a comma splice of every task on the floor, the redraw is greedy. Cut the process down. A second job is a second engagement, or a later season of this one.

### What usually gets dropped, and what must not

Dropped: retyping from one system into another, the blank page, the performance of thoroughness after the judgment is already made.

Kept: the release under a human name, the strange-file instinct, the hours when the record lies, any step a regulator or a harmed person would ask about later.

### Close

A redraw on one page, shown to the people who run the path, is the artifact. Their corrections are the rest of the artifact.

**Stamp:** Design the loop
**Text link:** Shadow week, when the lanes meet the files

## Layout

Posture: **Two lanes.**

A swimlane on desk. Two horizontal lanes stacked, each a full-width track with a left label rotated or set in a 120px stub: "As it is run" and "As it will be run". Inside each lane, the steps are text blocks separated by a 1px arrow (a simple line and chevron, not a library's cartoon arrow). Lane one has five steps drawn from its paragraph. Lane two has five steps drawn from its paragraph. Steps are `--bg-raised`, radius 0, hairline.

Above, headline and dek. Below the lanes, "The job sentence" is a pull-quote style plate, `--bg-sunken`, Newsreader, with the example sentence. Label it "An example job sentence" in mono so it is not mistaken for a universal slogan.

Then the kept/dropped section as two columns: Dropped, Kept. Brass tick for kept, a simple minus for dropped. Not a red cross.

Palm: each lane becomes a vertical list under its label. Arrow points down.

Stamp `/work/the-loop`. Text link `/shadow-week`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/work/redraw`. Story: `Pages/Redraw`, day, night, palm. Mast active: The Work. Rail 16 / 50. Crumb: Feld / The Work / Redraw.

Posture: **Two lanes**, per Layout. Derive the five step labels directly from the lane paragraphs, short noun phrases, and keep the full paragraphs as the section text above or inside an accessible description so nothing is lost. The visible steps may be condensed; the full prose must still appear on the page.

Copy otherwise verbatim. Stamp `/work/the-loop`. Text link `/shadow-week`.

Acceptance: two lanes distinguishable without color alone (labels); palm stacks; the example sentence is marked as an example; both ledgers; colophon; no hex; arrows are SVG using tokens.
