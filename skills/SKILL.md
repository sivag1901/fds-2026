# FDS 2026 — Facilio Design System Skills File
> Feed this file to any LLM to generate on-brand UI components, screens, and design tokens.

---

## What is FDS 2026?

FDS 2026 is Facilio's standalone design system. It defines a structured 7-family color palette, a 3-font typographic system, and logo usage rules. Colors are sourced from Figma (`fds-2026`, Section 1). Every color has 11 shades numbered `01` (lightest) → `11` (darkest). The mid-point base shade is typically `05` or `06`.

---

## Color System

### Color Roles

| Role | Families | Purpose |
|------|----------|---------|
| **Primary** | Violet | Brand identity, primary actions, focus rings, active states |
| **Accent** | Blue, Yellow, Green, Orange | Status indicators, highlights, supporting UI |
| **Neutral** | Charcoal, Grey, White, Black | Text hierarchy, surfaces, borders, backgrounds |

---

### Primary — Violet

| Token | Hex | Use |
|-------|-----|-----|
| violet-01 | `#f0ecfe` | Primary tint backgrounds, hover fill on ghost elements |
| violet-02 | `#ddd5fd` | Subtle primary fills |
| violet-03 | `#c0adfb` | Light primary accents |
| violet-04 | `#a386f9` | Focus rings, icon fills |
| violet-05 | `#8560f8` | Secondary primary elements |
| violet-06 | `#623cf6` | **Base — primary CTA, brand color** |
| violet-07 | `#4e2fcc` | Hover on primary |
| violet-08 | `#3b23a2` | Active / pressed primary |
| violet-09 | `#291878` | Dark primary text on light BG |
| violet-10 | `#180e4f` | Deep primary surfaces |
| violet-11 | `#0d0829` | Near-black, dark mode primary surfaces |

---

### Accent — Blue (Info)

| Token | Hex | Use |
|-------|-----|-----|
| blue-01 | `#eff6ff` | Info backgrounds |
| blue-02 | `#dbeafe` | Info tints |
| blue-03 | `#bedbff` | Light info fills |
| blue-04 | `#8ec5ff` | Info icons, borders |
| blue-05 | `#51a2ff` | Info accents |
| blue-06 | `#2b7fff` | **Base — links, info** |
| blue-07 | `#155dfc` | Hover on links |
| blue-08 | `#1447e6` | Active links |
| blue-09 | `#193cb8` | Dark info text |
| blue-10 | `#1c398e` | Deep blue surfaces |
| blue-11 | `#162456` | Near-black blue |

---

### Accent — Yellow (Warning)

| Token | Hex | Use |
|-------|-----|-----|
| yellow-01 | `#fefce8` | Warning backgrounds |
| yellow-02 | `#fef9c2` | Warning tints |
| yellow-03 | `#fff085` | Light warning fills |
| yellow-04 | `#ffdf20` | Warning highlights |
| yellow-05 | `#fdc700` | **Base — warning** |
| yellow-06 | `#f0b100` | Hover on warning |
| yellow-07 | `#d08700` | Active warning |
| yellow-08 | `#a65f00` | Dark warning text |
| yellow-09 | `#894b00` | Deep amber |
| yellow-10 | `#733e0a` | Dark amber |
| yellow-11 | `#432004` | Near-black amber |

---

### Accent — Green (Success)

| Token | Hex | Use |
|-------|-----|-----|
| green-01 | `#f0fdf4` | Success backgrounds |
| green-02 | `#dcfce7` | Success tints |
| green-03 | `#b9f8cf` | Light success fills |
| green-04 | `#7bf1a8` | Success highlights |
| green-05 | `#05df72` | Vivid success |
| green-06 | `#00c950` | **Base — success** |
| green-07 | `#00a63e` | Hover on success |
| green-08 | `#008236` | Active success |
| green-09 | `#016630` | Dark success text |
| green-10 | `#0d542b` | Deep green |
| green-11 | `#032e15` | Near-black green |

---

### Accent — Orange (Caution / Error)

| Token | Hex | Use |
|-------|-----|-----|
| orange-01 | `#fff7ed` | Caution backgrounds |
| orange-02 | `#ffedd4` | Caution tints |
| orange-03 | `#ffd6a7` | Light caution fills |
| orange-04 | `#ffb86a` | Caution highlights |
| orange-05 | `#ff8904` | **Base — caution** |
| orange-06 | `#ff6900` | Hover on caution / error |
| orange-07 | `#f54900` | Active caution |
| orange-08 | `#ca3500` | Dark caution text |
| orange-09 | `#9f2d00` | Deep orange |
| orange-10 | `#7e2a0c` | Dark orange |
| orange-11 | `#441306` | Near-black orange |

