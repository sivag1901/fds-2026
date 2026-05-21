# FDS 2026 — Poster Skill File
> Use this file as LLM context when generating poster designs, event graphics, and large-format visuals for Facilio.

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the print/large-format context.

---

## Colors

**Primary:** Violet — dominant brand presence, hero backgrounds, key callouts.
**Accent:** Blue, Yellow, Green, Orange — highlights, icons, supporting callouts.
**Neutral:** Charcoal, Grey, White `#ffffff`, Black `#000000`.

Poster backgrounds can use deep violet shades (`violet-10`, `violet-11`) or near-black (`charcoal-11`, `black`) for dramatic impact, or white/light neutral for clean informational layouts.

---

## Typography

| Element | Font | Weight | Notes |
|---------|------|--------|-------|
| Hero headline | Darker Grotesque | 800–900 | Large display, color `black` on light / `white` on dark |
| Section heading | Darker Grotesque | 700 | |
| Sub-heading | Darker Grotesque | 600 | |
| Body / descriptor | Inter | 400–500 | Color `charcoal-08` on light / `charcoal-02` on dark |
| Stat / numeral | IBM Plex Mono | 600–700 | For large numerical values |
| Label / tag | IBM Plex Mono | 500 | Accent `07` shade |

**Heading color rule:** Black on light backgrounds, White on dark backgrounds — consistent with FDS base rules.

---

## Spacing

Use `--fds-space-*` tokens as reference units. For print/large-format, scale these values proportionally based on output resolution and physical size.

---

## Icons

Use **Google Material Symbols, Outlined style, weight 300**. See `SKILL.md` → Icons for the full spec, color rules, and size guidelines.

Poster icon sizes: **40–56px** inline/supporting, **64–96px** standalone/feature icons, **40px** inside an 80px filled circle.

Export individual SVGs from [fonts.google.com/icons](https://fonts.google.com/icons) at weight 300, Outlined style.

---

## Logo

<!-- To be defined — which variant, sizing rules, placement, clear space for poster contexts -->

---

## Layout & Composition

<!-- To be filled in — grid, hierarchy, bleed, safe zone, and composition guidelines for posters -->

---

## Medium-Specific Rules

### Canvas Sizes
Two supported poster formats:

| Format | Dimensions | Aspect ratio | Use |
|--------|-----------|--------------|-----|
| **Square** | 1200 × 1200px | 1:1 | Social, digital display |
| **Landscape** | 1350 × 1080px | 5:4 | Wide display, event screens |

### Padding
Minimum **80px on all sides** for both formats. No content may appear outside this boundary.

```
Square (1200 × 1200):
  Safe content area: 1040 × 1040px
  Origin of content: x: 80px, y: 80px

Landscape (1350 × 1080):
  Safe content area: 1190 × 920px
  Origin of content: x: 80px, y: 80px
```

Background fills, gradients, and full-bleed images may extend to the canvas edge — only text and graphic elements must stay within the 80px safe zone.

### Spacing reference at poster scale
| Context | Recommended value |
|---------|------------------|
| Canvas padding (min) | 80px — between `space-72` and `space-88` |
| Between headline and body | `space-24` to `space-40` |
| Between sections / blocks | `space-48` to `space-64` |
| Between icon and label | `space-8` to `space-12` |

---

*FDS 2026 Poster — based on Facilio Design System tokens.*
