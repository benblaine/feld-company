# 07 — People

Editor note: every person below is invented for this draft. Do not generate photographic portraits. The site copy does not apologize for their existence; the colophon carries the fiction.

| | |
|---|---|
| Route | `/people` |
| Story | `Pages/People` |
| Section | Firm |
| Rail | 07 / 50 |
| Posture | Roster |

## Copy

**Browser title:** People — Feld Company

**Meta description:** The cast of a pod-sized firm: principals for deployment, evals, bindings, cartography, the loop, premises, and the floors we know.

**Eyebrow:** The firm · Cast

**Headline:** Ten people, and the seats a pod actually needs.

**Dek:** Names here are the seats we staff. A deployment borrows two or three of them, not the whole roster. Click a name. The note is short on purpose.

### Roster

**Adaeze Okonkwo — Managing Principal.**
Writes the engagement and signs the refusal. Spent a decade inside other firms' programs watching go-lives stand in for handbacks. Holds the rule that Feld stays the size of its keepers.

**Jonah Voss — Head of Forward Deployment.**
Builds the binding and sits on the floor for shadow week. Former integrator who left when the work became a slide. Still reads other people's batch windows for pleasure, which is a kind of character.

**Ruth Pell — Keeper of Evals.**
Believes an eval without a decay date is a rumor. Started in quality on a payments floor, where "looks right" was not a control. Will stop a model upgrade in the weather log and sleep well.

**Samir Qureshi — Head of Bindings.**
Connects the system of record, the system of use, and the unofficial workbook. Treats single sign-on as a design problem. Keeps a private museum of interfaces that were certified and unused.

**Leila Hart — Head of Cartography.**
Draws the process before anyone is allowed to propose an agent. Interviews the person who knows the exception, not only the sponsor who named the process. Her maps have marginalia. That is the point.

**Naomi Berg — Principal, Financial and Insurance.**
Claims, close, KYC refresh, the control that will not move. Speaks fluent reserve note. Protects the firm from taking a capital-markets toy and calling it an operations practice.

**Tomasz Wójcik — Principal, Industrial and Energy.**
Permits, shift logs, outage desks. Mechanical engineer by training. Will not let an agent close a permit. Has a calm way of saying no in a plant that is behind on the quarter.

**Helen Cho — Principal, The Loop.**
Designs release, review, exception, escalation, and night. Previously built review desks for content that could hurt someone. Brings that seriousness to files that only hurt someone slowly: a claim, a benefit, a write-up.

**Idris Adeyemi — Principal, Premises and Security.**
Decides what may leave the building, which tenant an agent runs in, and which model is disqualified before the eval even sees it. Reviews every write-binding. Unmoved by haste dressed up as a pilot.

**Esther Marlow — Principal, Civic and Health operations.**
Intake, prior authorization packets, referral desks, the dignity constraint. A former caseworker. The sentence she will not let the firm drop: the person the file is about can see why.

### A note on portraits

You will not find photographs of these people. The work is the face we are willing to show. If you need a human counterpart before a letter, ask in the letter. A principal writes back.

### Close

Two or three of these seats form a pod. The roles we hire for are described without romance.

**Stamp:** See the roles
**Text link:** Write to the firm

## Layout

Posture: **Roster.**

A single column of names at display size `--text-h2`, each a button that opens a Chamber (role `alert` or a light confirm without danger) containing the note and a close stamp labeled "Close". The seat title sits on the same line in UI face, `--fg-muted`, or directly under the name at palm.

The list is not cards in a grid of headshots. It is an index, like a playbill. Hairline between names. A brass index number 01–10 in mono at the left gutter.

Opening headline and dek in blade measure above the list. "A note on portraits" is a short Measure under the list, `--fg-muted`. Then the close.

Chamber contains only the note for that person, the name as the dialog title, and Close. No social links. No "view profile" to a page that does not exist. All ten notes are in the page, so this is one page, not ten routes.

Keyboard: each name is a button, Enter opens, Escape closes, focus returns to the name.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/people`. Story: `Pages/People`, day, night, palm, and a story with one chamber open. Mast active: Firm. Rail 07 / 50. Crumb: Feld / Firm / People.

Posture: **Roster**, per Layout. Copy verbatim. Do not generate faces. Do not add LinkedIn glyphs. Do not split into ten URLs.

Stamp to `/careers`. Text link to `/begin`. Chambers are native dialogs, focus trapped, focus restored, Escape closes.

Acceptance: ten names in source order; the open chamber's title is the person's name; background is inert (`inert` or dialog semantics) while open; night ledger keeps the playbill typographic; no hex; colophon present; the portrait note is visible without opening a chamber.