---

### Neutral — Charcoal (Text & Structure)

| Token | Hex | Use |
|-------|-----|-----|
| charcoal-01 | `#f8fafc` | Page backgrounds |
| charcoal-02 | `#f1f5f9` | Card / panel backgrounds |
| charcoal-03 | `#e2e8f0` | Dividers, borders |
| charcoal-04 | `#cad5e2` | Input borders |
| charcoal-05 | `#90a1b9` | Placeholder text |
| charcoal-06 | `#62748e` | **Base — muted text** |
| charcoal-07 | `#45556c` | Secondary text |
| charcoal-08 | `#314158` | Body text |
| charcoal-09 | `#1d293d` | Strong body text |
| charcoal-10 | `#0f172b` | Headings |
| charcoal-11 | `#020618` | Near-black, dark mode surfaces |

---

### Neutral — White & Black

| Token | Hex | Use |
|-------|-----|-----|
| white | `#ffffff` | Pure white surfaces, reversed text on dark backgrounds |
| black | `#000000` | **All titles and headings (h1–h4)** |

---

### Neutral — Grey (Structural Only)

> Never use grey for interactive elements. Grey is for structural/neutral surfaces only.

| Token | Hex | Use |
|-------|-----|-----|
| grey-01 | `#fafafa` | Page backgrounds |
| grey-02 | `#f5f5f5` | Subtle surfaces |
| grey-03 | `#e5e5e5` | Borders, dividers |
| grey-04 | `#d4d4d4` | Input borders |
| grey-05 | `#a1a1a1` | Placeholder text |
| grey-06 | `#737373` | **Base — muted** |
| grey-07 | `#525252` | Secondary text |
| grey-08 | `#404040` | Body text |
| grey-09 | `#262626` | Strong text |
| grey-10 | `#171717` | Headings |
| grey-11 | `#0a0a0a` | Near-black |

---

## Semantic Color Roles

```
── Primary ──────────────────────────────────────────
Primary action:       violet-06  (#623cf6)
Primary hover:        violet-07  (#4e2fcc)
Primary active:       violet-08  (#3b23a2)
Primary subtle bg:    violet-01  (#f0ecfe)
Focus ring:           violet-04  (#a386f9)

── Accent / Status ──────────────────────────────────
Info:                 blue-06    (#2b7fff)
Info background:      blue-01    (#eff6ff)
Info text:            blue-09    (#193cb8)

Success:              green-06   (#00c950)
Success background:   green-01   (#f0fdf4)
Success text:         green-09   (#016630)

Warning:              yellow-05  (#fdc700)
Warning background:   yellow-01  (#fefce8)
Warning text:         yellow-09  (#894b00)

Caution / Error:      orange-06  (#ff6900)
Caution background:   orange-01  (#fff7ed)
Caution text:         orange-09  (#9f2d00)

── Neutral ──────────────────────────────────────────
Title / Heading text: black      (#000000)   ← h1–h4 always
Body text:            charcoal-08 (#314158)
Muted text:           charcoal-06 (#62748e)
Strong text:          charcoal-09 (#1d293d)
Page background:      charcoal-01 (#f8fafc)
Card background:      charcoal-02 (#f1f5f9)
Border:               charcoal-03 (#e2e8f0)
Input border:         charcoal-04 (#cad5e2)
Placeholder:          charcoal-05 (#90a1b9)
White surface:        white       (#ffffff)

Neutral surface:      grey-01    (#fafafa)
Neutral border:       grey-03    (#e5e5e5)

── Tags (accent at shade 07) ────────────────────────
Info tag text:        blue-07    (#155dfc)
Warning tag text:     yellow-07  (#d08700)
Success tag text:     green-07   (#00a63e)
Caution tag text:     orange-07  (#f54900)
```

---

## Typography

### Font Roles

| Role | Font | Usage |
|------|------|-------|
| **Title** | Darker Grotesque | h1, h2, h3, h4 |
| **Body** | Inter | h5, h6, body copy, labels, inputs |
| **Mono** | IBM Plex Mono | Tags, numericals, code |

### Color Rules

