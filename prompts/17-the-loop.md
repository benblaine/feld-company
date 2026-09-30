# Build prompt 17 — The Loop

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 17 — The Loop

| | |
|---|---|
| Route | `/work/the-loop` |
| Story | `Pages/Loop` |
| Section | The Work |
| Rail | 17 / 50 |
| Posture | Five loops |

## Copy

**Browser title:** The Loop — Feld Company

**Meta description:** Human-in-the-loop, designed per process: release, review, exception, escalation, and night. Each pattern names a person and a thing that never proceeds alone.

**Eyebrow:** Labor 05 · The Loop

**Headline:** Name the human. Name the hour.

**Dek:** "Human in the loop" is not a pattern. It is five patterns, and a process usually needs one of them as its spine plus a rule for night. Choose as if you will be the person woken.

### Release

The agent drafts. A named person releases under their own name, or sends the draft back. Nothing leaves unattended. This is the default for anything a customer, a patient-adjacent file, a citizen, or a regulator might later read.

**Night:** the queue waits. It does not get creative at 2am.

### Review

The agent drafts and a person reviews a sample, not every file, against an eval that has earned the thinning. The sample rate is written down. The right to return to full release is written down. Review is a privilege a process grows into, not a shortcut on day one.

**Night:** sampling pauses. Full release resumes until morning, or the queue waits. Pick one and write it.

### Exception

The agent handles the ordinary file end to end, and refuses the rest into a desk owned by a person. "Ordinary" is defined by the eval, not by the agent's confidence in the moment. A confident wrong file is how exception patterns rot.

**Night:** refusals pile up for morning unless the exception desk is a true shift. If it is a true shift, staff it like one.

### Escalation

A person does the work. The agent is a second reader, called when the file matches a pattern the floor has already decided is dangerous, expensive, or merely odd. Escalation is how a floor begins when trust is low, and there is no shame in staying here.

**Night:** the person on shift keeps the authority they have by day. The agent does not gain courage after dark.

### The never list

Every loop card ends with sentences of refusal. The agent does not close a permit. The agent does not practice medicine. The agent does not deny a benefit without a reason a person can appeal. The agent does not invent a coverage. Copy the sentences that fit. Write the ones that are yours.

### Close

A loop card with blank names is a draft of a draft. Bring the names.

**Stamp:** See a loop card in the wild
**Text link:** Living evals, which keep the loop honest

## Layout

Posture: **Five loops.**

A control at the top: five radio buttons in a fieldset, legend "Choose the loop." Options: Release, Review, Exception, Escalation, and a fifth radio "Night, across all of them" which reveals only the night sentences stacked. Default selection is Release.

The selected pattern's prose replaces a panel below the radios, with the heading and the night line. Use a live region so the change is announced: "Showing release." The never list and the close stay outside the swap and are always visible.

Radios are the Field component, laid out horizontally on desk and vertically on palm, 40px targets.

Do not illustrate loops as circular arrows with a human icon. The word is enough. Helen Cho's practice is seriousness, not a diagram of a lasso.

Stamp links to `/records/claims` (a loop card in the wild). Text link `/work/evals`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/work/the-loop`. Story: `Pages/Loop`, day, night, palm, and a story per selected radio (five). Mast active: The Work. Rail 17 / 50. Crumb: Feld / The Work / The Loop.

Posture: **Five loops**, per Layout. Fieldset and radios from the library. Copy verbatim, each pattern shown only when selected, never-list always present. Live region announces the visible pattern.

Stamp `/records/claims`. Text link `/work/evals`.

Acceptance: keyboard can move between radios and the panel updates; the announcement fires; no content is reachable only by mouse; both ledgers; the never-list is present in every story; colophon; no hex.
