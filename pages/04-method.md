# 04 — Method

| | |
|---|---|
| Route | `/method` |
| Story | `Pages/Method` |
| Section | The Work |
| Rail | 04 / 50 |
| Posture | Stations |

## Copy

**Browser title:** Method — Feld Company

**Meta description:** Eight stations of a Feld install, from lifting a legacy system into reach to the work that never made the original list. Each station leaves an artifact behind.

**Eyebrow:** The Work · Method

**Headline:** Eight stations. Each one leaves something on the table.

**Dek:** The conjecture lists the work. This is how a pod walks it. Stations can run in parallel after the third. None of them is optional because a vendor demo skipped it. Duration is a range from the field, not a promise.

### Station 01 · Passage

**Duration:** a few weeks, or a quarter, depending on what "the system" turns out to mean.
**Artifact:** a path the agent can use, with the batch window and the forbidden hours written on it.
**Failure:** declaring the cloud migration done because the database moved, while the real work still happens in a terminal the agent has never seen.
**Link:** Passage

### Station 02 · Access

**Duration:** overlaps passage, and outlives it.
**Artifact:** a one-page access design: read, draft, release, train. Names in the boxes, not departments.
**Failure:** a cleanup program that finishes without a single permission changing.
**Link:** Access

### Station 03 · Bindings

**Duration:** the first thin binding in days, the write-binding only after shadow week.
**Artifact:** a catalog entry per system: of record, of use, and unofficial.
**Failure:** an API that works in the pod's tenant and dies on the customer's single sign-on.
**Link:** Bindings

### Station 04 · Redraw

**Duration:** a working redraw before any release right is granted.
**Artifact:** the workflow on one page. The agent's job, the human's judgment, the queue where a wrong draft sits.
**Failure:** automating the current path so faithfully that its superstitions become policy.
**Link:** Redraw

### Station 05 · The Loop

**Duration:** decided before shadow week, revised after it.
**Artifact:** a loop card. Who releases, who is the deputy, what happens at 2am, what never proceeds unattended.
**Failure:** "a human in the loop" with no human's name.
**Link:** The Loop

### Station 06 · Living evals

**Duration:** a first set before release, a cadence after.
**Artifact:** cases from this floor's files, an owner, a decay date, a threshold that pages someone.
**Failure:** a demo set that is never replenished, still green in a quarter when the work has changed.
**Link:** Living evals

### Station 07 · Weather

**Duration:** the contract's year, then a renewal or a real goodbye.
**Artifact:** a weather log. Model, date, what moved, what was retested, what was refused.
**Failure:** an upgrade performed on a Thursday because the vendor's note sounded kind.
**Link:** Weather

### Station 08 · Unlisted

**Duration:** the whole engagement.
**Artifact:** a running list in the pod's book. Incentives, freezes, the exception-keeper, the regulator, the vendor who will not grant scope.
**Failure:** surprise, late, dressed up as change management.
**Link:** Unlisted

### How the stations braid

Cartography starts before station 01 and stains every station after it. Shadow week sits between the redraw and the first release. The handback is not a station. It is the condition under which we are allowed to leave the building.

### Close

Pick up the station your building is actually stuck on. Or start at the first ninety days, which braids them into a calendar.

**Stamp:** The first ninety days
**Secondary:** Begin, if you already know the process

## Layout

Posture: **Stations.**

A horizontal track on desk: eight station plates in a row, each 280px wide, inside a frame that scrolls on the x-axis with visible previous/next stamps labeled "Previous station" and "Next station". Scroll-snap proximity on the x-axis. A thin brass baseline runs behind the plates like a survey line, the traveled portion in patina.

Each plate is a Record/Ticket: numeral, name, duration in mono, artifact, failure in `--fg-muted`, text link. The failure line is prefixed with the word "Stall" in mono index, oxide color plus the word, not color alone.

Above the track, headline and dek in a blade measure. Below the track, "How the stations braid" in a Measure, then the close cluster.

Palm: the track becomes a vertical Stack. The baseline becomes a left border. Prev/next hide.

The track is a `region` named "Stations of the install". Buttons are real buttons.

Night: baseline's traveled portion is phosphor; plates are `--bg-raised`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/method`. Story: `Pages/Method`, day, night, palm. Active mast link: The Work. Rail 04 / 50. Crumb: Feld / The Work / Method.

Posture: **Stations**, per Layout. Copy verbatim. Eight stations, correct links: `/work/passage`, `/work/access`, `/work/bindings`, `/work/redraw`, `/work/the-loop`, `/work/evals`, `/work/weather`, `/work/unlisted`. Stamp to `/ninety-days`. Secondary stamp to `/begin`.

Do not turn this into a logo-process infographic with circles and arrows. The baseline is one line. Failure is the word "Stall" plus text.

Acceptance: keyboard users can operate previous/next and can also tab into each plate's link; the horizontal scroll is not a trap; reduced motion disables snap; palm is vertical; no hex; colophon present.
