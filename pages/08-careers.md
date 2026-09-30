# 08 — Careers

| | |
|---|---|
| Route | `/careers` |
| Story | `Pages/Careers` |
| Section | Firm |
| Rail | 08 / 50 |
| Posture | Posting board |

## Copy

**Browser title:** Careers — Feld Company

**Meta description:** Four roles: forward-deployed engineer, eval keeper, cartographer, industry principal. The work is in the customer's building. The romance wears off. The practice does not.

**Eyebrow:** The firm · Roles

**Headline:** Come for a year inside someone else's process.

**Dek:** The conjecture's last line is the hiring plan: a good time to be an FDE, or a firm of them. These are the seats. None of them is a tour of meetings with a laptop for scenery. You will be in their building for the weeks that decide the install.

### What we ask of everyone

You can sit with a person who is good at their job and not rush them toward a tool. You can write a page someone on that floor will recognize as their Tuesday. You can say, in a meeting with a sponsor, that the process is not ready. You can come back for weather after the interesting month is over.

Travel is real. So is the week at your own desk, writing the eval nobody will clap for. We hire people who want both, and we say so before the first conversation.

### The four seats

**Forward-deployed engineer.** You make the binding and you sit through shadow week when it misbehaves. You can read a system you did not author.

**Eval keeper.** You build the set of cases from their files, name an owner, and defend the decay date against optimism.

**Cartographer.** You draw the process, including the unofficial one, before anyone is allowed to be clever.

**Industry principal.** You have stood on this kind of floor for years. You stop us from solving a generic company.

### What we will not pretend

This is not a remote-only idyll, and it is not a hero's schedule. Pods are small so that evenings can end. If a process truly requires a night presence, it is designed, staffed, and paid as night presence, not extracted from someone's goodwill.

The cast you just met is a draft of the firm. The roles are the true part.

### Close

Read a seat. If it sounds like your work, the letter at the end of this site has a line for you as well as for sponsors.

**Stamp:** Begin a letter
**Text link:** The forward-deployed seat, first

## Layout

Posture: **Posting board.**

Headline and dek, blade measure.

"What we ask of everyone" as a Measure.

Then four Tickets pinned on a Gather, two by two on desk, one column on palm. Each ticket has a mono index (Seat 01–04), a title, the two-line description from the copy, and a text link "Read the seat". Tickets are links to:

- `/careers/forward-deployed-engineer`
- `/careers/eval-keeper`
- `/careers/cartographer`
- `/careers/principal`

They look pinned, not floating: radius 0, hairline, a brass corner tick 12px in the top left, no shadow, slight `--bg-raised`. Hover strengthens the border. They do not rotate. "Pinned" is a metaphor for the reader of this packet, not a CSS transform.

Then the "will not pretend" Measure, then the close. Stamp `/begin`. The text link goes to the FDE page.

No photos of offsites. No benefits grid of unlimited vacation. If you feel the page needs warmth, it is already in the sentence about evenings.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/careers`. Story: `Pages/Careers`, day, night, palm. Mast active: Firm. Rail 08 / 50. Crumb: Feld / Firm / Careers.

Posture: **Posting board**, per Layout. Copy verbatim. Four tickets, correct hrefs, no rotation, no drop shadow, brass corner tick via the survey-tick icon or a 12px SVG.

Do not add salary numbers; they are not in the copy. Do not add a culture carousel.

Acceptance: each ticket is one link with a clear accessible name (the seat title); hover and focus states visible in both ledgers; palm is one column; colophon present; no hex in the page component.
