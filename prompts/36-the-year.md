# Build prompt 36 — The year

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 36 — The year

| | |
|---|---|
| Route | `/the-year` |
| Story | `Pages/Year` |
| Section | Practice |
| Rail | 36 / 50 |
| Posture | Seasons |

## Copy

**Browser title:** The year — Feld Company

**Meta description:** After ninety days: the seasons of an install. Model weather, the second process, and the temptation to widen too fast.

**Eyebrow:** Practice · The year

**Headline:** Stay long enough for the work to change twice.

**Dek:** The first ninety days prove a slice. The year proves the install can survive a model change, a staff change, and the temptation to bolt a second process onto a tired keeper.

### Season of the cadence

The decay date comes around more than once. The keeper runs it. We attend the first few and then we read the log. A cadence that only works when Feld is in the room is not a cadence.

### Season of weather

At least one material model change will arrive if the year is an ordinary year. The log records the retest and the decision. A year with no weather entry is a year nobody was watching, not a year of stability.

### Season of the second process

If the first process holds, a second may start. It gets its own map. It does not inherit the first process's permissions by convenience. The keeper of the first process is asked, not assumed, before their name is put on anything new.

### Season of leaving the building

We are there less. The handback note is signed. The right to call remains. Leaving is a season, not an event on a Friday. A pod that vanishes and a pod that will not leave are both failures, of different kinds.

### Close

Renew the year or end it cleanly. Both conversations happen in month ten, not in week fifty-two.

**Stamp:** Read the handback
**Text link:** Weather, the labor inside the year

## Layout

Posture: **Seasons.**

Four horizontal bands, full width of the gather, each with a large display numeral 01–04 in `--tick` at low contrast-but-still-AA for large type (brass on bone is acceptable at display size; on night use `--tick` which is night-brass). Check: large brass `#8a6433` on bone is 4.44 which fails AA even for large text? 

WCAG large text is 3:1 for UI components... actually large text AA is 3:1. 4.44 passes for large text (18pt+ or 14pt bold). Display numerals are large. OK.

Each band: numeral, season name as h2, paragraph. Bands alternate `--bg` and `--bg-raised` very quietly. Generous vertical padding `--space-8`.

Stamp `/handback`. Text link `/work/weather`.

No circular "season wheel."

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/the-year`. Story: `Pages/Year`, day, night, palm. Mast: none active. Rail 36 / 50. Crumb: Feld / The year.

Posture: **Seasons**, per Layout. Four bands in order: cadence, weather, second process, leaving the building. Copy verbatim. Numerals may use `--tick` because they are display size.

Stamp `/handback`. Text link `/work/weather`.

Acceptance: four seasons in order; alternating surfaces still pass text contrast (text uses `--fg` on `--bg` or `--bg-raised`, both fine); both ledgers; no circular diagram; colophon; no hex.
