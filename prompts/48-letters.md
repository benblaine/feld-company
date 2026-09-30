# Build prompt 48 — Three letters

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 48 — Three letters

| | |
|---|---|
| Route | `/letters` |
| Story | `Pages/Letters` |
| Section | Practice |
| Rail | 48 / 50 |
| Posture | Three envelopes |

## Copy

**Browser title:** Three letters — Feld Company

**Meta description:** Short letters to the CIO, the COO, and the chief AI officer. Each one names the decision that seat actually holds.

**Eyebrow:** Practice · Letters

**Headline:** The same install, written to the seat that has to live with it.

**Dek:** Choose the seat you sit in. The other two letters remain available. None of them is a persona. They are the decisions.

### To the chief information officer

You will be asked to make the old system reachable and to keep the new path revocable. Both are your work, and they pull against each other if the program is vain. Passage without a revocation you have practiced is a new room you cannot lock. Bindings that the vendor will not scope are a commercial problem wearing a technical coat. Send us, or your integrator, into that conversation in week one.

You do not have to become the owner of the process. You do have to refuse a write-access that has no field list. We will support that refusal in front of a sponsor. It is one of the reasons to hire a pod rather than a slide.

If you are also the person resetting access because the company is not large, read the mid-market page before you read the rest. The footprint has to fit the team you already have.

### To the chief operating officer

The process is yours, whatever the technology committee believes. The release name is probably someone you already trust with a bad day. The redraw will change their Tuesday. You should be the person who tells them that, and we should be in the room so the promise does not outrun the eval.

Ask us what we will not automate. If we answer with a category rather than a sentence about your floor, send us away. After shadow week, either a narrow release or a wait is a good report. A report that can only say "accelerating" is a report from a different kind of firm.

Your incentive question matters more than your tooling question. Who is paid for speed, and who is paid for never being the name on a mistake. Tell us before we draw the loop.

### To the chief AI officer

You have been hired to make this real without making it reckless. We will not compete with your platform strategy. We will ask it to tolerate a process that has its own eval, its own decay, and its own right to refuse a model the platform team likes.

The weather log should be a document you can show a board without translating it into enthusiasm. Refusals belong on it. If your office cannot publish a refusal, the company does not yet have a practice. It has a pipeline.

Keep the keeper in the business, not in your office. A center of excellence that owns every eval will become the bottleneck the conjecture is warning you about, wearing a modern name.

### Close

If you share a building with the other two seats, send them the letter, not a summary. Summaries are where the refusal gets lost.

**Stamp:** Begin from your seat
**Text link:** Readiness, if you want the questions first

## Layout

Posture: **Three envelopes.**

Three tabs, implemented as a tablist with keyboard support (roving tabindex, arrow keys, Home/End), labels: "CIO", "COO", "Chief AI officer". The selected letter is a stationery sheet, letter measure, `--bg-raised`, hairline, radius 0. The others are not display:none in a way that removes them from the accessibility tree incorrectly — use the tabs pattern properly: unselected panels `hidden`.

Default tab: CIO. Deep-link with hash `#cio`, `#coo`, `#caio` so a URL can open a letter. On load, read the hash.

Each panel starts with a mono dateline: "Letter · chief information officer" (and the matching titles).

Do not illustrate envelopes with a flap illustration. The tab is the envelope. A flap would be costume.

Stamp `/begin`. Text link `/readiness`.

Under the sheet, a line of text links to the other letters' hashes, for people who do not notice tabs. Duplicate access is fine.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/letters`. Story: `Pages/Letters`, day, night, palm, and one story per open tab. Mast: none active. Rail 48 / 50. Crumb: Feld / Letters.

Posture: **Three envelopes**, per Layout. WAI-ARIA tabs pattern, hashes `#cio` `#coo` `#caio`. Copy verbatim, each letter only in its panel. The mid-market mention links to `/scale/mid-market`.

Stamp `/begin`. Text link `/readiness`.

Acceptance: arrow keys move tabs; the selected tab is `aria-selected`; the panel is labelled; hash opens the right letter; both ledgers; no envelope illustration; colophon; no hex.
