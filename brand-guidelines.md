# Health Flare brand assets — v2.0 (November 2026)

The full guidelines live on the Health Flare Brand Guidelines canvas; this is the short version for contributors. v2.0 replaces v1.0 (the open-ring mark) entirely.

## The system
- **The mark**: a sun meeting still water. Three parts: the sun, the horizon (the cut) and the reflection (the lower slice, split once). Always one colour.
- **The brand moment**: an open sun with a spark lifting free, on a horizon with tapering reflections. It's a graphic for large surfaces, never a logo.

The mark carries the name and the moment carries the feeling.

## Optical sizes (pick the file; don't scale across ranges)
| File | Range | Construction | Use for |
|---|---|---|---|
| `full` | 64px+ / 20mm+ | horizon cut 7% of width, reflection split in two | splash, web, print, merch |
| `compact` | 24–63px / 8–20mm | both cuts open to 9% | app icons, nav, lockups |
| `micro` | ≤23px | one cut only, 11% | favicon, notifications, status bar |

## Clear space and minimums
- x = one quarter of the mark's width. Keep x clear on all sides of the mark and lockups.
- Minimums: mark 16px / 5mm · horizontal lockup 120px / 30mm wide · stacked 80px / 20mm wide.

## Lockups
- Horizontal (default): compact mark at 1.3× wordmark cap height, gap = 25% of mark width.
- Stacked: full mark above, centred.
- Products: "Inner Flare" + "by Health Flare".
- Wordmark is Fraunces 500. Outlined lockup files are still to be produced; don't typeset it live in final artwork.

## Colour
| Name | Hex | Role | Notes |
|---|---|---|---|
| Sunrise | #E0694E | Health Flare primary | white on it 3.3:1, marks and 24px+ type only |
| Rose | #D2546E | Inner Flare primary | white on it 4.0:1, marks and 24px+ type only |
| Amber | #F2A33A | the mark on dark grounds | 8.1:1 on Ink; never on light grounds |
| Ink | #221C18 | text, dark ground | 15.8:1 on Dawn |
| Slate | #6B5E54 | secondary text | 5.9:1 on Dawn |
| Ember | #B4502F | links, Health Flare text accent | 4.8:1 on Dawn |
| Deep Rose | #B0404F | Inner Flare text accent | 5.3:1 on Dawn |
| Dawn | #FBF7F2 | light ground | |
| Sand | #F3E9DD | surfaces | |

The mark is always one colour: no third colour in the horizon, and no recolouring of parts. No clinical blues.

## Typography
Fraunces (wordmark, display, headings) · DM Sans (interface, body, labels, numbers). Both OFL. Sentence case.

## Product family
Every app shares the horizon and reflection; only the shape above the line changes, and each app takes its own warm colour.
- Health Flare: the sun · Sunrise
- Inner Flare: a flame with its tip leaning right (so it never reads as a water drop) · Rose. In the brand moment the flame has two tongues and rises through the opening.

## Large displays: schemes
One ground plus one mark colour per composition.
- **Dawn** (Sunrise on Dawn): default
- **Sunrise** (white on Sunrise): bold moments
- **Dusk** (Amber on Ink): night and rest
- **Sand** (Ink on Sand): print
- **Rose** (white on Rose): Inner Flare

In wide formats the moment's horizon may run to the edges.

## App icons
1024px masters in `app-icons/`. Compact mark at 60% of the width, centred. iOS: no transparency, no pre-rounded corners. Android adaptive: keep the mark inside the 66dp safe zone; use `*-android-monochrome` for themed icons. Below 40px use the micro mark.

## Functional / status colours (v2.1, addendum)

The nine colours above are the **identity system** — nav, buttons, headers, the
mark, text. They are not enough to run a product that has to signal severity,
success, or a destructive action at a glance, and forcing those jobs onto
identity colours causes real problems: a "moderate symptom" chip in the same
hue as the primary CTA reads as "tap this," and a flattened severity scale
loses the at-a-glance legibility that's the whole point of a traffic-light
indicator.

So this is a second, separate palette for **functional UI signalling only**.
It is deliberately exempt from "no clinical blues" and "always one colour" —
those rules exist to protect the *mark's* identity, not to constrain status
UI that never touches the mark. Don't use these colours for anything brand
(nav, CTAs, headers) and don't use the identity colours for anything
functional (severity, success, destructive) — keep the two systems visually
non-overlapping on purpose.

| Token | Hex | Job | Notes |
|---|---|---|---|
| `flare.clear` | `#BFCBAE` | Severity: clear / calm | Ink text, 9.9:1 |
| `flare.mild` | `#F0D28A` | Severity: mild | Ink text, 11.5:1 |
| `flare.moderate` | `#E8A94A` | Severity: moderate | Ink text, 8.2:1. Deliberately distinct from Sunrise/Amber — must never look like the primary CTA colour |
| `flare.significant` | `#D1683F` | Severity: significant | Ink text, 4.6:1 |
| `flare.severe` | `#A8402C` | Severity: severe | White text, 6.1:1 |
| `destructive` | `#7A2E24` | Delete / irreversible actions only | White text, 9.4:1. Darker and more desaturated than `flare.severe` on purpose — a delete confirmation should not visually echo a severity flag |
| `info` | no dedicated hue | Informational banners, links | Use Sand background / Slate icon or label / Ink text instead of a coloured banner. Info gives up its hue entirely rather than get a brand-safe substitute — if that reads as a loss of signal in practice, revisit |

This scale was designed for Health Flare's 5-step symptom severity model. If
Inner Flare (or anything else) needs a functional palette for a different
number of steps or a different signal, extend this table — don't invent a
third, undocumented palette per app.

## Profile tag colours (v2.2, addendum)

A third, even narrower palette: colours used ONLY to tell multiple profiles
apart at a glance (e.g. avatar background when there's no photo — a parent
tracking themself plus two kids needs each one visually distinct). This is
not identity, and it is not functional/status — it carries no meaning beyond
"a different person than that other one." Don't reuse identity or functional
colours for this job either; a profile that happens to land on the same hue
as "severe" or as the primary CTA creates a false association.

Eight deliberately muted, deliberately earth-toned swatches, spread across
hue so adjacent profiles are never confusable, all well clear of white-text
contrast minimums:

| Token | Hex | White-on-it |
|---|---|---|
| `profile.brick` | `#762D33` | 9.6:1 |
| `profile.clay` | `#76322D` | 9.3:1 |
| `profile.rust` | `#763D2D` | 8.5:1 |
| `profile.cedar` | `#76492D` | 7.6:1 |
| `profile.walnut` | `#76542D` | 6.8:1 |
| `profile.ochre` | `#76602D` | 6.0:1 |
| `profile.honey` | `#766B2D` | 5.4:1 |
| `profile.olive` | `#76762D` | 4.8:1 |

Assignment is deterministic (e.g. keyed off a profile id, cycling through
the list) — not user-chosen, not meaningful, just a stable visual tag.

## Don't
- stretch, rotate, or add effects
- add a colour to the horizon
- run the horizon past the sun (it reads as Saturn)
- narrow the reflection (it reads as ice cream)
- recolour parts, or use blues
- place it on busy backgrounds
- use the full mark below 64px
- retype the wordmark
- use the moment as an icon

## Status
These are construction-accurate drawings. Before a public 1.0, a designer should do a final optical pass (overshoot, the flame's curve, cut weights at each size) and produce outlined wordmark lockups.
