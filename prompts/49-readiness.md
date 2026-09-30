# Build prompt 49 — Readiness

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 49 — Readiness

| | |
|---|---|
| Route | `/readiness` |
| Story | `Pages/Readiness` |
| Section | Practice |
| Rail | 49 / 50 |
| Posture | Twelve questions |

## Copy

**Browser title:** Readiness — Feld Company

**Meta description:** Twelve questions about a process, answered yes, not yet, or unnamed. The result is a paragraph, not a score dressed as science.

**Eyebrow:** Practice · Readiness

**Headline:** Twelve questions, and a paragraph at the end.

**Dek:** This is not an assessment you can pass. It sorts the process toward the labor that is actually open. Answer for one process, not for the company. "Unnamed" is a respectable answer. It is often the true one.

### The questions

Each question offers three choices: Yes, Not yet, Unnamed.

1. Can you name the process in a sentence the floor would recognize?
2. Can an agent read the system of record during floor hours, without a scrape?
3. Can you name the person who may release?
4. Can you name the deputy?
5. Do you know the unofficial system the floor actually trusts?
6. Is there a sentence for what must never be automated?
7. Are there twelve real files you could give an eval without inventing them?
8. Is there a person who could own that eval with hours in their week?
9. Do you know the next freeze?
10. Can you revoke the agent's access on the company's side, this week?
11. Would a model change next Thursday be met by a person, or by surprise?
12. Can the person the file is about, or the regulator, or the partner who signs, see why?

### How the paragraph is chosen

Write the result from the answers. Do not show a numeric score, a donut, or a maturity level.

- If question 1 is Not yet or Unnamed: "Start with the name of the process. The other gaps are real and they can wait for a noun."
- Else if 2 is Not yet or Unnamed: "You are in passage. The record is not in reach yet, whatever the cloud program says."
- Else if 3 or 4 is Not yet or Unnamed: "You are in the loop, and the loop is missing a person. Do not bind a write path."
- Else if 5 is Not yet or Unnamed: "Cartography is unfinished. The unofficial system is still off the map."
- Else if 6 is Not yet or Unnamed: "Write the never-list before shadow week. A pod should refuse to draft without it."
- Else if 7 or 8 is Not yet or Unnamed: "You can draw and bind, and you cannot yet prove. The eval needs files and a keeper."
- Else if 9 is Not yet or Unnamed: "Ask for the freeze calendar before you pick a date."
- Else if 10 is Not yet or Unnamed: "Premises work remains. A path you cannot revoke is not ready."
- Else if 11 is Not yet or Unnamed: "The install has no weather. Someone should be designated before the next model, not after."
- Else if 12 is Not yet or Unnamed: "The attestation and the reason are the gap. The floor may be fine and the reader of the file is not."
- Else: "The labor left is practice: shadow week, a narrow release, a year of weather. Begin."

If several branches would match, use the first matching branch in this list. Mention, under the paragraph, the other open questions as a plain list titled "Also open", without ranking them.

### Close

Bring the paragraph into the letter if you want to. It gives the pod a head start. It is not a commitment, and it is not a diagnosis of your company.

**Stamp:** Take this into the letter
**Secondary:** Begin without it

## Layout

Posture: **Twelve questions.**

A form. Each question is a fieldset with a legend (the question) and three radios: Yes, Not yet, Unnamed. Radios are the Field component. Number the legends in mono.

After question 12, a primary stamp "Read the paragraph" that reveals the result in a region `aria-live="polite"`. The result uses the rules above exactly. Also show "Also open" when applicable.

Do not store answers to a server. Keeping them in the page is enough. The stamp "Take this into the letter" links to `/begin` and may put the paragraph in the query string `?from=readiness` plus a short code, or simply link to `/begin` with a note "Paste your paragraph if you like." Prefer the honest note over a clever encoded payload. The begin page does not need to parse it.

Validation: if they press the button with a question unanswered, move focus to the first unanswered legend and set a summary: "The paragraph needs all twelve. The first open one is marked." Do not color the unanswered questions red without text.

No progress donut. A quiet "7 of 12 answered" in mono is allowed, tied to a live region that is not assertive.

Stamp result actions: primary links `/begin` with visible words "Take this into the letter". Secondary stamp also `/begin`, "Begin without it", ghost or secondary.

The close copy sits under the form as well so the rules are not only in the machine.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/readiness`. Story: `Pages/Readiness`, day, night, palm, a story with nothing answered and the button pressed (error), a story with only question 2 as Not yet and the rest Yes (passage paragraph), and a story with all Yes (the begin paragraph). Mast: none active. Rail 49 / 50. Crumb: Feld / Readiness.

Posture: **Twelve questions**, per Layout. Branching rules exact, first match wins. No numeric score. Copy verbatim, including every question.

Both stamps go to `/begin`. The page does not submit to a backend.

Acceptance: keyboard can answer every fieldset; error focuses the first gap; the live result matches the branch table; "Also open" lists later gaps; both ledgers; no chart; colophon; no hex.
