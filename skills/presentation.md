# FDS 2026 — Presentation Skill File
> Use this file as LLM context when generating slide decks, pitch decks, and presentation visuals for Facilio.

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the presentation context.

**Governing design style: Swiss Style (International Typographic Style).**
All presentation designs must follow this discipline — mathematical grids, strict typographic hierarchy, generous white space, no decorative ornament. Adapted here for the 1920×1080 slide canvas.

---

## Design Philosophy — Swiss Style

Presentations at FDS 2026 follow the principles of the International Typographic Style. Slides are not decorated canvases — they are structured, objective communication frames. One idea per slide. Nothing extra.

### Core rules
- **One idea per slide.** If a slide needs a subtitle to explain the title, the content should be split into two slides.
- **Grid governs everything.** Every element — text, image, rule, stat — is placed on the grid. Nothing floats.
- **Typography is structure.** Hierarchy is built through size, weight, and placement — not color, shadow, or decoration.
- **White space is intentional.** A slide with generous empty space is not unfinished — it is disciplined. Never fill space for the sake of filling it.
- **No decoration.** No drop shadows, no gradients on text or backgrounds, no rounded-corner boxes, no decorative borders, no clip art, no illustration.
- **Left-aligned, ragged right.** All body text and bullet points are flush left. Never centered for body copy. Titles may be left-aligned or centered only on full-bleed hero slides.
- **Asymmetric layouts.** Prefer asymmetric column splits over centered symmetric layouts — narrow left column for labels/stats, wider right for body content.
- **One accent per slide.** Violet is primary. One additional accent color per slide maximum — only for data status or callouts.

---

## Grid System

### Column grid
All slides use a column grid anchored within the 64px safe zone.

| Layout type | Columns | Gutter | Use |
|-------------|---------|--------|-----|
| Single column | 1 | — | Title slides, section dividers, full-width quotes |
| Two column | 2 | 48px | Content + visual, stat pairs, side-by-side comparison |
| Three column | 3 | 40px | Feature grids, icon + label rows, data callouts |
| Four column | 4 | 32px | KPI rows, icon grids |

- All columns are calculated from the safe content area (1792px wide at 64px margin).
- Content never crosses into the gutter.
- Images and visual blocks must align to at least one column edge.

### Baseline grid
- Base unit: **8px**
- All vertical spacing between elements must be a multiple of 8px.
- Body text sits on a 32px baseline grid (20px font / 1.6 line-height → 32px).

### Horizontal rules
1px rules in `charcoal-03` or `violet-06` are structural elements — use them to:
- Separate the slide header area from body content
- Anchor the slide number and logo in the footer zone
- Divide two-column layouts with a vertical rule (1px, `charcoal-03`)

Do not use rules decoratively. Each rule must serve a structural purpose.

---

## Colors

**Palette discipline:** Black and white are the primary slide surfaces. Introduce violet as a single accent. Accent colors (blue, yellow, green, orange) only for data status and callouts.

| Slide type | Background | Text |
|------------|-----------|------|
| Standard content | `white` or `charcoal-01` | `black` headings, `charcoal-08` body |
| Dark / hero | `charcoal-11` or `violet-11` or `black` | `white` headings, `charcoal-02` body |
| Section divider | `violet-06` or `charcoal-11` | `white` |
| Full-bleed photo | Photo extends to edge | `white` text over dark photo overlay |

**Color rules:**
- Per slide, use at most **one accent color** beyond black, white, and charcoal.
- Violet is the primary brand accent — hero backgrounds, progress bars, key callouts, section markers.
- Accent colors (blue, yellow, green, orange) are for data callouts and status indicators only.
- **Never use:** gradients on backgrounds or text, drop shadows, semi-transparent color washes over more than one slide element.

---

## Typography

All body type is set flush left, ragged right. No centered body copy.

