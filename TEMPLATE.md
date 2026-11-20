# Template rules: "Whitewash" (Tinos)

Chosen by Elena on 2026-11-20 from three Tinos directions
(`mockups/tinos/tinos-directions.html`, direction 1). Brand brief: `ideas_future/13-brand-brief.md`.
These rules apply to every page of elenastamatelou.com, and later to the company site,
the newsletter, slides and other material.

## 1. Idea in one line

Whitewashed walls, Aegean blue, a Cycladic arch: calm, light, serious, with one warm touch.

## 2. Colours

Defined once as CSS variables on `:root`, and redefined for dark mode.
Every pair below was checked for contrast (WCAG AA: 4.5 for text, 3.0 for shapes).

| Token | Light | Dark (Aegean night) | Use | Contrast on bg (L / D) |
|---|---|---|---|---|
| `--bg` | `#FBFAF6` whitewash | `#0E1A2B` | page background | – |
| `--surface` | `#FFFFFF` | `#13233A` | bands, form panel | – |
| `--soft` | `#E6EFF8` | `#18304C` | "Let's talk" band, image backgrounds | – |
| `--line` | `#DCE3EA` | `#24384F` | rules, borders | – |
| `--text` | `#14233A` | `#EEF1F4` | body text, headings | 15.1 / 15.4 |
| `--muted` | `#55657A` | `#A9B6C6` | secondary text | 5.7 / 8.5 |
| `--accent` | `#1F5FA8` Aegean | `#7FB2E5` | links, buttons, key words in headlines | 6.2 / 7.8 |
| `--warm` | `#B9853A` Volax stone | `#D9A75A` | **shapes only** (dots, small marks) | 3.1 / 8.0 |
| `--warm-text` | `#8A5F1F` | `#D9A75A` | small labels/tags in ochre | 5.4 / 8.0 |
| `--pop` | `#B8326B` bougainvillea | `#E2689A` | one highlight per view at most (e.g. a data point) | 5.4 / 5.6 |

Rules:
- Blue carries the site; ochre and bougainvillea are spices. **Never more than one bougainvillea mark per screen.**
- `--warm` in light mode is too pale for text: use `--warm-text` for any ochre text.
- No gradients, no shadows: flat colour only.
- Dark mode follows the visitor's system setting, with a toggle; the choice is remembered.

**Rhymes with signatomics** (the shared family link): navy ↔ Aegean night, crimson ↔ bougainvillea,
ochre ↔ Volax stone, and the same heading font.

## 3. Fonts

| Role | Font | Weights |
|---|---|---|
| Headings, logo word | **Bricolage Grotesque** (shared with signatomics) | 600, 700 |
| Body, labels, buttons | **Source Sans 3** | 400, 600 |

- Body 18 px (17 px on phones), line height 1.6, line length max ~70 characters.
- Headings: h1 clamp(34–56 px), letter-spacing −0.02em; h2 30 px; h3 24 px. Sentence case, never all caps,
  except the small eyebrow line above the h1 (uppercase, 14 px, letter-spacing 0.06em, `--muted`).
- One accent phrase per headline may be set in `--accent` (e.g. "explained clearly.").

## 4. Shapes and the arch

- **The arch** (Cycladic doorway: straight sides, half-circle top) is the signature shape: the logo, the photo
  frame, and at most one more place per page. Not on every card.
- Buttons: pill shape (fully rounded). Primary = filled `--accent`; secondary = 2 px `--accent` outline.
- Chips ("Open to"): pill, 1 px `--line` border, small ochre dot before the text.
- Everything else has small or no radius (images: 0; form panel: 12 px).
- Lines over boxes: sections are separated by 1 px `--line` rules and bands of colour, not by cards with shadows.

## 5. Logo (to refine)

Working logo (chosen 2026-11-20, not final): **the Aegean window**, an `--accent` arch with a `--warm`
sun setting behind two `--bg` sea lines (`mockups/tinos/logo-options.html`, option B). Elena prefers it simple:
no data meaning added (the variants in `window-variants.html` were declined for now).
Next to it: the word-mark "Elena Stamatelou" in Bricolage Grotesque 600.
The logo must work at 16 px (favicon), in one colour, and in dark mode.

## 6. Photo

Until a photo exists, the arch on the home page holds a simple **Aegean horizon** drawing (sea, sun, one
dovecote shape) in the palette, not a grey placeholder. When the photo comes: natural daylight, not
a studio portrait, cropped to the arch.

## 7. Images and data drawings

- Small, flat data drawings (dots, lines, bars) in palette colours, on `--soft` squares, like signatomics.
- No stock photos, no stock icons, no AI-generated images, no emoji.

## 8. Layout

- Max content width 1080 px; side gutter 24 px (16 px on phones); no horizontal scroll at 360 px.
- Generous vertical space: sections 64 px apart (44 px on phones).
- Projects as **stories** (picture left, text right; stacked on phones), not a card grid.
- Every page ends with the same two doors: **Let's talk** (form) and **the monthly letter**.

## 9. Words

- Voice: clear, calm, honest, warm; "I" and "you"; short sentences; no hype words.
- Say what the data cannot show, too.
- Never on the site: acting; the Greek company (until something is sold); confidential data,
  manuscripts under review, participant data.

## 10. Checks before release

Run the `site-architecture-audit` skill: rules check + visual check at 360, 768 and 1280 px, light and dark.
