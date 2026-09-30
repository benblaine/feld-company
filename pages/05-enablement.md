# 05 — Enablement

| | |
|---|---|
| Route | `/enablement` |
| Story | `Pages/Enablement` |
| Section | The Work |
| Rail | 05 / 50 |
| Posture | Two clocks |

## Copy

**Browser title:** Enablement — Feld Company

**Meta description:** One Tuesday on a claims floor, told twice. Once as a tool the company was enabled by. Once as work output placed in the process.

**Eyebrow:** The Work · Enablement

**Headline:** One Tuesday. Two ways it can be installed.

**Dek:** The conjecture draws the line where it matters: a completed implementation of a known tool, and then the vendor steps back; or work output, placed inside a process, with the complexity that comes with it. Here is that difference on a single floor, between 7:40 and 15:10.

**Scene:** A claims floor. Motor. A handler named R. has forty files and a reserve note due before she leaves. The composite is typical. R. is not a real person.

### Clock A · The tool she was enabled by

**7:40.** A new pane is live in the claim system. The training was last Thursday, forty minutes, a recording for anyone on leave.

**9:05.** R. pastes a note into the pane and receives a paragraph. It is fluent. It mentions a coverage she already ruled out yesterday. She deletes it and writes the note herself, faster than she can argue with the pane.

**11:30.** Three handlers are using the pane. One likes it for first sentences. No one is responsible for it. The usage chart, somewhere, is a number an executive will see in June.

**15:10.** The implementer has been gone since March. The pane is still enabled. The reserve notes are still hers, in the old way, with an extra tab she did not ask for.

### Clock B · Work output in the process

**7:40.** The queue has a name. "Draft reserve." An agent has read the file, the photo metadata, and yesterday's ruling. It has prepared a note and a list of what it did not know.

**9:05.** R. opens the draft. The wrong coverage is not in it, because that ruling is in the binding. She changes one sentence about the windshield. She releases the note under her own name. The draft, her edit, and the release are stored as one attestation.

**11:30.** A file the agent marked unsure sits in the exception desk, not in her pile. The unsure files are the eval's food. P. owns the eval. It decays on the first Monday of next month.

**15:10.** The pod is not in the building today. They are back on the first Thursday, because a model change shipped last week and twelve of P.'s cases moved. R.'s Tuesday did not become a product demo. It became a slightly different job, with her name still on the note.

### What changed is the responsibility

Clock A leaves a tool in the building. Clock B leaves a draft with a release, an exception path, an eval with an owner, and a date when someone comes back. The second clock is the one Feld is hired to build. It is slower to begin. It is the one still true in November.

### Close

If your floor still looks like clock A, the method says where to start.

**Stamp:** Read the method
**Text link:** A composite claims record

## Layout

Posture: **Two clocks.**

Headline and dek in a blade measure. Then a scene kicker in mono.

The two clocks are two columns on desk, span 6 and 6, separated by a hairline. Each column has a sticky header inside the column: "Clock A" in `--fg-muted`, "Clock B" in `--fg` with a 2px signal underline. Times are mono tabular, in a left gutter of the column, 64px. Events are text-face paragraphs.

The columns align by time. 7:40 lines up with 7:40. Use a grid of four rows, not two independent flowing articles, so the eyes can compare.

Below, "What changed is the responsibility" returns to a single Measure. Then the close.

Palm: Clock A fully, then Clock B fully, each time still in a gutter. A one-line preface before the stack: "Clock A first, then Clock B." Do not interleave on a phone. Comparison by scrolling back is acceptable; a tangled zip of times is not.

No illustration of R. No stock handler. The only graphic is the hairline and the times.

Night: Clock B's underline is phosphor. Clock A's header stays muted. Do not paint Clock A in red. It is not a villain. It is the older pattern.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/enablement`. Story: `Pages/Enablement`, day, night, palm. Mast active: The Work. Rail 05 / 50. Crumb: Feld / The Work / Enablement.

Posture: **Two clocks**, per Layout. Copy verbatim, including the initials R. and P. and the times. Do not add a third clock. Do not label Clock A "bad" or Clock B "good" in the UI; the prose carries the distinction. Do not use a red X / green check motif.

Stamp `/method`. Text link `/records/claims`.

Acceptance: at desk width the four times align across the hairline; at palm the clocks stack whole; reduced motion has no parallax on the sticky headers (sticky is allowed, animation is not); colophon present; no hex; the scene kicker is visible before the clocks.
