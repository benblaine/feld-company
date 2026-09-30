# Instrument — style guidelines

Instrument is Feld Company’s design system. It should feel like a surveyor’s field book typeset by a contemporary serif foundry: bone paper, ink, a patina signal, brass ticks, and a phosphor reticle that appears only at night. It should not feel like a SaaS template, a purple AI gradient, or a consultancy deck with the logo enlarged.

The system is for a marketing and doctrinal site, not a product console. Components still have to be complete, because the pages use them: forms on Begin and Readiness, ledgers on the eval and weather pages, chambers for confirmations, slips for acknowledgement.

## Principles

1. **The page is a document.** Hairlines, indices, and a measure do the work that drop shadows do on other sites.
2. **One signal color is on duty.** Patina by day. Phosphor by night. Brass is for ticks and large numerals, not for buttons.
3. **Type does the branding.** If the CSS loaded and the images failed, the page should still be obviously Feld.
4. **Each page has a posture.** Home is a reticle. The conjecture is a glossed edition. Shadow week is a notebook. Do not pour every page into a hero, three cards, and a testimonial.
5. **Night is designed.** Night survey is a second composition of the same tokens, not a filter and not an afterthought.
6. **Nothing decorative moves.** Motion is mechanical and short. A survey instrument does not bounce.
7. **The colophon is always present.** The firm is speculative. The records are composites. Levie is credited for the conjecture. This is a design constraint, not a footnote the implementer may drop.

## Color

Raw pigments never appear in components. Components use semantic tokens. Semantic tokens change with the ledger. Pigments do not.

### Pigments

| Token | Hex | Role |
|---|---|---|
| `--ink` | `#1a1916` | Day text, night ground’s cousin |
| `--ink-soft` | `#3a3834` | Day secondary text |
| `--bone` | `#efeae2` | Day ground |
| `--bone-2` | `#e4ddd2` | Day raised, strips, zebra |
| `--paper` | `#f7f4ee` | Day page, a step lighter than bone |
| `--patina` | `#1f6f62` | Day signal, links, focus when large |
| `--patina-deep` | `#16574d` | Day signal fill (buttons) so label text clears AA |
| `--brass` | `#8a6433` | Ticks, rules of emphasis, numerals at 24px and up |
| `--brass-ink` | `#6e4e24` | Brass that must be read below 24px |
| `--phosphor` | `#d6ff4a` | Night signal only |
| `--oxide` | `#9c3418` | Danger, day |
| `--oxide-deep` | `#7c2c12` | Danger fill, day |
| `--resin` | `#7a4e12` | Warning text, day |
| `--slate` | `#3e5366` | Info, day |
| `--night` | `#121410` | Night ground |
| `--night-2` | `#1c1e19` | Night raised |
| `--night-3` | `#262822` | Night sunken, tracks, code |
| `--night-ink` | `#ebe6dc` | Night text |
| `--night-muted` | `#b7b1a6` | Night secondary |
| `--night-brass` | `#c6a36a` | Night ticks |
| `--night-oxide` | `#f0b4a4` | Night danger text |
| `--night-resin` | `#e2b15a` | Night warning text |
| `--night-slate` | `#b7c7d6` | Night info text |

Patina `#1f6f62` on bone is 5.0:1. Use it for links and UI text at 16px or heavier. For a filled button, the fill is `--patina-deep` and the label is `--paper` (7.0:1). Brass `#8a6433` is 4.4:1 on bone: ticks and display numerals only. Readable brass text uses `--brass-ink`.

Phosphor is illegal as text or as a fill on any day surface. On a night surface it is the signal: links, the one primary stamp, the focus ring, the survey tick in the wordmark. Do not flood a night page with phosphor panels. A night page is still mostly bone-colored text on a near-black olive ground.

### Semantic tokens

Set on `:root` (day) and on `html[data-ledger="night"]`.

| Token | Day | Night |
|---|---|---|
| `--bg` | paper | night |
| `--bg-raised` | bone | night-2 |
| `--bg-sunken` | bone-2 | night-3 |
| `--fg` | ink | night-ink |
| `--fg-muted` | ink-soft | night-muted |
| `--fg-faint` | `#6b675f` | `#8a857b` |
| `--line` | `color-mix(in srgb, var(--ink) 14%, transparent)` | `color-mix(in srgb, var(--night-ink) 16%, transparent)` |
| `--line-strong` | ink | night-ink |
| `--signal` | patina | phosphor |
| `--signal-fill` | patina-deep | phosphor |
| `--signal-on` | paper | night |
| `--danger` | oxide | night-oxide |
| `--danger-fill` | oxide-deep | `#6e2c22` |
| `--danger-on` | paper | night-ink |
| `--warning` | resin | night-resin |
| `--info` | slate | night-slate |
| `--ok` | patina-deep | phosphor |
| `--focus` | patina-deep | phosphor |
| `--tick` | brass | night-brass |

