# Contributing

This repo holds the brand system, not application code. Most changes here are
design changes, not engineering ones.

## Proposing a change

- Open a PR. For anything beyond a typo fix in the guidelines doc (new colour,
  new optical size rule, a new product mark, reworked lockup), flag it for
  design review before merging — these assets get copied into multiple
  consumer repos and a bad merge propagates.
- Keep `brand-guidelines.md` as the single canonical doc. Don't fork
  per-product copies of it in this repo.
- New or changed asset files follow the existing naming convention:
  `<product>-<kind>-<size-or-variant>-<colour>.<ext>` (see `README.md`).

## Cutting a release

1. Merge the change.
2. Tag it (`git tag vX.Y.Z && git push origin vX.Y.Z`). Bump major for a
   visual system change (like v1 → v2), minor for new assets/colours, patch
   for fixes to existing files.
3. Note which consumer repos (`app`, `InnerFlare`, `website`, ...) need to
   re-sync which specific files — open a tracking issue or PRs against them
   rather than expecting them to notice.

## What NOT to do

- Don't add files no consumer has asked for yet "just in case" — keep this
  repo to what's actually in use or explicitly planned.
- Don't let a consumer repo's `docs/brand/` drift into holding its own
  modified copy of an asset. If a surface needs something the kit doesn't
  have, add it here first.
