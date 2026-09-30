# 15 — Bindings

| | |
|---|---|
| Route | `/work/bindings` |
| Story | `Pages/Bindings` |
| Section | The Work |
| Rail | 15 / 50 |
| Posture | Parts catalog |

## Copy

**Browser title:** Bindings — Feld Company

**Meta description:** Connecting the software a company already runs to agents. A catalog of the system of record, the system of use, and the unofficial system.

**Eyebrow:** Labor 03 · Bindings

**Headline:** Join the software they already paid for.

**Dek:** An agent that lives beside the real system, in a tab no one has to open, is a hobby. A binding is a deliberate connection, with a direction, a permission, and a way to fail visibly.

### The catalog

**System of record.** Where the truth is supposed to sit. Often old, often recently moved, often still fed by a batch. Bind it read-first. Write only after shadow week and a security signature.

**System of use.** Where the person already works: the claim screen, the teller tool, the maintenance console, the case jacket. This is the binding the floor will judge us by. If the draft does not appear here, it does not exist.

**Unofficial system.** The inbox and the workbook. Bind these read-only, and only for this process, and put an expiry on the binding. An unofficial system that becomes a permanent dependency was mislabeled. It is a system of record that no one owns. Say so, and give it an owner, or stop reading it.

### Patterns we will actually use

**API, when it is real.** Prefer it. Test it on their tenant, with their sign-on, on a file they consider boring.

**Event, when the floor is event-shaped.** A file arrives, a draft is requested, a release is recorded. Do not invent an event architecture for a desk that works in a pile.

**Attended desktop, when there is no API and the work cannot wait a year.** A person is present. The agent does not drive a screen unattended at 3am. This pattern has an expiry date on the day it is agreed.

**Read-only first.** Always available, often sufficient for the first month, and the only pattern we will defend in a hurry.

### A binding entry

Each system gets a catalog card: name in their language, pattern, direction, permission from the access design, owner, expiry if any, and the sentence that describes failure. "It will log and the draft will not appear." Failure that looks like success is a broken binding.

### Close

The first thin binding should be boring. Boredom is a feature of read-only.

**Stamp:** Redraw the workflow
**Text link:** Security of the premises

## Layout

Posture: **Parts catalog.**

Three catalog entries as Record plates without images, in a vertical stack, each with a mono part number: `B-01 Record`, `B-02 Use`, `B-03 Unofficial`. The part number is brass-ink at small size. Title is the system name. Body is the paragraph.

Under that, four pattern rows as a compact Ledger: Pattern, When, Constraint. Rows: API, Event, Attended desktop, Read-only first. Caption: "Binding patterns Feld will sign."

Then "A binding entry" as prose, then close.

Stamp `/work/redraw`. Text link `/security`.

Visual reference: a machined-parts list, plenty of hairlines, mono part numbers, no isometric 3D connectors, no "integration diagram" of floating logos.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/work/bindings`. Story: `Pages/Bindings`, day, night, palm. Mast active: The Work. Rail 15 / 50. Crumb: Feld / The Work / Bindings.

Posture: **Parts catalog**, per Layout. Copy verbatim. Use Record for the three systems and Ledger for the four patterns. Do not depict third-party logos.

Stamp `/work/redraw`. Text link `/security`.

Acceptance: part numbers visible; table caption present; attended-desktop row includes the expiry constraint; both ledgers; palm scrolls the table rather than card-ifying it; colophon; no hex.