`--fg-faint` is for indices and meta, and must still clear 4.5:1. `#6b675f` on `#f7f4ee` does. `#8a857b` on `#121410` does. If a new combination is introduced, measure it before it ships. Do not “fix” contrast by dropping opacity on text.

### Color behavior

- Links are `--signal`, underlined, underline-offset 3px. Underline is always visible, not only on hover.
- A second accent in a diagram is brass, used once, for the path under discussion.
- Status in a ledger: a 6px disc plus a word. Color is never the only carrier.
- Charts, if any page needs one, are rules and numerals. No donuts, no gradient fills, no grid-glows.

## Typography

Load these, in this order of preference:

| Role | Face | Fallback |
|---|---|---|
| Display | Fraunces (opsz 144, soft 50, wght 560) | Iowan Old Style, Palatino Linotype, serif |
| Text | Newsreader (opsz 16–72, wght 420) | Iowan Old Style, Palatino Linotype, serif |
| UI | Geist | Schibsted Grotesk, Avenir Next, sans-serif |
| Mono | Geist Mono | IBM Plex Mono, ui-monospace, monospace |

Fraunces **wonk** stays at 0 for headlines. Wonk 1 is reserved for the conjecture pull-quote and for nowhere else. The irregularity is a citation, not a brand twitch.

### Scale

Desktop. Mobile multiplies display sizes by 0.62 and leaves body alone.

| Token | Size / line / tracking | Face | Use |
|---|---|---|---|
| `--text-display` | 92 / 0.92 / -0.03em | Display | Home and manifesto only |
| `--text-h1` | 64 / 0.96 / -0.03em | Display | Page title |
| `--text-h2` | 40 / 1.05 / -0.02em | Display | Section |
| `--text-h3` | 26 / 1.2 / -0.015em | Display | Subsection |
| `--text-lede` | 22 / 1.45 / -0.011em | Text | The dek under an h1 |
| `--text-body` | 18 / 1.55 / 0 | Text | Prose |
| `--text-ui` | 15 / 1.4 / 0 | UI | Nav, buttons, labels |
| `--text-small` | 13 / 1.45 / 0.01em | UI | Meta, help |
| `--text-index` | 12 / 1.3 / 0.14em | Mono | Eyebrows, crumbs, ticks. Uppercase |
| `--text-num` | 13 / 1.4 / 0 | Mono, tabular | Tables, eval scores, dates |

Prose measure is 68 characters. Ledes may run to 42ch under a display headline so the line looks like a blade, not a paragraph. Do not justify. Hyphenate long words on display sizes (`hyphens: auto` with a lang of `en`).

Numerals in running text use the text face’s oldstyle figures if the font offers them. Numerals in UI, tables, and indices use mono tabular lining figures. A page may mix them: oldstyle in the essay, tabular in the margin.

## Space, radius, border, shadow

4px base. Tokens: `--space-1` 4, `--space-2` 8, `--space-3` 12, `--space-4` 16, `--space-5` 24, `--space-6` 32, `--space-7` 48, `--space-8` 64, `--space-9` 96, `--space-10` 144, `--space-11` 200.

Use the tokens. A one-off 20px padding is a bug.

Radius is nearly square, like a machined plate.

| Token | Value | Use |
|---|---|---|
| `--radius-0` | 0 | Editorial blocks, images, the page |
| `--radius-1` | 2px | Fields, ledger cells |
| `--radius-2` | 4px | Stamps (buttons), slips |
| `--radius-3` | 8px | Chambers |
| `--radius-round` | 999px | The 6px status disc and nothing else |

Borders:

| Token | Value |
|---|---|
| `--border-hair` | 1px solid var(--line) |
| `--border-strong` | 1px solid var(--line-strong) |
| `--border-signal` | 1px solid var(--signal) |

Shadows are rare. A hairline is the default edge.

| Token | Value | Use |
|---|---|---|
| `--shadow-0` | none | Almost everything |
| `--shadow-plate` | `0 1px 0 color-mix(in srgb, var(--fg) 8%, transparent), 0 24px 40px -28px color-mix(in srgb, var(--ink) 45%, transparent)` | Cards that genuinely float, slips |
| `--shadow-chamber` | `0 40px 80px -32px color-mix(in srgb, var(--ink) 65%, transparent)` | Modals |

