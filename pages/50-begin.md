# 50 — Begin

| | |
|---|---|
| Route | `/begin` |
| Story | `Pages/Begin` |
| Section | Practice |
| Rail | 50 / 50 |
| Posture | The letter you send |

## Copy

**Browser title:** Begin — Feld Company

**Meta description:** Write to Feld. Name the process, the person who releases today, and what must never be automated. A person reads the letter. The firm may decline.

**Eyebrow:** Practice · Begin

**Headline:** Tell us the process, and what must never be automated.

**Dek:** A person reads this. The firm may decline, and a decline is a complete response. If you are writing about a seat rather than a process, say so in the first line and skip what does not apply.

### The letter

**Your name.** Text. Label: Name.
Helper: The name you want on the reply.

**Email.** Label: Email.
Helper: We reply to this address. We do not add it to a list.
Error: That address cannot receive a reply.

**The seat you are writing from.** Select. Label: Seat.
Options: Choose one. Chief information officer. Chief operating officer. Chief AI officer. Operator of the process. Integrator. Keeper, or becoming one. A person who wants a seat here. Something else.
Error: The letter needs this.

**The size, if you are writing about a company.** Radios. Legend: Size of the company.
Options: Global enterprise. Upper mid-market. Holding company. Not the point of this letter.
Helper: "Not the point" is the right answer for a person seeking a seat.

**The process.** Text. Label: Process.
Helper: In the company's words, one sentence.
Error: The letter needs this. If you are seeking a seat, write "the seat" and say which one in the body.

**System of record.** Text. Label: System of record.
Helper: What the floor treats as the file of truth. "Unknown" is allowed.

**Who releases today.** Text. Label: Who releases today.
Helper: A role is acceptable if you cannot yet name the person. "Unnamed" is allowed.

**What must never be automated.** Textarea. Label: What must never be automated.
Helper: A sentence, not a category. If you do not know, write that.
Error: The letter needs this, even if the sentence is "we have not decided."

**The letter itself.** Textarea. Label: The letter.
Helper: As long as it needs to be. If you came from the twelve questions, paste the paragraph.
Error: The letter needs a letter.

**The promise.** Checkbox. Label as a full sentence: A person will read this letter, the firm may decline, and this page does not create an engagement.
Error: The letter needs this promise before it can be sent.

There is no password and no account. Do not add either.

### Confirm

Chamber, confirm. Title: Send this letter?
Body: It will be read by a person at the firm. You can still abandon it.
Stamps: Back. Send the letter.
Sending state of the primary stamp: Sending.

### What happens after

Success slip: The letter is with us. A person reads it.
The form remains, replaced in place by a short closing:

**Headline of the close:** It is with a person.

**Body:** If the process fits, you will hear from a principal. If it does not, you will hear that too. A decline is a complete response, and it will say why in a sentence.

Error slip, if the send fails: The letter did not leave this browser.
The form stays filled.

### What this page holds

Only the letter, and only if you send it. Measurement is off. There is no chat beside the form. Correspondence has no street address because the work is forward-deployed.

### Close, before the form is sent

If you are not ready to write, the twelve questions are a way to find the first sentence.

**Text link:** Read the twelve questions

## Layout

Posture: **The letter you send.**

A stationery sheet, letter measure, `--bg-raised`, hairline, radius 0, holding the form. Headline and dek above the sheet on the plain background.

Fields in the order given, stacked, `--space-5` between them. The size radios are a fieldset. The select is native. The two textareas are text-face; the shorter one ("What must never be automated") is four rows, the letter is ten.

Primary stamp at the bottom of the sheet: Send the letter. It opens the confirm chamber rather than sending immediately. The chamber's Send stamp performs the send. In this draft there is no backend: the send waits 600ms and succeeds, unless the query string contains `fail=1`, which shows the error slip and keeps the values. Document that query in the story, not on the page.

Validation runs on submit of the chamber's Send, or on the first Send the letter press — validate before opening the chamber. If invalid, do not open the chamber; focus the first invalid field; show the field errors; a summary at the top of the form in a live region: "The letter is missing answers. They are marked on the form."

Checkbox unchecked is invalid. "Unknown", "Unnamed", and "we have not decided" are valid content. Do not block them.

After success, replace the form with the closing headline and body, and move focus to that headline. The slip also fires, polite, and can auto-dismiss.

The text link to `/readiness` sits under the sheet.

No newsletter checkbox. No phone field. No company-size slider.

## Prompt

You are a senior design systems engineer building the last page of the Feld Company quire on the Instrument library. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, and `CHROME.md`.

Build `/begin`. Story: `Pages/Begin`, day, night, palm, a validation-error story, a confirm-chamber-open story, a success story, and a `fail=1` error-slip story. Mast: the Begin stamp is the current page, so mark it `aria-current="page"` rather than as a second call to action that navigates away. Rail 50 / 50. Crumb: Feld / Begin.

Posture: **The letter you send**, per Layout. Use Field components for text, email, select, radios, textareas, and the checkbox. Use Chamber for the confirm. Use Slip for success and error. Copy and labels verbatim. Do not add a password, a phone number, a newsletter, or a chatbot.

Client-side only. Success path waits 600ms then shows the close. `?fail=1` shows the error slip and preserves input. No analytics events.

Acceptance: tab order follows the fields then the stamp; errors are text plus `aria-invalid`; the chamber traps focus and Escape returns to the stamp without sending; success moves focus to the closing headline; both ledgers; the promise checkbox is a full sentence; colophon present; no hex in the page; this is page 50 of 50 in the rail.

When this page is done, the quire is complete. Do not invent a page 51.
