# FDS 2026 — Blog Image Skill File
> Use this file as LLM context when generating blog cover images, OG images, and in-article visuals for Facilio.
> Patterns sourced from the FDS 2026 Figma file (node 33:8664).

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the blog image context.

---

## Colors

Three background modes are used across all templates:

| Mode | Colors | Used in |
|------|--------|---------|
| **Violet** | `violet-06` (#623cf6) full bleed | All cover images, some in-article |
| **Dark** | `charcoal-09` (#1d293d) or `charcoal-10` (#0f172b) | Most in-article dark variants |
| **Light** | `charcoal-01` (#f8fafc) or `charcoal-02` (#f1f5f9) | Card fills, light-bg in-article |

**Content cards** inside images always use `charcoal-01` or `charcoal-02` as fill (light grey rounded cards).
**Accent/highlight cards** are always `violet-06` filled — used for brand anchor cells in grids, arrow connectors, highlighted steps, and the "After" column in comparison tables.

**Semantic color use:**
- Positive / after state → green checkmark (`green-06`)
- Negative / before state → red or orange ✗/⊘ icon (`orange-07` or `red`)
- Stats and numbers → `violet-06` text
- Step numbers, icons → white on `violet-06` circle background

---

## Typography

| Element | Font | Weight | Color |
|---------|------|--------|-------|
| Title / headline | Darker Grotesque | 700–800 | `black` on light / `white` on dark or violet |
| Sub-title / descriptor | Darker Grotesque | 600 | `charcoal-07` on light / `white` on dark |
| Card title | Darker Grotesque | 700 | `black` on light card / `white` on violet card |
| Body / description text | Inter | 400 | `charcoal-07` on light / `charcoal-02` on dark |
| Stat / numeral | IBM Plex Mono | 600–700 | `violet-06` on any bg |
| Label / list item | Inter | 400 | `charcoal-08` on light / `white` on dark |
| Step number | Inter or Darker Grotesque | 700 | `white` on `violet-06` circle |

**Heading color rule:** Black on light backgrounds, white on dark and violet backgrounds. Never use grey for headline text.

---

## Logo

Always use the **classic** variant.
- On dark or violet backgrounds → `logos/classic/facilio-white.svg`
- On light/grey backgrounds → `logos/classic/facilio-dark.svg`

**Placement rules:**
- Split-layout templates → top-left of the left content panel
- Full-width center-title templates → top-center, above the title
- Never place the logo bottom-left or bottom-right — always top of the image

---

## Decorative Element

A **striped sphere / orb** shape appears bottom-left of the content panel in several split-layout templates. It is always dark-filled (near black) and serves as a decorative anchor. Use it in split-layout cover images and in-article templates that have a left content panel with empty lower space.

---

## Canvas Sizes

| Format | Dimensions | Aspect ratio | Use |
|--------|-----------|--------------|-----|
| **Cover / OG** | 1200 × 630px | ~1.91:1 | Blog cover image, Open Graph (Facebook, LinkedIn, social sharing) |
| **In-article** | 1200 × 880px | ~1.36:1 | Images used inside the blog post body |

### Padding
Minimum **48px on all sides** for both formats.

```
Cover / OG (1200 × 630):
  Safe content area: 1104 × 534px
  Origin of content: x: 48px, y: 48px

In-article (1200 × 880):
  Safe content area: 1104 × 784px
  Origin of content: x: 48px, y: 48px
```

Background fills and full-bleed colors extend to the canvas edge. Only text, logo, and graphic elements must stay within the safe zone.

---

## Cover Image Templates (1200 × 630)

All cover images share a fixed structural base:
- **Full-bleed violet-06 background** — always, no exceptions
- **Two-panel split** — left: light grey rounded card (~50% width), right: B&W photo with rounded corners (~50% width)
- Logo (dark variant) top-left of the left panel
- Title (Darker Grotesque, bold, black) in the left panel, left-aligned

### Three cover variants

| Variant | Left panel content |
|---------|-------------------|
| **Cover + title + shape** | Logo → title → decorative orb (bottom-left) |
| **Cover + title** | Logo (top-left) → title (bottom-left area) |
| **Cover + bullet-points** | Logo → title → sub-heading → 3 bullet items with dividers |

---

## In-Article Templates (1200 × 880)

### 1 — Steps

Use when showing a numbered sequence or process.

**Staircase** — Dark charcoal bg. Title on the left. Right side: ascending staircase bars (violet fill), each bar has a violet-filled circle number (white text) on the left end, and a label on the bar. Bars ascend from bottom-left to top-right.

**Two-column Steps with Description** — Light grey bg. Left panel: logo + title + orb. Right panel: numbered list where each item has a violet circle number, a bold step title, and a description line below. Items connected by thin violet horizontal lines.

**Two-column Steps without Description** — Same as above, step title only, no description.

---

### 2 — Horizontal Cards

Use when comparing or listing 2 items side by side.

Two large rounded cards side by side inside a shared card container. Header title above the container (center-aligned, white on dark/violet bg, or black on light bg).

| Variant | Card content |
|---------|-------------|
| **Horizontal cards** | Violet arrow icon (top-left) + image area + bold title + paragraph description |
| **Horizontal cards with pointers** | Violet arrow icon (top-left) + image area + bold title + bullet list |
| **Stacked** | Violet circle icon (top-left) + bold title + bullet list. Dark charcoal bg. |

---

### 3 — Stacked Cards with Description

Two cards side by side (same as Horizontal Cards), dark charcoal background. Each card: bold title (violet) + description paragraph. No icon.

---

### 4 — Card Grids

Use for listing multiple items (features, use cases, benefits).

**Grid structure:** Cards arranged in a grid. The **center card is always violet-06 filled** with the Facilio logo + icon + topic name — acts as the brand anchor. All other cards use light grey fill.

| Variant | Grid | Cell content |
|---------|------|-------------|
| **5 Card Grid with Numbers** | 1 large title card + 2 right + 3 bottom | Large % numeral (violet, IBM Plex Mono) + label |
| **5 Card Grid with Icons** | Same layout | Icon (violet) + label |
| **7 Card Grid with Numbers** | 3×3, center = violet brand card | Large % numeral (violet) + label |
| **7 Card Grid with Icons** | 3×3, center = violet brand card | Icon (violet) + label |

Dark charcoal bg for all card grid templates.

---

### 5 — 4 Grids

Use for 4 equal checkmark/benefit items.

2×2 grid of equal rounded cards. Each card: green checkmark icon (centered top) + text (centered).

| Variant | Background |
|---------|-----------|
| **4 grids** | Violet-06 full bleed, white title, cards have grey fill |
| **4 grids open** | Light grey bg, logo + title top-left, same cards |

---

### 6 — 2 Column List

Split layout. Left: grey rounded card with logo + title + orb. Right: stacked rows, each row is a rounded card with a violet-filled circle checkmark icon + label text. Typically 4 items. Dark charcoal outer bg.

---

### 7 — Tables

Use for structured comparison or feature matrix content.

**Comparison table (Before vs After):**
- Dark charcoal-06/07 bg. Title centered (white).
- 2-column table inside a rounded container. Left column = dark grey header "Before" + rows with red ✗ icons. Right column = violet-06 header "After" + rows with green ✓ icons. Rows separated by horizontal dividers.

**Features table:**
- Violet-06 bg. Title centered (white).
- 3-column table (e.g. Strategy | Approach A | Approach B). Header row = dark rounded cards. All rows = dark bg, white text. Leftmost column labels are bold.

---

### 8 — Timelines

Use for chronological or sequential history/process content.

| Variant | Layout |
|---------|--------|
| **Timeline 1** | Split. Left: grey card with logo + title + orb. Right: dark area with horizontal connecting line, violet dot nodes, each with bold label + description below. |
| **Timeline 2** | Violet bg. Title + sub-title centered top. Bottom: horizontal pill rail with era/date labels (violet rounded pills) hanging down, each with a dark rounded description card below. |
| **Timeline 3** | Dark bg. Logo + title top-left. Center: horizontal tick-mark bar with 5 nodes dropping down. Each node: bold label (violet) + description text. |

---

### 9 — Diagrams & Flows

Use for conceptual relationships, processes, and system explanations.

**Venn diagram** — Light bg. Title top-center (black). Two large overlapping circles (grey fill). Intersection = violet-06. Each circle: icon + bold title + list items. Intersection: white text label.

**Flow - Detailed** — Dark charcoal bg. Title + sub-title centered top. 4 icon-nodes arranged horizontally, connected by curved arch lines from above. Each node: violet-filled circle + icon (white) + label below. Bottom-center: grey rounded pill stat callout (e.g. "97% SLA adherence").

**Flow - Simple** — Same structure as Detailed, without sub-title and without the stat callout pill.

**Levels** — Split layout. Left: grey card with logo + title + orb. Right: 3 stacked arch/semi-circle shapes in violet shades (darkest shade at bottom, lightest at top). Each arch: bold white level name + description text centered.

**Cycle** — Violet-06 bg. Center: dark rounded pill with bold white title. 6 nodes arranged in an oval loop around the pill, connected by thin violet lines. Each node: violet diamond shape + label text.

**This to that** — Dark bg. Title centered top. 3 rows, each row: [grey rounded card — source label] → [violet-06 rounded square with white arrow →] → [grey rounded card — outcome text]. Arrow connector is always violet.

**Comparison** — Dark bg. Title centered top. Two side-by-side panels: left = grey bg + competitor/generic logo placeholder + feature list, right = violet-06 bg + Facilio logo + same feature list. Used for product/brand differentiation.

---

## Spacing Reference

| Context | Value |
|---------|-------|
| Canvas padding (min) | 48px |
| Between logo and title | `space-16` to `space-24` |
| Between title and content area | `space-24` to `space-32` |
| Between cards in a grid | `space-12` to `space-16` |
| Between list items | `space-12` |
| Between icon and label | `space-8` |
| Card corner radius | ~16–20px (large rounded) |

---

*FDS 2026 Blog Image — sourced from Figma file eFOBPdj9il7u3R5KP7GEns, node 33:8664.*