No glow, except the focus ring. No colored shadow.

## Layout

The page wrapper is **Quire**.

```
┌────┬──────────────────────────────────────────┐
│rail│ mast                                      │
│72px│──────────────────────────────────────────│
│    │                                            │
│ 04 │   measure or gather                        │
│ /  │                                            │
│ 50 │                                            │
│    │                                            │
│    │ colophon                                   │
└────┴──────────────────────────────────────────┘
```

- The rail is fixed, 72px, bone-2 by day and night-2 by night, with a hairline on its right edge. Contents, stacked and centered: the survey tick, then the page index “04” over “50” in mono, then the ledger toggle as a vertical word if it fits, otherwise the toggle lives in the mast. Below 960px the rail disappears and its contents move into the mast and the mobile index.
- **Measure** is the prose column: max 68ch, centered in the remaining width, with at least `--space-7` of side padding.
- **Gather** is a 12-column grid inside a 1280px container (1440 on home). Column gap `--space-5`. Row gap `--space-8`.
- Home omits the numeric rail index and uses the labor list as the rail instead.
- A full-bleed image, when a page has one, breaks the measure and runs to the right edge of the viewport, never under the rail. One image per page is the maximum. Many pages have none, and that is preferred.
- Sticky subnavs are not used. The rail is the only sticky instrument.

### Breakpoints

| Name | Width | What changes |
|---|---|---|
| `desk` | ≥ 1200 | Full rail, display scale |
| `lap` | 960–1199 | Rail narrows to 56px, h1 drops to 52 |
| `palm` | < 960 | Rail gone, index becomes a chamber, display × 0.62, tables scroll inside a sunken frame rather than collapsing into cards unless the layout section says otherwise |

## Motion

| Token | Value |
|---|---|
| `--ease` | `cubic-bezier(0.2, 0.8, 0.2, 1)` |
| `--dur-quick` | 120ms |
| `--dur-ui` | 200ms |
| `--dur-page` | 360ms |

No overshoot, no spring, no parallax, no scroll-jacking, no typewriter, no counter that spins up from zero unless the readiness result is counting a score — and even there, prefer an instant numeral.

Page entrance, if any: opacity 0 to 1 and 8px of vertical travel over `--dur-page`. Under `prefers-reduced-motion: reduce`, opacity only, over 1ms effectively instant, and no travel.

The ledger toggle crossfades custom properties over `--dur-page`. Do not animate `background-color` on the entire DOM with a transition-all. List the properties.

## Imagery and iconography

**Photography.** Documentary, available light, 35mm feeling. Work, not lifestyle: a claims desk after hours, a permit clipboard, a yard at dawn, hands, paper, a screen seen from the side with no readable third-party UI. No one looks at the camera. No thumbs. No diverse-team-pointing-at-a-laptop stock. Grade as a duotone toward ink and bone, with patina allowed in the shadows at no more than 15%. If an image is generated, those are the constraints, and it must contain no real company’s name.

**Drawings.** Diagrams are engravings: 1px strokes, square ends, brass or patina for the single highlighted path, labels in mono. They are inline SVG, currentColor plus `var(--signal)`, so they survive the ledger switch.

**Icons.** 20px grid, 1.5px stroke, round caps, square joins except where a round cap is needed for the survey tick. Custom set, named: tick, passage, key, binding, redraw, loop, eval, weather, unlisted, stamp, sever, ledger, chamber, slip, index. Lucide is acceptable only if thinned to 1.5px and limited to this set’s meanings. No filled pictorial icons. No sparkles.

**Logo.** Wordmark “FELD” in Fraunces wght 560, tracking -0.03em. The D contains the survey tick in `var(--signal)`. Clear space equals the width of the E. On bone or night only. Never on a photograph. Never recolored to brass.

## Components

Names below are the engineering names. The brand nickname sits in parentheses for copy and story titles. Build all of them in the library before building pages. Stories live under `Instrument/…`.

### Stamp (Button)

