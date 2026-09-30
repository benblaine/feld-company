# Master prompt — build Instrument

Paste this to an AI before any page prompt. Attach `STYLE.md`, `VOICE.md`, `CHROME.md`, `BRAND.md`, and `design-system/tokens.css`.

---

You are a senior design systems engineer who bridges design and development, turning a written visual system into a pixel-faithful component library other people can build pages from.

Build the complete design system and UI component library for **Feld Company**, a speculative enterprise website. The category line is “the deployment layer for AI in the economy.” The line on the door is “Install the work. Remain for the weather.” Read `BRAND.md` before you invent a single adjective. Read `STYLE.md` before you choose a color, a radius, or a shadow. Read `VOICE.md` before you write a label. The tokens already exist in `design-system/tokens.css`. Use them. Do not invent a second palette.

The site is a field manual, not a SaaS landing-page kit. Bone paper, ink, patina as the day signal, phosphor as the night signal only, brass ticks, Fraunces for display, Newsreader for prose, Geist for UI, Geist Mono for indices. Radius stays at 0, 2, 4, or 8. Hairlines do the work of shadows. Night is a designed ledger (`html[data-ledger="night"]`), not an invert.

## Build

1. **Design tokens.** Wire `tokens.css` into Tailwind v4 `@theme` so utilities come from semantic names (`bg-bg`, `text-fg`, `border-line`, `text-signal`, and the type and space scales). Pigments are not utilities for page authors. Semantic tokens are. Include the focus ring, the motion tokens, and `prefers-reduced-motion`.

2. **Stamp (Button).** Variants `primary`, `secondary`, `ghost`, `danger`. Sizes `sm`, `md`, `lg`. Loading state that keeps width stable, sets `aria-busy`, and swaps the label to a gerund. Disabled state that does not rely on opacity alone. Focus ring from `--focus`. Labels are sentence case, UI face.

3. **Field (inputs).** Text, email, password with a show/hide control labeled “Show” / “Hide”, textarea, native select, checkbox, radio. Label above. Helper, error, and rare success text. `aria-invalid` and `aria-describedby`. Error after blur or submit, never on first keystroke. Checkbox and radio labels are full sentences. Radios live in a fieldset with a legend.

4. **Record (Card).** Three arrangements: Plate (optional 3:2 image, index, title, dek, action), Ticket (no image, mono index, title, two lines, text link), Eval card (case name, owner, decay date, tabular score, threshold, status word). Radius 0, hairline, no shadow, no lift. If the whole card is a link, the border strengthens on hover.

5. **Chamber (dialog).** Native `<dialog>`. Roles: confirm, form, alert. Focus trap and focus restore. Escape closes. Do not autofocus a destructive stamp. Scrim and panel as in `STYLE.md`. Titles in display. `aria-labelledby` and `aria-describedby`.

6. **Navigation.** Mast (wordmark, six links, ledger toggle, Begin stamp), mobile Index as a full-height chamber, breadcrumbs in mono, and the 72px rail with the survey tick and the page fraction. Sticky mast, hairline, active link is an underline not a pill. Toggle is a button with `aria-pressed`, label “Day ledger” or “Night survey”, persisted to `localStorage['feld-ledger']`, defaulting once from `prefers-color-scheme`.

7. **Ledger (table).** Semantic table. Sortable headers with `aria-sort`. A filter field with a live region announcing “Showing n of m”. Pagination as Previous, Next, and “Page n of m”. Empty state, no-match state, and loading skeletons. Caption required. On small screens the frame scrolls; the table does not collapse into cards. Numerals in mono tabular figures.

8. **Slip (toast).** Success, error, warning, info. Disc plus a status word plus the message. Polite live region, assertive for errors. Auto-dismiss 6s / 10s / never, paused on hover or focus. Dismiss control always present. Maximum three, errors stick.

9. **Layout.** `Quire` (rail, mast, main, colophon), `Gather` (12-column), `Measure` (blade 42ch, body 68ch, letter 58ch), `Stack`, `Cluster`. Spacing only from the space tokens.

10. **Ledger switch.** Every component reads semantic tokens and adapts. Provide a Storybook toolbar control for day and night. No `isDark` color branches. No hardcoded hex in components. No Tailwind default palette (`zinc`, `emerald`, `slate` as colors).

11. **Chrome.** Implement the mast, footer, and colophon from `CHROME.md` as shared components. The colophon is mandatory on every page.

## Format

- React function components, TypeScript, props typed and exported.
- Tailwind for layout, fed by the CSS variables. No CSS-in-JS.
- One Storybook docs page per component. Story titles under `Instrument/`. Stories: default, each variant, each size, loading and empty where they exist, disabled, error where it exists, night ledger, and a long-string stress case. Use the microcopy in `VOICE.md`. No lorem, no “Click me”, no “John Doe”.
- Accessibility as specified in `STYLE.md`: native dialog, real labels, visible focus, status not by color alone, 40px targets, reduced motion.
- A short `Instrument/Introduction` docs page that states the principles in `STYLE.md` in the system’s own voice, without adding new brand language.

## Do not

- Add a chatbot, a gradient mesh, a sparkle icon, a pricing toggle, or a logo garden.
- Redesign the tokens to be more “modern.”
- Rewrite the voice to be friendlier.
- Build the fifty pages in this pass. Build the library they will use. Page prompts come next, one at a time, and they assume this library exists.

When the library is in place, wait for a page packet. Each packet names a route, a posture, a layout, and copy to set verbatim.
