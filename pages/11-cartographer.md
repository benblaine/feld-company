# 11 — Cartographer

| | |
|---|---|
| Route | `/careers/cartographer` |
| Story | `Pages/RoleMap` |
| Section | Firm |
| Rail | 11 / 50 |
| Posture | Before the ink |

## Copy

**Browser title:** Cartographer — Feld Company

**Meta description:** The seat that draws the process, including the unofficial one, before an agent is proposed. Interviews the exception-keeper, not only the sponsor.

**Eyebrow:** Roles · Seat 03

**Headline:** Cartographer.

**Dek:** You draw the process while it is still only theirs. Nothing is proposed until the map has survived contact with the person who knows the exceptions.

### What the map has to contain

The official path, in the company's own names for the steps. The unofficial path: the inbox, the workbook, the call someone makes "just to check." The hours the path is forbidden, including the batch window and the freeze before quarter-end. The name of the person who releases, and the name of the person who actually notices when a file is strange. Those are often different people.

A map that came from the process document alone is a clean picture of a place you have not visited. We do not hang those.

### How you spend the first days

You sit. You ask to see the last file that went badly, and the last file that went well for an uninteresting reason. You read the queue's real name, which is sometimes an insult, and you put that name on the map in quotes. You notice incentives: who is measured on speed, who is measured on not being the one who released a mistake.

You write marginalia. An unmarked map is unfinished, because the doubt is part of the data.

### What you bring

You have made a workflow visible to the people who run it, and they recognized themselves, including the parts they were not proud of. You can draw. More important, you can throw a drawing away in front of its subject and start again without defending the hour you spent.

You are allowed to be untechnical. You are not allowed to be uninterested in the binding, because a map that cannot be implemented is a poster. Samir will sit with you. You do not have to become Samir.

### Close

In the letter, describe a process you mapped that turned out to be two processes wearing one name.

**Stamp:** Write to the firm
**Text link:** See redraw, where maps go to be changed

## Layout

Posture: **Before the ink.**

Split gather. Left, span 6: an inline SVG engraving of a map that is deliberately incomplete. A main path of five square nodes labeled with invented-generic step names from the copy's spirit: Intake, Check, Draft, Release, File. A dashed unofficial path from Check to a node labeled "The workbook". A node labeled "Strange file" off to the side, connected with a brass line. Marginalia in mono, rotated 0 degrees, small: "Name in quotes. Confirm with R." One node has no label, only a question mark, to show the map is unfinished. Strokes 1px, currentColor, the brass line in `var(--tick)`, no fill.

Right, span 6: the dek and the first section.

Then full-width Measures for the remaining sections. The SVG has a title and a description for assistive tech: "An unfinished map: official path, a side workbook, and an unlabeled step."

Palm: drawing first, capped at 280px tall, then text.

Do not use a stock illustration of a treasure map. No compass rose. No parchment texture.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/careers/cartographer`. Story: `Pages/RoleMap`, day, night, palm. Mast active: Firm. Rail 11 / 50. Crumb: Feld / Firm / Careers / Cartographer.

Posture: **Before the ink**, per Layout. The drawing is inline SVG using tokens, with a title and desc. Copy verbatim.

Stamp `/begin`. Text link `/work/redraw`.

Acceptance: the unlabeled node is visibly unlabeled; the unofficial path is dashed; night mode inherits currentColor so the map does not vanish or stay brown-on-brown; reduced motion has no drawing animation (it is static); colophon; no hex in the SVG (use `var(--fg)`, `var(--tick)`, `var(--line-strong)`).