| Element | Font | Weight | Size | Color |
|---------|------|--------|------|-------|
| Slide title | Darker Grotesque | 700 | 48–60px | `black` on light / `white` on dark |
| Section divider title | Darker Grotesque | 800 | 56–72px | `white` |
| Sub-title / h3 | Darker Grotesque | 600 | 32–40px | `black` or `white` |
| Body copy | Inter | 400 | 20–24px | `charcoal-08` on light / `charcoal-02` on dark |
| Bullet point | Inter | 400 | 18–22px | `charcoal-08` on light / `charcoal-02` on dark |
| Caption / footnote | Inter | 400 | 14–16px | `charcoal-06` |
| Stat / KPI numeral | IBM Plex Mono | 600–700 | 48–80px | Accent `07` or `black` |
| Label / tag | IBM Plex Mono | 500 | 13–15px | Accent `07` shade |
| Slide number | IBM Plex Mono | 400 | 13px | `charcoal-05` |

### Typographic rules
- **Line height:** 1.4× for titles. 1.6× for body copy.
- **Max line length:** No text block should exceed 70 characters per line — use column width to enforce this.
- **Fewer words.** A slide title should be 3–7 words. A bullet point should be a phrase, not a sentence.
- **No italic** for emphasis — use weight (600) or a label/tag treatment.
- **No underline** except for hyperlinks shown in speaker notes.
- **Tracking:** 0 for body text. Slight positive tracking (0.03em–0.06em) for ALL CAPS labels only.
- **Bullet points:** Use a simple 1px `violet-06` or `charcoal-05` dash or rule marker — never software-default round bullets or arrow bullets.

---

## Spacing

Base unit is **8px**. All spacing values must be multiples of 8.

| Context | Value |
|---------|-------|
| Slide content margin (min) | 64px (`space-64`) |
| Slide content margin (comfortable) | 80px or 96px |
| Between title and body | 32–48px (`space-32` to `space-48`) |
| Between body sections | 48px (`space-48`) |
| Between bullet items | 12–16px (`space-12` to `space-16`) |
| Between columns | 48–64px (`space-48` to `space-64`) |
| Between icon and label | 12px (`space-12`) |
| Rule to content gap | 16px (`space-16`) |

---

## Icons

Use **Google Material Symbols, Outlined style, weight 300**. See `SKILL.md` → Icons for the full spec, color rules, and size guidelines.

Presentation icon sizes: **32–40px** inline/supporting, **48–64px** standalone/feature icons, **28px** inside a 56px filled circle.

Icons must be single-color only — never multi-color within a slide icon set.

