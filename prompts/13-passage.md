# Build prompt 13 — Passage

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 13 — Passage

| | |
|---|---|
| Route | `/work/passage` |
| Story | `Pages/Passage` |
| Section | The Work |
| Rail | 13 / 50 |
| Posture | Batch window |

## Copy

**Browser title:** Passage — Feld Company

**Meta description:** Legacy systems, lifted into reach so an agent can meet the work. The cloud move is the means. The batch window, the terminal, and the forbidden hours are the design.

**Eyebrow:** Labor 01 · Passage

**Headline:** Lift the old system into reach.

**Dek:** An agent cannot do work it cannot see. Passage is the labor of moving a system of record into a place the agent can use, without pretending the screen where people still work has ceased to exist.

### What passage is for

Somewhere in the company, the file of truth still lives behind a terminal, a nightly batch, a vendor who delivers extracts on Tuesdays, or a client-server application with one remaining operator. The cloud program may already be "done." The work is not in reach until an agent can read the record it is accountable for, during the hours the floor is allowed to touch it.

Passage is finished when that path exists, the forbidden hours are written down, and a human can explain the path without the pod in the room.

### The batch window

Treat the timetable as part of the system, because it is.

| Window | What is true |
|---|---|
| 02:00–04:30 | Night batch. The record is a liar if you read it. Agents do not write. They barely read. |
| 04:30–06:00 | Extract settles. A thin read is allowed. No release. |
| 06:00–18:00 | Floor hours. Read is allowed. Draft is allowed. Release follows the loop card, not the network diagram. |
| Quarter-end freeze | Named by Finance, often longer than they first said. Passage respects it even when the pilot does not want to. |
| Vendor Tuesday | The extract from the outside party arrives late more often than the interface agreement admits. The map says so. |

These hours are an illustration, the kind of artifact a pod leaves on the table. Your hours will be different. A passage that does not produce a table like this is unfinished.

### What we will not call passage

A database that moved, while the operators remained on a screen the agent will scrape. A scrape, offered cheerfully as a bridge, with no date to take it out. A full estate migration that must complete before any process can begin. Passage is cut to the process we were hired into. The rest of the estate can stay ugly for now.

### Close

If your system of record is already in reach, skip to access. If you are not sure, you are in passage.

**Stamp:** The access design
**Text link:** Begin with this labor

## Layout

Posture: **Batch window.**

Headline and dek, then the first section in a Measure.

The timetable is a real Ledger table, caption "An illustrated batch window. Not a client's." Sortable is unnecessary; do not add sort chrome for decoration. Numerals and times in mono. The row "Night batch" carries a status word "Closed" in oxide plus text. "Floor hours" carries "Open" in patina plus text. Status is a disc and a word.

Under the table, a mono line: "Times in the floor's own zone. Write the zone on the artifact."

Then the remaining prose. Close stamps: primary to `/work/access`, text link to `/begin`.

A thin SVG timeline under the table is optional and must match the rows, not add new facts. Prefer the table alone if the timeline would repeat it. Choose the table alone.

Palm: the table scrolls inside a sunken frame. First column sticky.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/work/passage`. Story: `Pages/Passage`, day, night, palm. Mast active: The Work. Rail 13 / 50. Crumb: Feld / The Work / Passage.

Posture: **Batch window**, per Layout. Use the Ledger component even without sorting. Caption required. Copy verbatim. Status cells for Closed and Open use disc plus word.

Stamp `/work/access`. Text link `/begin`.

Acceptance: table has a caption and a scrolling frame at 390px; times are tabular mono; night ledger restyles the table via tokens; empty and loading states are not shown on this page (they belong to the component's own stories); colophon; no hex.
