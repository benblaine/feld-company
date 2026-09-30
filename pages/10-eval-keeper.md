# 10 — Eval keeper

| | |
|---|---|
| Route | `/careers/eval-keeper` |
| Story | `Pages/RoleEval` |
| Section | Firm |
| Rail | 10 / 50 |
| Posture | Decay |

## Copy

**Browser title:** Eval keeper — Feld Company

**Meta description:** The seat that builds evals from a company's own files, gives them an owner and a decay date, and stops an upgrade the cases will not carry.

**Eyebrow:** Roles · Seat 02

**Headline:** Eval keeper.

**Dek:** You are hired to disappoint optimists on a schedule. A living eval is a set of this floor's own cases, scored, owned, and presumed stale on a date everyone can see.

### The specimen

**Case:** Reserve note, side-glass, prior ruling on coverage.
**Owner:** P., claims quality. Deputy: the Friday handler.
**Born:** from twelve files the floor chose, not from a public set.
**Score:** the draft matched the handler's release on the points that matter, and flagged the one file it should have refused.
**Threshold:** if more than two cases in the set drift, the queue pauses. A person pages. The agent does not "try harder."
**Decay:** first Monday of next month. After that the score is a relic, even if it is green.

This specimen is the shape of the job. You will make many of them. You will retire them. You will refuse to let a sponsor screenshot the green ones for a board meeting after the decay date.

### The argument you will keep having

The forward-deployed engineer wants the binding to feel alive. The sponsor wants a line to move. You want the line to mean this month's work. Both of them are your colleagues. The decay date is how you stay friends.

When weather arrives — a new model, a new capability, a quiet regression — you re-run the living set before anyone switches. You write the result in the log, including the refusal.

### What you bring

You have built test sets that were allowed to fail a launch. You can explain a false green to someone who does not love numbers. You are bored by leaderboards and alert to a single file that would harm a person.

You do not need to be the best engineer in the pod. You need to be the one who will say the set is dead.

### Close

If you have killed a launch with a test, say which kind, without naming the employer if you cannot.

**Stamp:** Write to the firm
**Text link:** How living evals work on an install

## Layout

Posture: **Decay.**

The specimen is an Eval card from the design system, set large, span 7, not a screenshot of a product. Around it, a second quieter plate, span 5, titled "After the decay date" containing only this sentence: "The score remains visible. A resin banner reads: Stale. Do not cite." Show that banner in `--warning` text plus the word, on `--bg-sunken`.

This pair sits between the dek and "The argument you will keep having." It is a designed object, and the words in the specimen match the copy's specimen list exactly.

The rest of the page is a letter-width Measure.

No chart of a model climbing up and to the right.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/careers/eval-keeper`. Story: `Pages/RoleEval`, day, night, palm. Mast active: Firm. Rail 10 / 50. Crumb: Feld / Firm / Careers / Eval keeper.

Posture: **Decay**, per Layout. Use the Eval card component for real, not a lookalike div soup, so the story also proves the component. Copy verbatim. The stale banner is part of the page composition beside the card.

Stamp `/begin`. Text link `/work/evals`.

Acceptance: the card shows owner, decay, score, threshold, and a status word; the stale state is text and not color alone; palm stacks card then banner; both ledgers; colophon; no hex in the page.