Variants: `primary`, `secondary`, `ghost`, `danger`.
Sizes: `sm` 32px height, `md` 40, `lg` 48. Horizontal padding `--space-4` / `--space-5` / `--space-6`.
Label: UI face, 15px, no uppercase, no letterspacing tricks.
Primary: fill `--signal-fill`, label `--signal-on`, no border, radius `--radius-2`.
Secondary: transparent, `--border-strong`, label `--fg`.
Ghost: transparent, no border, label `--fg`, underline on hover.
Danger: fill `--danger-fill`, label `--danger-on`.
Loading: label swaps to “Working” or the page’s specified gerund, width stays stable (min-width captured before swap), a 1px arc at the inline end, `aria-busy="true"`, disabled.
Disabled: 40% opacity is forbidden. Use a sunken fill and `--fg-faint`, and keep the border. Always expose the reason outside the button.
Focus: 2px `--focus` ring, 3px offset. Visible on the night phosphor ring against night ground — add a 1px night-ink inner gap if the ring ever sits on a phosphor fill.
Hit area at least 40×40 even when the visible stamp is `sm`.

### Field (inputs)

Text, email, password (with a show/hide that is a ghost stamp labeled “Show”), textarea, select, checkbox, radio.
Label above, UI 13px, `--fg`. The input is 44px tall, radius `--radius-1`, background `--bg`, border `--border-hair`, text `--text-body` but UI face so forms don’t pretend to be essays. Textareas are text-face, because the begin form is a letter.
Focus: border becomes `--signal`, plus the focus ring.
Error: border `--danger`, message underneath in `--danger`, `aria-invalid`, `aria-describedby`. Icon plus text.
Success: only after a valid blur, a one-word “Usable” in `--ok`, never a party.
Helper text in `--fg-muted`, `--text-small`.
Checkbox and radio: 18px squares (checkbox) and circles (radio — the one allowed circle besides the status disc), 1.5px stroke, patina or phosphor fill when checked, label is a full sentence.
Select: native, restyled only as far as the border and the chevron. Do not rebuild a listbox unless a page prompt says so.
Groups of radios are fieldsets with legends.

### Record (Card)

Three arrangements, all radius 0, `--border-hair`, background `--bg-raised`, no shadow:

1. **Plate** — optional image (3:2, duotone, object-fit cover), then index, title in display h3, dek in text, a ghost or secondary stamp.
2. **Ticket** — no image. A mono index in the corner (“Labor 03”), title, two lines, a text link.
3. **Eval card** — a specimen used on the evals page and in stories: name of the case, owner, decay date, score as a tabular numeral, threshold, status word.

Hover, if the whole card is a link: the border becomes `--line-strong` over `--dur-ui`. No lift.

### Chamber (Modal and dialog)

Roles: `confirm`, `form`, `alert`.
Implement with the native `<dialog>` element. `showModal()` for the focus trap and the top-layer. Restore focus to the invoker on close. Escape closes alert and form; a danger confirm asks for an explicit cancel stamp and still allows Escape, because trapping a person in a modal is not seriousness.
Scrim: `color-mix(in srgb, var(--night) 64%, transparent)` in both ledgers.
Panel: `--bg-raised`, radius `--radius-3`, `--shadow-chamber`, padding `--space-6`, max-width 480px for alert and confirm, 640px for a form. Title in display h3. Body in text.
Alert has one stamp. Confirm has secondary “Back” and primary or danger for the commit. Form chamber contains fields and a footer row.
`aria-labelledby` the title. `aria-describedby` the body. Do not autofocus a destructive stamp; autofocus the cancel.
Stories must show keyboard open and close.

### Mast, Index, Crumb, Night menu (Navigation)

**Mast.** Height 72px, sticky, background `--bg` at 92% with a 8px backdrop blur, bottom hairline. Left: wordmark. Center or left-following: The Work, Industries, Scale, Records, Firm, Journal. Right: ledger toggle, then primary stamp “Begin”. At `palm`, the links collapse into an “Index” ghost stamp.
Active link: signal underline, 2px, full width of the word. Not a pill.
**Index.** The mobile menu is a chamber, full height, not a dropdown. It lists the same links plus the current section’s children. Close stamp labeled “Close”.
**Rail.** Described under layout. It is navigation for the page’s place in the quire, not a second menu.
**Crumb.** Mono index, on interior pages above the h1: `Feld / Work / Passage`. The current crumb is `--fg` and not a link. Separators are a slash with spaces, in `--fg-faint`.

### Ledger (Table)

