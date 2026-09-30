# 03 — Manifesto

| | |
|---|---|
| Route | `/manifesto` |
| Story | `Pages/Manifesto` |
| Section | Foundation |
| Rail | 03 / 50 |
| Posture | Nine rooms |

## Copy

**Browser title:** Manifesto — Feld Company

**Meta description:** Nine statements Feld will work by. A field manual's first page, written as rooms you scroll through.

**Eyebrow:** Foundation · Nine rooms

**Headline:** What we will work by.

**Dek:** Not values on a wall. Operating statements. If a pod cannot act on one of these on a Tuesday, it does not belong here.

### 01 · The unit of work is the process

We are hired into a process that already has a name inside the company: the reserve note, the month-end close, the permit to work, the benefits intake. We are not hired into "AI."

### 02 · The agent drafts. A person releases.

Release is a named seat, with a deputy for leave and for night. If no one will put their name on the release, the process is not ready, and the agent does not get a queue.

### 03 · Access is a design, not a cleanup

Who may read, who may draft, who may release, who may have their work used as an example. Four questions. A data lake that cannot answer them is a larger unread room.

### 04 · We bind what the company already runs

The system of record, the system people actually touch, and the unofficial system — the inbox, the side workbook, the shared drive named Final. Pretending the unofficial system is not load-bearing is how installs fail in week six.

### 05 · Evals are born from the floor and given a decay date

A benchmark from the public internet is a different instrument. Our eval is a set of cases from this company's own files, with an owner and a date after which it is presumed stale.

### 06 · Weather is part of the contract

A new model is not a pleasant surprise to be absorbed by the customer's spare time. The return visit is scheduled. What is retested is written down. What we refuse to switch is written down too.

### 07 · We will decline work

Processes where release cannot be named. Processes where a person being reviewed cannot see why. Processes that ask an agent to practice a licensed profession. Processes a pod does not yet understand. The refusal is delivered early, in writing.

### 08 · The handback is the product

The customer ends with a keeper, a runbook, a binding they can operate, and a right to call the pod back for weather. A go-live party is not a handback.

### 09 · We are guests on someone else's floor

We sit where the work sits. We learn the queue's real name. We do not arrive with a platform and look for a place to put it.

### Close

If these match the work you have, begin. If they do not, the refusal will save both sides a quarter.

**Stamp:** Begin a deployment
**Text link:** Read the method

## Layout

Posture: **Nine rooms.**

Each statement is a room: min-height `100svh` minus the mast, so one statement occupies the screen. Scroll-snap on the main column, `proximity` not `mandatory`, so a person is not trapped. Under reduced motion, scroll-snap is off.

Inside each room, a Gather: brass numeral at `--text-h1` in the left three columns, vertically centered; the statement in the remaining columns, headline at `--text-h2` in Fraunces, the paragraph at `--text-body` beneath, measure blade. The numeral is `aria-hidden` because the heading text carries the meaning; the visible heading includes the words, not only the number. Room index for assistive tech is the heading.

A slim progress of nine ticks fixed at the right edge of the measure, the current room's tick in `--signal`. This is decorative and `aria-hidden`; the headings are the real structure.

The opening headline and dek are room zero, shorter, not snapped. The close is a last room with the two actions, not a tenth statement.

Palm: numeral above the statement, rooms still tall but min-height auto if the paragraph would overflow, snap off.

No images. No cards. Background stays `--bg`. Room 07 (decline) may use `--bg-raised` as the only surface change, a quiet emphasis.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/manifesto`. Story: `Pages/Manifesto`, day, night, palm, and a reduced-motion story where snap is absent.

Posture: **Nine rooms**, per Layout. Rail 03 / 50. Crumb: Feld / Manifesto.

Set the Copy verbatim, nine statements, in order. Do not add a tenth. Do not soften statement 07. Scroll-snap as specified, defeated by `prefers-reduced-motion`. The right-edge ticks are decorative.

Stamp to `/begin`. Text link to `/method`.

Acceptance: one statement dominates the viewport at desk width; keyboard users can tab to the stamp without being snap-jailed (snap is proximity, and focus is not stolen); night ledger changes signal to phosphor and room 07's raised surface to night-2; colophon after the close, outside the snapped rooms so it can be reached.
