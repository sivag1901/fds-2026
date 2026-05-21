# FDS 2026 — PDF Skill File
> Use this file as LLM context when generating PDF documents, reports, brochures, and data sheets for Facilio.

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the document/PDF context.

**Governing design style: Swiss Style (International Typographic Style).**
All PDF designs must follow this discipline — mathematical grids, strict typographic hierarchy, generous white space, no decorative ornament.

---

## Design Philosophy — Swiss Style

PDF designs at FDS 2026 follow the principles of the International Typographic Style (Swiss Style), developed in Zürich and Basel in the 1950s. The goal is objective, clear, and universal communication — not stylistic expression.

### Core rules
- **Grid governs everything.** Every element — text, image, rule, whitespace — is placed on the grid. Nothing floats freely.
- **Typography is structure.** Hierarchy is created through size, weight, and placement — never through decoration, color, or flourish.
- **White space is intentional.** Negative space is not emptiness — it is breathing room, rhythm, and structure. Never fill space for the sake of filling it.
- **No decoration.** No drop shadows, no gradients, no rounded-corner boxes, no decorative borders, no illustration, no background patterns.
- **Left-aligned, ragged right.** All body text is flush left. Never justified. Never centered for body copy.
- **Objective visual language.** Photography over illustration. Data over metaphor. Clarity over emotion.
- **One accent, used with discipline.** Per document section, use one accent color maximum — violet is primary. Accent colors (blue, yellow, green, orange) are reserved for status and data callouts only.

---

## Grid System

### Column grid
All pages use a **modular column grid**. Content is never placed freely — it must snap to a column or defined margin unit.

| Page type | Columns | Gutter |
|-----------|---------|--------|
| Single-column (body text) | 1 column | — |
| Two-column (report / data sheet) | 2 columns | 24px |
| Three-column (reference / table-heavy) | 3 columns | 16px |

- Columns are calculated from the safe content area (515px wide at 40px margin, 443px at 56px margin).
- Gutters are fixed. Content never crosses into the gutter.
- Images, callout boxes, and tables must align to at least one column edge.

### Baseline grid
- Base unit: **8px**
- All vertical spacing (line heights, gaps, section breaks, rule positions) must be a multiple of 8px.
- Body text sits on a 24px baseline grid (16px font / 1.5 line-height).

### Horizontal rules
Thin horizontal rules (1px, `charcoal-03` or `charcoal-04`) are a primary structural element — use them to:
- Separate the header from body content
- Mark major section breaks
- Anchor the footer
- Frame table headers

Do not use rules decoratively. Each rule must serve a structural purpose.

---

## Colors

**Palette discipline:** Use black and white as the primary document surface. Introduce violet sparingly as a single accent. Accent colors (blue, yellow, green, orange) only for data status and callouts — never as decoration.

