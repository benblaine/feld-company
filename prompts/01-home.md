# Build prompt 01 — Home

Paste this file to an AI together with:
`design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

The Prompt section at the bottom is the instruction. The Copy section is verbatim site text and must be set as written. The Layout section is the composition.

---

# 01 — Home

Editor note: speculative firm. Copy below the rule is what the site says.

| | |
|---|---|
| Route | `/` |
| Story | `Pages/Home` |
| Section | Arrival |
| Rail | The eight labors, not the fraction |
| Posture | Reticle |

## Copy

**Browser title:** Feld Company — The deployment layer

**Meta description:** Feld installs AI agents into the work enterprises already run, and remains while the models change. Passage, access, bindings, redraw, the loop, living evals, and weather.

**Eyebrow:** Feld Company · The deployment layer

**Headline:** Install the work. Remain for the weather.

**Dek:** A model can be bought in an afternoon. The workflow it has to enter was built over decades, by people who will still be here on Monday. Feld is the firm that does the long part.

**Primary stamp:** Begin a deployment

**Secondary stamp:** Read the conjecture

### The long part

Moving the old system into reach. Setting access so an auditor can see it. Binding the software the company already runs. Redrawing the workflow so the agent has a job and a visible way to be wrong. Naming the human who releases the output. Writing evals that stay alive after the kickoff. Returning when the model changes.

The amount of that work is larger than the demonstration suggests. Feld is built to do it, and to stay.

### Three ways the work arrives

**By industry.** A claims floor and a shift log ask for different sentences. The doctrine holds. The floor changes.

**By size.** Fifty thousand people and eight hundred people do not fail in the same week. The install is cut to the company that has to live with it.

**By the problem inside the building.** Some need the old system lifted into reach. Some already live in the cloud and still cannot say who is allowed to let an agent's draft leave.

### Work output, placed in a process

The applied layer will look like software, and like agents, and like firms that remain. Feld is that third shape. We are hired when a company has moved past the demonstration and needs the work itself to change: a record of what the agent did, a person responsible for release, and a plan for next quarter's model.

### From the conjecture

> With AI agents, you're delivering actual work augmentation to the organization, which has a completely different set of complexities associated with it. You're no longer deploying tools that the company is merely enabled by, you're deploying work output in a process.

Aaron Levie, in the public post this firm is drafted from. The margin notes are ours. The sentences in the quote are his.

### And the list may be longer

Passage, access, bindings, redraw, the loop, evals, weather. Then the deputy, the quarter-end freeze, the bonus plan, the person who knows the exception by first name. That longer list has its own page, because it is where installs actually stall.

### Close

A good time to be the person in the building.

**Stamp:** Begin a deployment
**Text link:** See the first ninety days

## Layout

Posture name: **Reticle**.

Full viewport first screen. Background `--bg`. No photograph. No product mock. The survey tick sits large, about 96px, in `--signal`, top-left of the gather, aligned with the headline's cap height.

Left rail, unusually, is the labor index: 01 Passage through 08 Unlisted, each a text link in mono index, brass tick on the current hover. This replaces the page fraction on this page only.

Headline is `--text-display`, measure `--blade`, two lines as broken in the copy. Dek is `--text-lede` in Newsreader, max 42ch, under the headline, not beside it.

The two stamps sit in a cluster under the dek, primary then secondary. They do not stick to the bottom of the viewport.

Below the fold, "The long part" is a single Measure, body width, no cards.

"Three ways" is a Gather of three columns on desk, one on palm. Each column is a Ticket without a border: a brass numeral 01–03, an h3, and the paragraph. Hairline only on the top of each column.

The quote is set in Fraunces at `--text-h2`, wonk 1 (the only wonk on the site besides the conjecture page), measure 28ch, with attribution in mono index underneath. A patina rule, 48px wide, above the quote.

The close is a full-bleed `--bg-raised` band, headline at h2, stamps left aligned, generous `--space-10` vertical padding.

Night: the tick and the quote's rule become phosphor. The raised band becomes `--night-2`. No other color events.

Storybook: `Pages/Home` day, night, and palm (390px). The story supplies no extra sections.

## Prompt

You are a senior design systems engineer building one page of the Feld Company site on top of the Instrument library. Follow `design-system/PROMPT.md`, `STYLE.md`, `VOICE.md`, and `CHROME.md`. If they conflict with a generic landing-page habit, the files win.

Build the Home page at `/` in React and TypeScript. Story title: `Pages/Home`. Stories for day ledger, night ledger, and a 390px palm width.

Posture: **Reticle**, as specified in this packet's Layout. Home's rail is the eight labors, not the fraction. Mast and colophon come from `CHROME.md`. Active mast link: none. Begin stamp in the mast still goes to `/begin`.

Use the Copy section verbatim, including the Levie quotation and the attribution. Do not add a logo garden, metrics, a video, a chatbot, testimonials, or a fourth "way the work arrives." Do not rewrite headlines to be shorter. The period in "Install the work." stays.

Components: Quire, Mast, Gather, Measure, Stack, Stamp, Ticket-style columns (you may compose these from Stack and type tokens if Ticket assumes a link wrapper — these columns link: industry to `/industries`, size to `/scale/global`, problem to `/method`). The quote is a `blockquote` with `cite`. Links: conjecture `/conjecture`, ninety days `/ninety-days`, unlisted `/work/unlisted`, begin `/begin`. Labor rail links to the eight labor routes in `SITEMAP.md`.

Tokens only. Fraunces wonk 1 on this quote and nowhere else on this page. Phosphor only when `data-ledger="night"`. Respect reduced motion. Keyboard: stamps, labor links, mast, and toggle are reachable, and focus rings use `--focus`.

Acceptance: the colophon is visible; the page has no hex values; both ledgers look designed; at palm the labor rail moves into the Index chamber under a heading "The work", and the headline fits without overflow.
