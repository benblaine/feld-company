# Build prompt 02 — The conjecture

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 02 — The conjecture

Editor note: the quoted paragraphs are Aaron Levie's, from the public post supplied as this project's brief. The margin notes are Feld's and may be set as site copy. Do not tighten or paraphrase the quotation.

| | |
|---|---|
| Route | `/conjecture` |
| Story | `Pages/Conjecture` |
| Section | Foundation |
| Rail | 02 / 50 |
| Posture | Margin gloss |

## Copy

**Browser title:** The conjecture — Feld Company

**Meta description:** The public post by Aaron Levie that Feld treats as a founding text, set with the firm's margin notes beside each movement.

**Eyebrow:** Foundation · A founding text

**Headline:** The deployment layer, said plainly.

**Dek:** Feld did not invent this opening. Aaron Levie wrote it down. We set the post here in full, and we write in the margin what a firm would have to be in order to take the work seriously.

**Kicker under the dek:** Aaron Levie · public post · the text supplied as this firm's brief

### I

> There's a huge opportunity right now in being the deployment layer for AI into the economy. The amount of work it takes to change out workflows in enterprises tends to be far greater than anyone realizes or would prefer. Clearly this is what the applied layer of AI is going to look like in the form of software and agents, but also it opens up new services firms opportunities.

**Margin:** The opportunity is a layer, which means it sits between a model and a Monday morning. Software will be part of it. Agents will be part of it. So will firms whose job is the changing of the workflow, which is the part everyone hopes will be small. It will not be small. Feld is a services firm of that kind, with enough engineering in the pod to do the binding and enough patience to remain.

### II

> Legacy systems need to be moved to the cloud, data organization and access needs to be updated, software needs to be connected to agents in new ways, workflows need to be reengineered for agents, HITL needs to be figured out for the process, evals need to be generated and maintained, and the entire system needs to be continually updated as new models get released and new capabilities emerge. And the full list may even be longer.

**Margin:** We name these so they can be staffed. Passage. Access. Bindings. Redraw. The Loop. Living evals. Weather. And a page called Unlisted, because he was right to leave the list open. An install that cannot point to an owner for each of these is a demonstration with a longer badge.

### III

> AI is not the same as just deploying software. Software you generally did the implementation of an existing, well understood category of technology, then stepped back and the customer kept running. With AI agents, you're delivering actual work augmentation to the organization, which has a completely different set of complexities associated with it. You're no longer deploying tools that the company is merely enabled by, you're deploying work output in a process. Completely different implementation and enablement process.

**Margin:** This is the sentence the rest of the site stands on. A tool leaves a customer enabled. Work output leaves a customer responsible for something newly alive: drafts in a queue, a person who releases them, a record, a way of being wrong. Enablement, for us, is the design of that responsibility. The page called Enablement stages one Tuesday both ways, so the difference can be felt rather than sloganed.

### IV

> As a result, this is going to open up lots of new kinds of firms and plays for existing firms to diffuse AI into organizations. We're going to see approaches by industry, by size of company, and by problem inside of companies. Traditional SIs will modernize and adapt (some will clearly not adapt as well), and new entrants will also be founded in this period that take advantage of this window. Great time to be an FDE or FDE firm.

**Margin:** Industry, size, and the problem inside the building are the three cuts of this website, not a marketing grid we invented later. Traditional integrators have a window of their own. We wrote them a separate essay, with respect, because some of them employ the best people on a given floor and will still miss the weather. New entrants will be founded in this period. Feld is a draft of one. The last line is the careers page, said by someone else, which is the right way to hear it.

### Close

The post ends. The work it names does not.

**Stamp:** Read the method
**Text link:** The eight labors, one by one

## Layout

Posture: **Margin gloss.** A scholarly edition, not a blog post.

Desktop: a two-column gather inside the quire. Left column span 7, the quotation in Newsreader at `--text-body`, each Roman-numeral section separated by `--space-8` and opened by a brass numeral. Right column span 4, offset by one column, the margin note in UI face at `--text-ui`, `--fg-muted`, aligned to the top of its quotation. A hairline between the columns. The margin column is sticky within each section only, so note II stays beside paragraph II.

The headline and dek are full measure above the two columns, blade width.

On palm: quotation, then its margin note in a `--bg-raised` block directly underneath, labeled in mono "Margin". No side column.

Do not style the quotation as a tweet screenshot. No avatar, no verified badge, no social counts. The attribution kicker is enough.

Night: margin notes stay muted. The hairline holds. Phosphor appears only on links and the stamp.

## Prompt

You are a senior design systems engineer building one page of the Feld Company site on the Instrument library. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, and `CHROME.md`.

Build `/conjecture`. Story: `Pages/Conjecture`, day, night, and palm.

Posture: **Margin gloss**, per this packet's Layout. Rail fraction 02 / 50. Crumb: Feld / Conjecture. Mast: no active item, or "Journal" if you must mark a parent — prefer none. This page is foundation, not journal.

Set the Copy verbatim. The blockquoted paragraphs are Aaron Levie's and must be character-exact, including "HITL" and the parenthesis in the fourth paragraph. Margin notes are Feld's, labeled "Margin". Do not add commentary he did not get. Do not shorten the quote. Wonk stays 0 on this page; the home page holds the only display wonk.

Stamp links to `/method`. Text link is an anchor list or a text link to `/work/passage` with the visible words "The eight labors, one by one". Implement the four sections as an ordered set, not as cards.

Acceptance: at 1280px the notes sit beside the paragraphs they answer; at 390px they stack under them; the colophon remains; keyboard order is mast, then headline region, then each paragraph and its note's links, then footer. No tweet chrome. No hex in the component.
