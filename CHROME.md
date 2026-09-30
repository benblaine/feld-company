# Chrome

Every page uses this mast, this footer, and this colophon. Page packets do not restate them. They state only the exceptions.

## Mast

Wordmark links home: **Feld**

Links, in order:

1. The Work → `/method`
2. Industries → `/industries`
3. Scale → `/scale/global`
4. Records → `/records/claims`
5. Firm → `/firm`
6. Journal → `/journal`

Then the ledger toggle: **Day ledger** / **Night survey**.

Then a primary stamp: **Begin** → `/begin`.

At palm width, the six links move into an Index chamber. The stamp and the toggle stay visible.

The Work’s children, for the index and for any section listing, in labor order:

Passage `/work/passage`, Access `/work/access`, Bindings `/work/bindings`, Redraw `/work/redraw`, The Loop `/work/the-loop`, Living evals `/work/evals`, Weather `/work/weather`, Unlisted `/work/unlisted`. Also Method `/method` and Enablement `/enablement`.

## Footer

Four columns of text links, UI face, then the colophon across the full measure.

**Labors.** Passage, Access, Bindings, Redraw, The Loop, Living evals, Weather, Unlisted.

**The firm.** Firm, People, Careers, Security, Pricing, Begin.

**Writing.** Conjecture, Manifesto, Field records, Journal, Letters, Readiness.

**Scale and floors.** Industries, Global enterprise, Upper mid-market, Holding companies, Engagement, First ninety days.

Small line under the columns, mono index: `Feld Company · The deployment layer · Page NN of 50`

## Colophon

Set in text face, small size, `--fg-muted`, under a hairline, on every page:

> Feld Company is a speculative firm, written so the deployment layer would have a voice and a manual. The conjecture it quotes belongs to Aaron Levie. Field records are composites, shaped like the work and attached to no client. Portraits are not of real people, because the cast is invented.

No social row. No “made with” line. No newsletter. The begin stamp is the only ask, and the footer does not repeat it if the page already ends on one.

## Rail

On every interior page the rail shows the survey tick, then:

```
NN
/
50
```

NN is the page’s number from `SITEMAP.md`, in mono. Home shows the eight labors in the rail instead of a fraction, each as an anchor.

## Title and social

Browser title pattern is in `VOICE.md`.

If a social card is built: bone ground, the word FELD, the page’s h1 in display, no photograph, no gradient. 1200×630. Night card only if the sharer is in night; default the day card.

## 404 and refusal

If the implementer builds a 404, the h1 is “This page was never in the quire.” A secondary stamp returns home. It is not one of the fifty and does not take a number.
