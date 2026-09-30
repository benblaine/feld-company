# Feld Company

A speculative enterprise website for the deployment layer: the work of installing AI agents into how a large organization actually operates, and remaining while the models change.

The firm is fictional. The brief is not. Aaron Levie described the opening in a public post (the one supplied with this project): changing enterprise workflows is heavier than anyone prefers; the applied layer shows up as software, as agents, and as new kinds of services firms; the work runs from legacy systems to living evals to the next model release; traditional integrators will adapt unevenly; this is a good time to be a forward-deployed engineer, or a firm of them.

This project drafts the company that would take that work. It is a copy deck, a visual system, and a set of build prompts. It is not a claim that Feld Company exists, and the field records are composites.

## What is in here

| Path | What it is |
|---|---|
| `BRAND.md` | Name, position, the conjecture, the offer, the cast |
| `STYLE.md` | Style guidelines: type, color, layout, motion, imagery, components |
| `VOICE.md` | How the site is allowed to sound |
| `SITEMAP.md` | All 50 routes, in order |
| `CHROME.md` | Mast, footer, and colophon used on every page |
| `design-system/tokens.css` | The token system as CSS variables |
| `design-system/PROMPT.md` | Master prompt: build the Instrument component library |
| `pages/01`–`pages/50` | One packet per page: copy, layout, and a build prompt |
| `prompts/` | The same prompts extracted, for pasting into an AI on their own |

## How to use a page

Each file in `pages/` is a packet.

1. Read the **Copy** as the site’s words. An implementing model should set them as written.
2. Read **Layout** as the composition for that page only. The fifty pages are not one template with the nouns swapped.
3. Paste **Prompt** into an AI that has also been given `design-system/PROMPT.md`, `STYLE.md`, and `VOICE.md`. The extracted copy in `prompts/` repeats the copy, so a single file is enough if the style guide is attached.

Build the library once, from the master prompt, then build pages against it. Page prompts assume Instrument already exists.

## What this project deliberately is not

- A live React application. The prompts are the build. Running them is a separate job, one page or one library at a time.
- A client list. No real logos, no borrowed metrics, no unnamed “leading bank.”
- A medical, legal, or benefits product. On those pages the agent drafts and a qualified person releases.

## Stack the prompts ask for

React, TypeScript, Tailwind CSS (tokens as CSS variables, not a second palette in the config), and Storybook-style stories for every component. Dark mode is a first-class ledger: Day and Night, both designed, neither an invert filter.
