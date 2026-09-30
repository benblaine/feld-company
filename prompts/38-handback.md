# Build prompt 38 — Handback

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 38 — Handback

| | |
|---|---|
| Route | `/handback` |
| Story | `Pages/Handback` |
| Section | Practice |
| Rail | 38 / 50 |
| Posture | On the table |

## Copy

**Browser title:** Handback — Feld Company

**Meta description:** What remains with the company when the pod steps aside: a keeper, a runbook, a binding they can operate, a weather log, and the right to call.

**Eyebrow:** Practice · Handback

**Headline:** What we leave on the table.

**Dek:** Stepping aside is a designed season. The table, at the end of it, should hold things a keeper can pick up without us. If a thing only works while a Feld engineer is logged in, it is not ready to be left.

### On the table

**The keeper's name**, employed by the company, with hours for the cadence written into their actual job, not into a hope.

**The runbook**, in the company's language: how to pause the queue, how to retire a case, how to add a case, who to call when the binding fails on a Sunday.

**The binding**, with its permissions, its expiry dates, and the sign-on their own administrator can grant and revoke.

**The eval set**, current, with the next decay date already in the book.

**The weather log**, including the refusals, because a log of only the upgrades is a brochure.

**The loop card**, names refreshed, deputy confirmed for the coming month.

**The attestation**, still visible to the floor, still storing draft, edit, and release.

**A letter of what we will still answer**, and for how long. The right to call is specific. "Feel free to reach out" is not a handback.

### What we take with us

Nothing of theirs. Cases stay. Notes from cartography that they consider sensitive stay in their premises. We keep our own method, and the right to remember the shape, not the file.

### The signature

The keeper signs the handback note, or they do not. An unsigned note means we are still in the season of leaving. We do not announce completion over their hesitation.

### Close

This is the product. The rest of the site describes how a table gets this full.

**Stamp:** Read the pricing letter
**Text link:** The essay on stepping aside

## Layout

Posture: **On the table.**

A literal table surface: a wide plate, `--bg-raised`, with the eight items laid out as a 2×4 grid of small tickets on desk, 1 column on palm. Each ticket has a short title (the bold lead-in) and the sentence. No shadows that pretend to be physical objects beyond `--shadow-plate` on the whole surface only, not on each ticket. Tickets are flat, hairline, radius 0.

The plate has a caption beneath, not inside: "The handback table. Eight things, or we are not done."

Prose for "What we take with us" and "The signature" below the plate, letter measure.

Stamp `/pricing`. Text link `/journal/stepping-aside`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/handback`. Story: `Pages/Handback`, day, night, palm. Mast: none active. Rail 38 / 50. Crumb: Feld / Handback.

Posture: **On the table**, per Layout. Eight items exact. The shadow, if used, is `--shadow-plate` on the whole plate once. Copy verbatim.

Stamp `/pricing`. Text link `/journal/stepping-aside`.

Acceptance: eight tickets; caption present; palm is one column; both ledgers; colophon; no hex; the signature section is outside the plate.
