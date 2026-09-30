# 14 — Access

| | |
|---|---|
| Route | `/work/access` |
| Story | `Pages/Access` |
| Section | The Work |
| Rail | 14 / 50 |
| Posture | Four keys |

## Copy

**Browser title:** Access — Feld Company

**Meta description:** Data organization and access, redesigned as four permissions: read, draft, release, train. Names in the boxes, not departments.

**Eyebrow:** Labor 02 · Access

**Headline:** Four permissions, with names in them.

**Dek:** The conjecture asks for data organization and access to be updated. In practice that means a person can answer four questions about a given process, and the answers are names.

### The four keys

**Read.** Who may see the file. Includes the agent, which is not a vague "the system." An agent that can read is a principal in this list, with a scope written in one sentence.

**Draft.** Who may prepare work that is not yet the record. Often the agent, and sometimes a junior person. Draft is allowed to be wrong in a way release is not.

**Release.** Who may let the draft become the record, or leave the building. A name. A deputy for leave and for night. If the honest answer is "the team," the access design is not finished.

**Train.** Who may have their work kept as an example for the next month's eval or for a finer binding. This is the permission companies forget, and the one their people feel. Training on a person's judgment is a use of that person. Ask.

### The middle of the building

Shared inboxes. A drive of spreadsheets, one of them called final, one of them called final_v7, both current. A personal folder that is, operationally, the control. Access work that tidies the lake and never touches these is a public garden beside an unmoved house.

We inventory the unofficial stores for this process only. We say which of them the agent may read. We say which of them must be closed, and who is affected, before we close them. Surprise is not a control.

### Organization, meant plainly

Records need descriptions a stranger can use: what a field means, which value is stale, which duplicate is the survivor. A catalog entry of ten lines beats a platform with a vision. The entry names the owner of the description, because descriptions rot the way evals rot.

### Close

Bring the four names to the first meeting. If you do not know the release name, that is the meeting.

**Stamp:** Bind the software
**Text link:** Begin with access

## Layout

Posture: **Four keys.**

Four full-width rows, stacked, each a horizontal plate. Left: a large mono index 01–04 and the key name in display h2 (Read, Draft, Release, Train). Right: the paragraph, measure about 50ch. A key icon from the system, 1.5px stroke, at the far left. Hairline between rows. The Release row uses `--bg-raised` so the eye lands on the name that matters most. Do not color the rows green/yellow/red.

Below the rows, two prose Measures: "The middle of the building" and "Organization."

No padlock photography. No matrix of checkmarks across a fake org chart.

Stamp `/work/bindings`. Text link `/begin`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/work/access`. Story: `Pages/Access`, day, night, palm. Mast active: The Work. Rail 14 / 50. Crumb: Feld / The Work / Access.

Posture: **Four keys**, per Layout. Copy verbatim. Release row is the raised surface. Icons are the key icon, `aria-hidden`, with the heading carrying the name.

Stamp `/work/bindings`. Text link `/begin`.

Acceptance: the four keys are in source order; palm stacks label above paragraph inside each row; night raised surface is night-2; the word Train is not omitted; colophon; no hex.