Export individual SVGs from [fonts.google.com/icons](https://fonts.google.com/icons) at weight 300, Outlined style.

---

## Layout Principles

### Asymmetry within the grid
Swiss Style does not center everything. Prefer asymmetric column splits over symmetric two-column layouts.

```
Example 2-column split (1792px safe area, 48px gutter):
  Left column:  560px  (stat, label, section marker, icon)
  Gutter:        48px
  Right column: 1184px (title, body copy, list)
```

For feature grids and KPI rows, use equal columns — asymmetry applies to narrative layouts, not data arrays.

### Section markers
Use a solid `violet-06` left-border rule (4–6px wide, full text-block height) or an IBM Plex Mono 500 ALL CAPS label in `violet-06` to mark a section or category. Never use filled background boxes for section headings on a slide.

### Callout boxes
Callout boxes on slides use a **4–6px left-border rule** in the accent color — not a filled card with rounded corners and a shadow.

```
Structure:
  Left border: 5px solid accent-06
  Background: accent-02 (very light tint)
  Padding: 24px
  Text: body size, Inter 400, accent-08
  No border-radius. No shadow.
```

### Stat / KPI callouts
Large numerical KPIs use IBM Plex Mono 600–700 at 56–80px, with a compact IBM Plex Mono 500 label above in `charcoal-06`. Group multiple KPIs in a column-aligned row using equal-width grid columns.

### Photography
Photography can be used as:
- **Full-bleed background** on hero / section divider slides — photo extends to canvas edge, text stays within 64px safe zone
- **Half-slide image** — photo fills the right or left column, text occupies the opposite column
- Black-and-white or desaturated photography is preferred over full-color to maintain visual discipline

No illustration. No stock vector art. No icon-as-hero usage.

---

## Slide Types

### Title slide
- Background: `white` or `charcoal-11`
- Large document/deck title: Darker Grotesque 800, 56–72px, black or white
- Subtitle or date: Inter 400, 20px, `charcoal-06` or `charcoal-03`
- Logo: bottom-left or top-left, within the 64px safe zone
- A single `violet-06` horizontal rule or left-border accent element — nothing more

### Section divider slide
- Background: `violet-06`, `charcoal-11`, or `black`
- Section title: Darker Grotesque 800, 64–80px, `white`
- Optional section number: IBM Plex Mono 500, 14px, `charcoal-03`, top-left
- No body text. No bullet points. One idea only.

### Content slide
- Background: `white` or `charcoal-01`
- Slide title: Darker Grotesque 700, 48–56px, `black`, flush left, anchored to the top grid band
- Body text or bullet list: Inter 400, 20–22px, `charcoal-08`, in the main content column
- Optional left-column: stat, icon, or section label
- Slide number: IBM Plex Mono 400, 13px, `charcoal-05`, bottom-right of safe zone

### Data / chart slide
- Title: Darker Grotesque 700, 40–48px, `black`
- Chart or table: grid-aligned, no decorative chart styling — flat bars, simple lines, no 3D
- Data labels: IBM Plex Mono 500, 14px
- Legend: Inter 400, 13–14px, `charcoal-07`, aligned to column grid
- Axis labels: Inter 400, 12–13px, `charcoal-06`
- Chart colors follow accent palette — one color per data series; violet for primary series

### Quote slide
- Background: `charcoal-11` or `violet-11`
- Quote text: Darker Grotesque 600–700, 32–40px, `white`, flush left, ragged right
- Attribution: Inter 400, 16–18px, `charcoal-03`, below the quote with 32px gap
- A single `violet-06` or `white` 4px left-border rule to the left of the quote block
- No quotation mark glyphs as decorative elements

### End / closing slide
- Mirrors the title slide in structure
- CTA or contact: Inter 400, 20px
- Logo centered or bottom-center
- No bullet lists

---

## Logo

- Use the **classic Facilio logo** (horizontal wordmark) for all presentation slides
- **Content slides:** compact/wordmark variant, 20–24px height, bottom-left of safe zone
- **Title and end slides:** full variant, 28–32px height, bottom-left or centered
- **Section dividers (dark bg):** white variant
- Minimum clear space around the logo: equal to the cap-height of the wordmark
- Never place the logo on a patterned or gradient background

---

## Medium-Specific Rules

### Canvas Size
**1920 × 1080px** (16:9). This is the only supported presentation canvas size.

### Padding
Minimum **64px on all sides**. No content, text, or graphics may appear outside this boundary.

```
Slide: 1920 × 1080px
Safe content area: 1792 × 952px  (1920 − 128px, 1080 − 128px)
Origin of content: x: 64px, y: 64px
```

For slides with full-bleed backgrounds or photography, the background extends to the canvas edge — but all text and graphic content must remain within the 64px safe zone.

### What is never allowed in FDS presentations
- Drop shadows on any element (text, box, image, icon)
- Gradients (background, text, or shape fills)
- Rounded corners on callout boxes or containers
- Centered body text or bullet points
- Software-default bullet styles (round dots, arrows, chevrons)
- Decorative dividers (anything other than a plain 1px rule)
- Illustration or vector stock art
- More than one accent color family per slide
- Animations that serve style over communication (transitions, fly-ins, bounces)

---

*FDS 2026 Presentation — International Typographic Style · based on Facilio Design System tokens.*