Semantic `<table>`, width 100%, UI face for cells, mono for numerals and dates.
Header sticky inside the table frame, `--bg-sunken`, label in `--text-index`, a sort button inside the header cell with `aria-sort`.
Row hover: `--bg-sunken`. Selected row, if ever: a 2px signal inset on the row’s first cell, plus text.
Filter: a field above the frame, labeled “Filter the queue”, affecting a live region “Showing 12 of 40”.
Pagination: “Previous” and “Next” as secondary stamps, and “Page 2 of 9” in mono. Keep the query in the URL on pages that are real data. Specimen tables in stories may be local state.
Empty and no-match states: one row with a single cell, the copy from `VOICE.md`, left aligned, padding `--space-7`.
Loading: five skeleton rows, blocks in `--bg-sunken` with a 1.2s opacity pulse. Under reduced motion, static blocks. `aria-busy` on the table.
Caption required, visually available, even if it is the page’s kicker.
Do not turn the table into cards at palm. Scroll the frame. The first column can be sticky.

### Slip (Toast)

Region: `aria-live="polite"` for success and info, `assertive` for error. A list, bottom-left on desk (to avoid the begin stamp), top on palm, inset `--space-5`, max-width 360px.
Variants: success, error, warning, info. A 6px disc in the status color, a word (“Sent”, “Stopped”, “Decay”, “Note”), then the message in UI face.
Auto-dismiss in 6s for success and info. Warning 10s. Error does not auto-dismiss. Hover or focus pauses the timer. A ghost “Dismiss” is always present. `prefers-reduced-motion` skips the slide; the slip appears.
Do not stack more than three. A fourth replaces the oldest non-error.

### Quire, Gather, Measure, Stack (Layout)

- `Quire` renders rail, mast slot, main, colophon. Props: `index`, `section`, `ledger` is not a prop — the ledger is global state.
- `Gather` is the 12-column grid. Children declare `span`.
- `Measure` is the prose column. Prop `width`: `blade` (42ch), `body` (68ch), `letter` (58ch).
- `Stack` is vertical rhythm: `gap` from the space tokens only.
- `Cluster` is an inline row that wraps, gap `--space-3`, for stamps and meta.

Utilities, if exposed, are these and no more: the space scale as padding and gap, the grid spans, `tabular-nums`, and `sr-only`. Do not publish a second, looser utility layer that lets a page invent a new shadow.

### Ledger switch (Dark mode)

A toggle button in the mast, `aria-pressed`, label “Day ledger” or “Night survey”.
Persist `localStorage['feld-ledger']` as `day` or `night`. If absent, use `prefers-color-scheme`. Changing the OS preference while a stored choice exists does not override the stored choice.
Implementation: `data-ledger` on `<html>`, semantic tokens restated. Components do not mention hex and do not branch on a `isDark` boolean for color. An `isNight` boolean is allowed only where layout genuinely changes, which should be almost nowhere.
Storybook: a global toolbar control for the ledger, and a story for every component in both ledgers. The acceptance test is a screenshot pair, not a glance.

## Accessibility floor

- WCAG 2.2 AA. Body text aims at AAA and already clears it in both ledgers.
- Every control has a visible focus ring. Never `outline: none` without a replacement.
- Chambers trap and restore focus. Slips do not steal focus.
- Status is icon or disc plus text.
- Hit targets 40px.
- The mast’s begin stamp and the ledger toggle are in the tab order. The decorative survey tick is `aria-hidden`.
- Language `en` on the document. If a later page quotes another language, mark it.
- Reduced motion respected, as above.
- The readiness diagnostic and the begin form can be completed with a keyboard only, and errors are announced as a summary at the top of the form on submit.

## Storybook

Title prefix: `Instrument/`.
Every component story file includes: default, each variant, each size where sizes exist, loading or empty where the component has them, a disabled state, an error state where applicable, a night ledger story, and a long-string story (a German compound or a 40-character queue name) to prove the layout does not explode.
Docs page for each component starts with the sentence of what it is for, then the do and the don’t from this file, then the controls. No lorem. Use the microcopy in `VOICE.md`.

## What Instrument refuses

- Inter, Arial-as-a-brand, or a default system sans for display.
- Purple, electric blue, or a gradient mesh.
- Sparkle icons, node-graph hero illustrations, 3D glass blobs.
- Cards with 24px radius and a soft shadow as the default section pattern.
- Stock photography of handshakes, glass offices, or people pointing at charts.
- A chatbot widget.
- Autoplaying video.
- A cookie-consent carnival. If a consent line is required, one sentence in the colophon and a chamber with two stamps: “Use only what the letter needs” and “Accept measurement”. The draft ships with measurement off.
- Fake client logos.
- Any component that hardcodes `#fff`, `#000`, or a Tailwind palette color (`zinc-900`, `emerald-500`) instead of a semantic token. Tailwind is the engine. The tokens are the palette. Map them in `@theme` and then use those names only.
