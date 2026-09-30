# 21 — Industries

| | |
|---|---|
| Route | `/industries` |
| Story | `Pages/Industries` |
| Section | Industries |
| Rail | 21 / 50 |
| Posture | Index of floors |

## Copy

**Browser title:** Industries — Feld Company

**Meta description:** The floors Feld knows how to enter: banking, insurance, health-system operations, plants, energy, freight, retail operations, civic institutions, and firms of record.

**Eyebrow:** Industries

**Headline:** Approaches by the floor, not by the sector's adjective.

**Dek:** The conjecture expects the work to differ by industry. So do we. Each page names the first process we would touch and the release decision we will not take away from a person.

### The floors

**Banking.** KYC refresh and the credit memo's first draft. The control that will not move, stays. `/industries/banking`

**Insurance.** The reserve note and the file a handler releases under their name. `/industries/insurance`

**Health systems.** Operations around the clinician: packets, referrals, coding queries. The clinician releases. The agent does not practice. `/industries/health-systems`

**Plants.** The maintenance work order and the permit. The agent does not close a permit. `/industries/plants`

**Energy.** The shift log and the outage desk, where a sentence may be read by a regulator. `/industries/energy`

**Freight.** The yard, the dwell, the update a customer is owed in plain words. `/industries/freight`

**Retail operations.** Allocation and the Monday labor schedule. Not the storefront, not the brand. `/industries/retail-operations`

**Civic institutions.** Benefits intake and the case note. The applicant can see why. `/industries/civic`

**Firms of record.** The matter and the workpaper. The partner still signs. `/industries/firms-of-record`

### What we are not claiming

We are not claiming every industry, and we are not claiming the dramatic part of these ones. Trading desks, clinical diagnosis, the creative campaign, the autonomous vehicle: other firms may be built for them. Our cut is the operational process with a release decision a person can name.

### Close

If your floor is missing, the letter can still find us. Say the release decision in one sentence.

**Stamp:** Write the release decision
**Text link:** Or start with size, if industry is the wrong cut

## Layout

Posture: **Index of floors.**

A list, not a card grid. Each floor is a full-width row, hairline top, min-height 72px, the name in display h3 as the link, the sentence in `--fg-muted` on the same row at desk, wrapping under the name on palm. A mono index 01–09 at the left. The whole row is the link, with the visible name as the accessible name, and the sentence in the same link so it is not a mouse-only expansion.

Hover: the row's background becomes `--bg-raised` and the name's underline (links are underlined) stays. No arrow-in-a-circle.

Headline and dek above, blade. The disclaimer and close below in a Measure.

Stamp `/begin`. Text link `/scale/global`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/industries`. Story: `Pages/Industries`, day, night, palm. Mast active: Industries. Rail 21 / 50. Crumb: Feld / Industries.

Posture: **Index of floors**, per Layout. Nine rows, exact hrefs from the copy. Whole row is one link. Copy verbatim.

Stamp `/begin`. Text link `/scale/global`.

Acceptance: nine links in order; palm wraps the sentence without overflow of the page; focus ring visible on the row; both ledgers; colophon; no industry photography; no hex.
