# Build prompt 18 — Living evals

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 18 — Living evals

| | |
|---|---|
| Route | `/work/evals` |
| Story | `Pages/Evals` |
| Section | The Work |
| Rail | 18 / 50 |
| Posture | The set |

## Copy

**Browser title:** Living evals — Feld Company

**Meta description:** Evals generated from the real work and maintained after kickoff: cases, an owner, a decay date, and a threshold that pages a person.

**Eyebrow:** Labor 06 · Living evals

**Headline:** An eval that knows its own funeral.

**Dek:** Generate the set from this floor's files. Name an owner. Give it a decay date. Decide the threshold that pauses the queue. Then keep the set alive after the demonstration has left the calendar.

### What goes in the set

Cases the floor recognizes. Ordinary ones, so the agent is not praised for surviving a circus. Ugly ones, including the file that went wrong last quarter. A few the agent should refuse. The mix is written on the card, so a later reader can see whether the set has drifted toward easy greens.

Public benchmarks can teach a pod something in private. They are not this labor, and they are not cited to the customer's board as if they were the work.

### Who keeps it

A keeper on the customer's side, named before go-live, paired with Feld's eval keeper through the first decays. After the handback, the customer's keeper runs the cadence. We return for weather, or when they ask, not as the permanent owners of their judgment.

### The page that gets sent

When the threshold breaks, a person is paged. The page says which cases moved, and it says "the queue is paused." It does not say "minor regression" unless someone is prepared to own that phrase in front of the floor. Paging is a product surface. Write it like a letter to a tired person.

### Close

If you cannot point to twelve real files, you are early, and that is a fine time to begin. It is a bad time to switch a model.

**Stamp:** Weather, and the upgrades
**Text link:** The keeper's seat

## Layout

Posture: **The set.**

A Ledger of six specimen rows, caption "A specimen set. Composite. Not a client." Columns: Case, Kind, Owner, Decay, Status. Kinds from a small vocabulary: Ordinary, Ugly, Refusal. Statuses: Living, Stale, Paused. Include one stale row and one paused row so the component's status words are visible. Times and dates in mono. This table is filterable by Kind via the Ledger filter, and paginated only if you insist — six rows do not need pages. Do not paginate six rows. Sort by Case is allowed.

Specimen rows, use exactly:

| Case | Kind | Owner | Decay | Status |
|---|---|---|---|---|
| Side-glass, prior ruling | Ordinary | P. | 6 Apr | Living |
| Duplicate claimant | Ugly | P. | 6 Apr | Living |
| Night-batch read | Refusal | P. | 6 Apr | Living |
| Coverage already denied | Refusal | P. | 2 Mar | Stale |
| Photo without metadata | Ordinary | P. | 6 Apr | Paused |
| Neighbor-check file | Ugly | Deputy | 6 Apr | Living |

Below the table, the prose sections. A slip example may be shown statically (not auto-fired) with the warning copy: "This draft has a decay date of Friday." Label it "The page a person receives" so it is not a surprise toast on load. It must not auto-dismiss in a loop. Prefer rendering the Slip component in a static preview mode if the component supports it; otherwise a Record that quotes the slip. Do not fire a toast on page load.

Stamp `/work/weather`. Text link `/careers/eval-keeper`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/work/evals`. Story: `Pages/Evals`, day, night, palm, plus a filtered story showing only Refusal. Mast active: The Work. Rail 18 / 50. Crumb: Feld / The Work / Living evals.

Posture: **The set**, per Layout. Use Ledger. The six rows are exact. Filter works. Do not paginate. Do not toast on load. Copy verbatim around the table.

Stamp `/work/weather`. Text link `/careers/eval-keeper`.

Acceptance: filter live region announces the count; stale and paused are words plus discs; caption includes "Composite"; both ledgers; palm scrolls the frame; colophon; no hex.