| Element | Font | Color |
|---------|------|-------|
| h1, h2, h3, h4 | Darker Grotesque | `black` (#000000) — always |
| h5, h6 | Inter | `black` (#000000) — always |
| Body copy | Inter | `charcoal-08` (#314158) |
| Muted / secondary text | Inter | `charcoal-06` (#62748e) |
| Tag text | IBM Plex Mono | Accent `07` shade matching tag intent |

Tags use the `07` shade of the relevant accent color for their text:
- Info tag → `blue-07` (#155dfc)
- Warning tag → `yellow-07` (#d08700)
- Success tag → `green-07` (#00a63e)
- Caution / error tag → `orange-07` (#f54900)

### Font Rules
1. Darker Grotesque is a display/title font — use only for h1–h4. Variable weight 300–900; prefer Bold (700) for h1–h2, SemiBold (600) for h3–h4.
2. Inter handles h5, h6, and all body copy. Variable font — weight 400 for body, 500–600 for emphasis, 700 for strong labels.
3. IBM Plex Mono is reserved strictly for tags, badges, numerical values, and code. Do not use it for prose.
4. Never mix Darker Grotesque into body copy or IBM Plex Mono into headings.

### CSS Usage
```css
@import 'tokens/colors.css';
@import 'tokens/typography.css';

h1, h2, h3, h4, h5, h6 {
  color: var(--fds-black);
}

h1 { font-family: var(--fds-font-title); font-weight: 700; }
h2 { font-family: var(--fds-font-title); font-weight: 700; }
h3 { font-family: var(--fds-font-title); font-weight: 600; }
h4 { font-family: var(--fds-font-title); font-weight: 600; }
h5 { font-family: var(--fds-font-body);  font-weight: 600; }
h6 { font-family: var(--fds-font-body);  font-weight: 600; }

body, p { font-family: var(--fds-font-body); color: var(--fds-charcoal-08); }

.fds-tag     { font-family: var(--fds-font-mono); }
.fds-numeral { font-family: var(--fds-font-mono); }

.fds-tag--info    { color: var(--fds-blue-07); }
.fds-tag--warning { color: var(--fds-yellow-07); }
.fds-tag--success { color: var(--fds-green-07); }
.fds-tag--caution { color: var(--fds-orange-07); }
```

---

## Spacing

### Scale Rules

- **4px multiples** for values up to 24px
- **8px multiples** for values from 32px to 200px
- **Maximum spacing: 200px** — never exceed this

### Full Scale

| Token | Value | Step |
|-------|-------|------|
| `--fds-space-4` | 4px | 4px |
| `--fds-space-8` | 8px | 4px |
| `--fds-space-12` | 12px | 4px |
| `--fds-space-16` | 16px | 4px |
| `--fds-space-20` | 20px | 4px |
| `--fds-space-24` | 24px | 4px — last fine step |
| `--fds-space-32` | 32px | 8px — first coarse step |
| `--fds-space-40` | 40px | 8px |
| `--fds-space-48` | 48px | 8px |
| `--fds-space-56` | 56px | 8px |
| `--fds-space-64` | 64px | 8px |
| `--fds-space-72` | 72px | 8px |
| `--fds-space-80` | 80px | 8px |
| `--fds-space-88` | 88px | 8px |
| `--fds-space-96` | 96px | 8px |
| `--fds-space-104` | 104px | 8px |
| `--fds-space-112` | 112px | 8px |
| `--fds-space-120` | 120px | 8px |
| `--fds-space-128` | 128px | 8px |
| `--fds-space-136` | 136px | 8px |
| `--fds-space-144` | 144px | 8px |
| `--fds-space-152` | 152px | 8px |
| `--fds-space-160` | 160px | 8px |
| `--fds-space-168` | 168px | 8px |
| `--fds-space-176` | 176px | 8px |
| `--fds-space-184` | 184px | 8px |
| `--fds-space-192` | 192px | 8px |
| `--fds-space-200` | 200px | 8px — maximum |

### Rules
1. Only use values from this scale. Never use arbitrary pixel values for spacing.
2. For component-internal spacing (padding, gap between elements) prefer values ≤ 24px.
3. For layout-level spacing (section padding, page margins, column gaps) use 32px and above.
4. Never exceed 200px for any single spacing value.

### CSS Usage
```css
@import 'tokens/spacing.css';

.card {
  padding: var(--fds-space-16);
  gap:     var(--fds-space-8);
}

.section {
  padding-top:    var(--fds-space-64);
  padding-bottom: var(--fds-space-64);
}
```

---

## Logo Usage

### Web — Always Use Classic Variant

| Background | File |
|------------|------|
| Light background | `logos/classic/facilio-dark.svg` |
| Dark background  | `logos/classic/facilio-white.svg` |

### Rules
1. On web, always use the **classic** variant (`logos/classic/`). Never use the modern variant on web.
2. Choose dark vs. white based on the background:
   - Light surfaces (charcoal-01 through charcoal-04, grey-01 through grey-04) → `facilio-dark.svg`
   - Dark surfaces (charcoal-08 through charcoal-11, any color at shade 08–11) → `facilio-white.svg`
   - When the background is the primary brand color (violet-06 and darker) → `facilio-white.svg`
3. Never place the logo on a busy or patterned background without a clear safe zone.

---

## LLM Prompt Instructions

When generating UI components using FDS 2026:

1. **Color roles first**: Violet = primary action only. Accent colors (blue/yellow/green/orange) = status only. Charcoal/Grey = all structure, text, and surfaces.
2. **Always use token names** (e.g. `violet-06`) in reasoning, then resolve to hex or CSS var for code output.
3. **Light mode defaults**: page background `charcoal-01`; body text `charcoal-08`; all headings `black` (#000000).
4. **Dark mode**: backgrounds `charcoal-10`/`charcoal-11`; body text `charcoal-02`; headings `white` (#ffffff).
5. **Font assignment**: h1–h4 → Darker Grotesque, color always `black`. h5/h6/body → Inter, headings `black`, body `charcoal-08`. Tags/numbers → IBM Plex Mono, color from accent `07` shade.
6. **Logo on web**: always classic variant; dark svg on light BG, white svg on dark BG.
7. **Grey is structural only** — never use grey for buttons, links, or interactive states. Use charcoal for text hierarchy.
8. **Accessibility**: Light text on `violet-06` passes AA. Dark text (`charcoal-09`+) on tint backgrounds (`01`–`03`) passes AA.
9. **11-step scale rule**: `01`–`03` = tint backgrounds. `04`–`05` = light accents. `06` = base. `07`–`08` = hover/active. `09`–`11` = dark text / deep surfaces.
10. **Spacing**: use only scale tokens. ≤ 24px for component internals, ≥ 32px for layout. Max is 200px. Never use arbitrary values.

---

## Example: Button Component Spec

```
Primary Button:
  background:       violet-06 (#623cf6)
  text:             white
  font:             Inter, 500
  hover background: violet-07 (#4e2fcc)
  active:           violet-08 (#3b23a2)
  focus ring:       violet-04 (#a386f9) at 3px offset
  disabled:         charcoal-04 bg, charcoal-06 text

Secondary Button:
  background:       transparent
  border:           violet-06 (#623cf6)
  text:             violet-06 (#623cf6)
  font:             Inter, 500
  hover background: violet-01 (#f0ecfe)

Danger Button:
  background:       orange-06 (#ff6900)
  text:             white
  font:             Inter, 500
  hover:            orange-07 (#f54900)
```

---

## File References

| File | Description |
|------|-------------|
| `tokens/colors.json` | W3C Design Token Community Group format |
| `tokens/colors.css` | CSS custom properties (`--fds-*` variables) |
| `tokens/colors.js` | Plain JavaScript module |
| `tokens/typography.css` | `@font-face` declarations + `--fds-font-*` tokens |
| `tokens/spacing.json` | W3C Design Token format — spacing scale |
| `tokens/spacing.css` | CSS custom properties (`--fds-space-*` variables) |
| `tokens/spacing.js` | Plain JavaScript module |
| `logos/classic/facilio-dark.svg` | Web logo — light backgrounds |
| `logos/classic/facilio-white.svg` | Web logo — dark backgrounds |
| `skills/SKILL.md` | This file — base rules, all mediums |
| `skills/web.md` | Web UI components and pages |
| `skills/poster.md` | Poster and large-format graphics |
| `skills/pdf.md` | PDF documents and reports |
| `skills/presentation.md` | Slide decks and presentations |

---

## Medium-Specific Skill Files

For targeted generation, use the medium-specific file instead of this base file:

| Medium | File | Use when |
|--------|------|----------|
| Web UI | `skills/web.md` | Building components, pages, prototypes |
| Poster | `skills/poster.md` | Event graphics, large-format visuals |
| PDF | `skills/pdf.md` | Reports, brochures, data sheets |
| Presentation | `skills/presentation.md` | Slide decks, pitch decks |

Each medium file imports all rules from this base file and adds medium-specific overrides.

---

*FDS 2026 — Facilio Design System. Sourced from Figma file `eFOBPdj9il7u3R5KP7GEns`, Section 1. 77 color tokens across 7 families.*
