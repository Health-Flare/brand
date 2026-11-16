# Health Flare brand

Canonical source for the Health Flare brand system: the mark, the brand moment,
colour, typography, and the production asset kit. This is where the brand lives —
`app`, `InnerFlare`, `website`, and any other surface absorb only the subset of
files they actually use, copied in at a pinned tag. Nothing here should be
duplicated in full into a consumer repo.

- Guidelines: [`brand-guidelines.md`](brand-guidelines.md) — the short-form
  contributor guide (optical sizes, clear space, colour, typography, do/don't).
- Assets: [`assets/`](assets) — marks, the brand moment graphic, app icon
  masters, and favicons, per the structure below.
- Trademark status: [`TRADEMARKS.md`](TRADEMARKS.md).

## Structure

```
brand-guidelines.md          canonical guidelines doc
assets/
  marks/                      <product>-mark-<size>-<colour>.svg
                               size: full | compact | micro
                               colour: sunrise/rose (primary) · amber · ink · white
  moment/                      <product>-moment-<colour>.svg  (large-surface graphic, not a logo)
  app-icons/                   1024px masters, incl. dark and Android monochrome variants
  favicon/                     favicon.svg, PNG sizes, apple-touch-icon
```

## How a consumer repo should use this

1. Work out what that surface actually renders — an app only needs its own
   product's icon + the mark sizes/colours its UI themes use; a marketing site
   needs favicons, both products' marks, and the moment graphic; most repos
   need none of the other product's assets.
2. Copy only those files into `docs/brand/assets/...` in the consumer repo,
   under a short `docs/brand/README.md` that names the source tag (e.g.
   `Health-Flare/brand@v2.0.0`) and links back here for the full rules.
3. Don't copy `brand-guidelines.md` in full into a consumer repo. Link to it.
   If a repo genuinely needs a quick-reference (e.g. just the colour table),
   write a short excerpt and say explicitly it's an excerpt of this doc.
4. When this repo cuts a new tag, re-sync the specific files each consumer
   already carries — don't re-absorb the whole kit.

## Versioning

Releases are tagged (`v2.0.0`, ...). v2.0 replaces v1.0 (the open-ring mark)
entirely — there's no visual continuity to preserve, so don't mix v1 and v2
assets in a consumer repo.

v2.1 is additive: it introduces the "Functional / status colours" section in
`brand-guidelines.md` (severity scale, destructive, info) as a second palette
alongside the v2.0 identity system, for apps that need to signal severity or
destructive actions without borrowing identity colours for the job. No marks
or identity colours changed.

## Status

These are construction-accurate drawings, not final production art. Before a
public 1.0 of the system itself: a designer needs to do the optical pass
(overshoot, the flame's curve, cut weights at each size) and produce outlined
wordmark lockups (Fraunces 500 — don't typeset it live in final artwork today).
