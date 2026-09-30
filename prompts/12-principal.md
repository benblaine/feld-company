# Build prompt 12 — Industry principal

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 12 — Industry principal

| | |
|---|---|
| Route | `/careers/principal` |
| Story | `Pages/RolePrincipal` |
| Section | Firm |
| Rail | 12 / 50 |
| Posture | Witness |

## Copy

**Browser title:** Industry principal — Feld Company

**Meta description:** The seat for people who have stood on a kind of floor for years: claims, close, plant, intake. They stop the firm from solving a generic company.

**Eyebrow:** Roles · Seat 04

**Headline:** Industry principal.

**Dek:** You have already done the job the agent is being asked to draft for, or you have led the people who do it. Feld hires you so the pod does not mistake fluency for judgment.

### A letter from the seat

You will be in the building less than the forward-deployed engineer and more than the sponsor expects. Your job in the first month is witness. You listen for the sentence that means this floor is unlike the last three, and for the sentence that means it is exactly like them. You say which is which, out loud, before the redraw hardens.

You will block work. A claims principal blocks a capital-markets novelty that wandered into a motor floor. A plant principal blocks an agent that wants to close a permit. A civic principal blocks a draft the applicant cannot appeal. These blocks are not failures of collaboration. They are the seat.

Later you become the person who can tell a peer at the customer, in their language, what changed and what did not. The keeper should be able to call you after we step aside, for a while. Put that in the engagement. Do not leave it as goodwill.

### What you bring

Years on one kind of floor, recent enough that the queue's names are still in your mouth. The ability to write a page a handler, a clerk, a shift lead, or a reviewer will accept as fair. A reputation for stopping things, which we will ask about.

You do not need to write the binding. You need to know when the binding has crossed into the work you once signed your name under.

### Floors we know we need

Financial and insurance operations. Industrial and energy. Civic and health operations. Firms of record, when the partner still signs. If your floor is not on that list, the letter is still open. Say what the release decision is, in one sentence. We will know if we are ready to learn it.

### Close

Name the floor. Name the decision you used to be accountable for.

**Stamp:** Write to the firm
**Text link:** The industries, seen from this seat

## Layout

Posture: **Witness.**

The page is a letter. Measure width `--letter` (58ch), text face, the dek set as the first paragraph rather than a marketing lede — but the dek style may remain lede size for the first sentence only.

"A letter from the seat" opens with a dateline in mono: "From the principal's desk · no headquarters". The heading is still a real h2.

Pull nothing out into cards. The "Floors we know we need" section is a short list with brass ticks, each line linking to the industry index or the relevant page: `/industries/insurance`, `/industries/plants`, `/industries/civic`, `/industries/firms-of-record`.

A large brass opening quotation mark is forbidden; this is not that kind of letter. Let the dateline do the work.

Stamp `/begin`. Text link `/industries`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/careers/principal`. Story: `Pages/RolePrincipal`, day, night, palm. Mast active: Firm. Rail 12 / 50. Crumb: Feld / Firm / Careers / Industry principal.

Posture: **Witness**, per Layout. Letter measure. Copy verbatim. Floor names link to the routes above.

Stamp `/begin`. "The industries, seen from this seat" links to `/industries`.

Acceptance: the measure is 58ch and readable; palm keeps the same measure with page padding; list links are underlined signal; both ledgers; colophon; no portrait; no hex.