| Role | Value | Usage |
|------|-------|-------|
| Page background | `white` (#ffffff) | All standard pages |
| Body text | `charcoal-08` (#314158) | All running text |
| Headings | `black` (#000000) | All headings h1–h4 |
| Caption / footnote | `charcoal-06` (#62748e) | Captions, footnotes, page numbers |
| Horizontal rules | `charcoal-03` (#c0cbd8) | Structural dividers |
| Primary accent | `violet-06` | Section markers, callout left-border, table header bg |
| Info callout | `blue-02` bg + `blue-08` text | Info/note boxes |
| Warning callout | `yellow-02` bg + `yellow-08` text | Warning/caution boxes |
| Success callout | `green-02` bg + `green-08` text | Positive/tip boxes |
| Alert callout | `orange-02` bg + `orange-08` text | Alert/critical boxes |

**Never use:** gradients, drop shadows, semi-transparent overlays, or more than one accent family per page.

Avoid deep dark backgrounds — prefer white page backgrounds for readability and print efficiency.

---

## Typography

All type is set flush left, ragged right. No centred body copy. No justified text.

| Element | Font | Weight | Size (px) | Color |
|---------|------|--------|-----------|-------|
| Document title (cover) | Darker Grotesque | 800 | 36–48 | `black` |
| Chapter heading (h1) | Darker Grotesque | 700 | 28–32 | `black` |
| Section heading (h2) | Darker Grotesque | 600–700 | 22–26 | `black` |
| Sub-heading (h3) | Darker Grotesque | 600 | 18–20 | `black` |
| Minor heading (h4) | Inter | 600 | 14–16 | `black` |
| Body copy | Inter | 400 | 14–16 | `charcoal-08` |
| Lead / intro paragraph | Inter | 400 | 16–18 | `charcoal-08` |
| Caption / footnote | Inter | 400 | 11–12 | `charcoal-06` |
| Table header | Inter | 600 | 12–13 | `black` or `white` (on `violet-06` bg) |
| Table cell | Inter | 400 | 12–14 | `charcoal-08` |
| Stat / numeral | IBM Plex Mono | 600 | 24–40 | `black` or accent `07` |
| Label / tag / badge | IBM Plex Mono | 500 | 11–12 | Accent `07` shade |
| Code snippet | IBM Plex Mono | 400 | 12–13 | `charcoal-09` |

### Typographic rules
- **Line height:** 1.5× for body copy (16px font → 24px line height). 1.2× for headings.
- **Paragraph spacing:** One blank baseline unit (8px) between paragraphs — do not indent.
- **Tracking:** 0 for body text. Slight positive tracking (0.02em–0.05em) for ALL CAPS labels and table headers only.
- **Never use italic** for emphasis — use weight (600) or a label treatment instead.
- **Never use underline** except for hyperlinks.
- **Widow/orphan control:** No single word on a final line. No heading at the bottom of a column without at least two lines of body following it.

---

## Spacing

Base unit is **8px**. All spacing values must be multiples of 8.

| Context | Value |
|---------|-------|
| Page margin (minimum) | 40px (`space-40`) |
| Page margin (comfortable) | 56px or 64px (`space-56` / `space-64`) |
| Between heading and body | 16px (`space-16`) |
| Between paragraphs | 12–16px (`space-12` to `space-16`) |
| Between major sections | 32–48px (`space-32` to `space-48`) |
| Table cell padding | 8–12px (`space-8` / `space-12`) |
| Callout box padding | 16px (`space-16`) |
| Rule to content gap | 8px |
| Between columns (gutter) | 16–24px |

---

## Icons

Use **Google Material Symbols, Outlined style, weight 300**. See `SKILL.md` → Icons for the full spec, color rules, and size guidelines.

PDF icon sizes: **16–20px** inline, **24–32px** standalone/feature icons, **16px** inside a 32px filled circle.

Icons must be single-color only (`charcoal-07` on light backgrounds, accent `07` for status icons). No multi-color icons.

Export individual SVGs from [fonts.google.com/icons](https://fonts.google.com/icons) at weight 300, Outlined style.

---

## Layout Principles

### Asymmetry within the grid
Swiss Style does not center everything. Prefer asymmetric column splits — a narrow left column for labels/numbers and a wider right column for body content is a classic and effective pattern.

```
Example 2-column split (515px safe area, 24px gutter):
  Left column:  155px  (labels, stats, section markers)
  Gutter:        24px
  Right column: 336px  (body text, descriptions)
```

### Section markers
Use a solid `violet-06` left-border rule (3–4px wide, full column height) or a violet section label in IBM Plex Mono 500 ALL CAPS to mark major sections. Never use filled background boxes for section headings.

### Callout boxes
Callout boxes use a **4px left-border rule** in the appropriate accent color — not a filled background box with rounded corners.

```
Structure:
  Left border: 4px solid accent-06
  Background: accent-02 (very light tint)
  Padding: 16px
  Text: body size, Inter 400, accent-08
  No border-radius. No shadow.
```

### Tables
Tables follow a minimal-line Swiss approach:
- **Header row:** `violet-06` background, `white` Inter 600 text, 1px white bottom rule
- **Body rows:** alternating `white` and `charcoal-01` — no color if data is sparse
- **Cell borders:** horizontal hairline rules (`charcoal-02`) only — no vertical column dividers
- **Last row:** 1px `charcoal-04` bottom rule to close the table
- No rounded corners. No drop shadow on tables.

### Data / stat callouts
Large numerical stats use IBM Plex Mono 600 at 32–40px, with a compact IBM Plex Mono 500 label above in `charcoal-06`. Group stats in a column-aligned row — never scatter them across the page.

---

## Document Structure

### Cover page
- White background with a single `violet-06` accent element (left-border rule or top color bar, max 8px thick)
- Document title: Darker Grotesque 800, 40–48px, black, top-left aligned within the grid
- Subtitle / description: Inter 400, 16–18px, `charcoal-08`
- Date, version, or client: IBM Plex Mono 500, 12px, `charcoal-06`, bottom-left
- Logo: top-right or bottom-right within the margin
- No full-bleed hero images. No gradient washes.

### Page header
- Thin 1px `charcoal-03` rule across the full content width, 8px below the header content
- Left: document title or chapter name — Inter 600, 11px, `charcoal-06`
- Right: Facilio logo (compact/wordmark variant), scaled to 16px height
- Header sits at the top of the safe zone (y: 40–56px from top edge)

### Page footer
- Thin 1px `charcoal-03` rule across the full content width, 8px above the footer content
- Left: section name or document subtitle — Inter 400, 11px, `charcoal-06`
- Right: page number — IBM Plex Mono 500, 11px, `charcoal-06`
- Footer sits at the bottom of the safe zone (y: 8px above the 40px margin)

### Table of contents
- Two-column grid: left column for chapter/section titles, right column for page numbers
- Leader dots (…) between title and number in `charcoal-03`
- Section headings in Darker Grotesque 600; sub-entries in Inter 400
- Separated by 1px `charcoal-02` rules between major sections

---

## Logo

- Use the **classic Facilio logo** (horizontal wordmark) for all PDF documents
- **Header:** compact/wordmark variant, 16px height, top-right
- **Cover page:** full variant, 24–28px height, positioned within the grid (top-right or bottom-right)
- Minimum clear space around the logo: equal to the height of the 'F' in the wordmark
- On white backgrounds: use the standard dark logo
- Never place the logo on a colored or patterned background within a PDF

---

## Medium-Specific Rules

### Canvas Size
**A4 — 595 × 842px** (portrait). This is the only supported PDF canvas size.

### Padding
Minimum **40px on all sides**. Content must never breach this boundary.

```
Page: 595 × 842px
Safe content area: 515 × 762px  (595 − 80px, 842 − 80px)
Origin of content: x: 40px, y: 40px
```

Wider margins (**56px or 64px**) are preferred for text-heavy documents — use 40px only when space is tight.

### What is never allowed in FDS PDFs
- Drop shadows on any element
- Gradients (background, text, or overlays)
- Rounded corners on callout boxes, tables, or containers
- Centered body text
- Justified text
- Italic type for emphasis
- Decorative dividers (anything other than a plain 1px rule)
- Background images on content pages
- More than one accent color family per spread

---

*FDS 2026 PDF — International Typographic Style · based on Facilio Design System tokens.*
