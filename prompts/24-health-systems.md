# Build prompt 24 — Health systems

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 24 — Health systems

| | |
|---|---|
| Route | `/industries/health-systems` |
| Story | `Pages/Health` |
| Section | Industries |
| Rail | 24 / 50 |
| Posture | Release line |

## Copy

**Browser title:** Health systems — Feld Company

**Meta description:** Operational work around clinicians: prior-authorization packets, referral desks, coding queries. The agent drafts. A licensed person releases. Feld does not install the practice of medicine.

**Eyebrow:** Industries · Health systems

**Headline:** Draft the packet. Leave the practice of medicine to the person licensed for it.

**Dek:** Health systems are full of operational prose that sits around the clinical decision: packets assembled from five systems, referrals that leak, coding queries written in a hurry at the end of a clinic. That prose is the work we will enter. The decision is not.

### The packet

A prior-authorization packet is a hunt. The agent can gather what the policy asks for, from the systems the access design allows, and list what is missing. A person in the office releases the packet. If a clinical statement is required, a clinician writes or approves that statement. We do not install an agent that implies a diagnosis to make a packet smoother.

### The query

Coding queries and documentation questions are a correspondence between colleagues. An agent may draft the question in the house form, more completely than a tired afternoon allows. The coder or the clinician sends it. The eval watches for drafts that nudge the documentation toward a higher code. Those cases are refusal cases. They pause the queue.

### The release line

Every artifact this floor produces carries a visible line: who drafted, who released, and which seat's license or duty the release relied on. If we cannot print the line, we do not ship the artifact. Patients are not a test environment. Neither are the people who care for them, whose names would be on an error.

### What we decline here

Diagnosis. Triage that decides who is seen. Anything that speaks to a patient as if it were their clinician. A "copilot" sitting inside the encounter, unreviewed. If your letter describes those, we will say no, and we will say it quickly so you can find a firm with a different conscience or a different competence. Ours is operations, with the release line intact.

### Close

Name the packet, not the diagnosis. Name the person who releases it.

**Stamp:** Begin with a packet
**Text link:** Civic intake, where the duty of explanation rhymes

## Layout

Posture: **Release line.**

Quiet, clinical in the typographic sense: lots of paper, no red crosses, no heartbeat line, no stock photo of a corridor. Headline and prose in a letter measure so the page reads as a policy note.

The release line is a designed specimen under the third section, full width of the measure, `--bg-sunken`, mono label "Release line" and then, in text face: "Drafted by the packet agent · Released by M. Okoye, authorization office · Clinical statement approved by the ordering clinician, not by the agent."

Mark the specimen "Composite example."

A danger stamp is not used. Decline is prose, not a red button.

Stamp (primary, ordinary) `/begin`. Text link `/industries/civic`.

## Prompt

You are a senior design systems engineer building one page on the Instrument library for Feld Company. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`.

Build `/industries/health-systems`. Story: `Pages/Health`, day, night, palm. Mast active: Industries. Rail 24 / 50. Crumb: Feld / Industries / Health systems.

Posture: **Release line**, per Layout. Copy verbatim, including the refusals. Do not add medical advice, symptom lists, or imagery of patients. The specimen sentence is exact.

Stamp `/begin`. Text link `/industries/civic`.

Acceptance: the decline section is present and unsoftened; the release line specimen is visible; no medical iconography (no crosses, hearts, ECG); both ledgers; colophon; no hex.
