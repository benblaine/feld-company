# Build prompt 26 — Energy

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 26 — Energy

| | |
|---|---|
| Route | `/industries/energy` |
| Story | `Pages/Energy` |
| Section | Industries |
| Rail | 26 / 50 |
| Posture | Shift log |

## Copy

**Browser title:** Energy — Feld Company

**Meta description:** Shift logs and the outage desk for grid and generation operators. Sentences that a regulator may read. The log stays dull and exact.

**Eyebrow:** Industries · Energy

**Headline:** Write the sentence a regulator can read.

**Dek:** An outage desk does not need a more exciting voice. It needs a log that says what happened, in the order it happened, without a model smoothing the awkward half hour.

### The log

Operators already write. They write tired, at the end of a thing. An agent may propose the entry from the events the binding can see: the alarm, the switching step, the call to the neighboring control. The operator releases the entry. If the agent did not see it, the entry says it did not see it. Invention in a shift log is not a writing problem. It is an incident.

### The desk during the event

We do not install an agent into the middle of a live switching decision. The desk's loop, during the event, is escalation at most: a second reader on a prepared procedure, never a new instruction. After the event, the draft log is the work. Shadow week for this floor happens on quiet days and on drills, not because we want drama in the eval.

### Weather, in their sense and ours

A storm is their weather. A model release is ours. Both can land on the same Thursday. The engagement's weather plan says which work pauses when the grid is under stress. The answer is: the install pauses. Their weather outranks ours.

### Close

Bring a log entry you are proud of because it is plain. We will know the floor from that.

**Stamp:** Read the outage record
**Text link:** Plants, and the permit

## Layout

Posture: **Shift log.**

A log specimen of four timestamped lines, mono for the times, text face for the entries, on `--bg-sunken`, caption "Specimen entries. Composite. Deliberately plain."

Set exactly:

**04:12** Alarm received. Feeder east. No switching yet.
**04:18** Neighboring control informed. Name of the operator written by the operator, not proposed.
**04:41** Load transferred per procedure 12. The procedure was already open.
**05:02** Draft log offered. Released by the shift lead after one correction: the alarm was 04:11, not 04:12.

The correction in the last line is the point; set the corrected time in the same face, not in a highlight color. Accuracy is not a marketing callout.

Prose in a Measure around the specimen. No lightning bolts, no city-at-night hero, no green "sustainability" band.

Stamp `/records/outage`. Text link `/industries/plants`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/industries/energy`. Story: `Pages/Energy`, day, night, palm. Mast active: Industries. Rail 26 / 50. Crumb: Feld / Industries / Energy.

Posture: **Shift log**, per Layout. The four lines exact. Copy verbatim.

Stamp `/records/outage`. Text link `/industries/plants`.

Acceptance: times are tabular mono; the correction is readable without a color highlight; both ledgers; no storm photography; colophon; no hex.
