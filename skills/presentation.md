# FDS 2026 — Presentation Skill File
> Use this file as LLM context when generating slide decks, pitch decks, and presentation visuals for Facilio.

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the presentation context.

---

## Colors

**Primary:** Violet — slide accents, key callout backgrounds, progress indicators, highlight bars.
**Accent:** Blue (info), Yellow (warning/attention), Green (positive/success), Orange (caution/alert) — use for data callouts, status indicators, chart elements.
**Neutral:** Charcoal and White are the primary slide surface colors. Black for all headings.

Slide backgrounds are typically `white` or `charcoal-01` for light decks, or `charcoal-11`/`violet-11`/`black` for dark/hero slides.

---

## Typography

| Element | Font | Weight | Color |
|---------|------|--------|-------|
| Slide title | Darker Grotesque | 700 | `black` on light / `white` on dark |
| Section divider title | Darker Grotesque | 800 | `black` or `white` |
| Sub-title / h3 | Darker Grotesque | 600 | `black` or `white` |
| Body copy | Inter | 400 | `charcoal-08` on light / `charcoal-02` on dark |
| Bullet point | Inter | 400 | `charcoal-08` on light / `charcoal-02` on dark |
| Caption / footnote | Inter | 400 | `charcoal-06` |
| Stat / KPI numeral | IBM Plex Mono | 600–700 | Accent `07` or `black` |
| Label / tag | IBM Plex Mono | 500 | Accent `07` shade |

**Key rule:** Presentation type sizes are larger than web — titles typically 36–60px equivalent, body 18–24px equivalent. Fewer words per slide is always better.

---

## Spacing

Presentations use generous spacing. Use `--fds-space-*` values as a reference baseline:

| Context | Suggested value |
|---------|----------------|
| Slide content margin | `space-48` to `space-80` |
| Spacing between elements | `space-24` to `space-48` |
| Between title and body | `space-32` |
| Between bullet items | `space-12` to `space-16` |

---

## Icons

Use **Google Material Symbols, Outlined style, weight 300**. See `SKILL.md` → Icons for the full spec, color rules, and size guidelines.

Presentation icon sizes: **32–40px** inline/supporting, **48–64px** standalone/feature icons, **28px** inside a 56px filled circle.

Export individual SVGs from [fonts.google.com/icons](https://fonts.google.com/icons) at weight 300, Outlined style.

---

## Logo

<!-- To be defined — slide master logo placement, sizing, dark vs. light variant per slide theme -->

---

## Slide Types

<!-- To be filled in — title slide, section divider, content slide, data/chart slide, quote slide, end slide specs -->

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

For slides with prominent hero visuals or full-bleed backgrounds, the background image may extend to the canvas edge — but all text and interactive content must remain within the 64px safe zone.

### Spacing reference at 1920×1080
| Context | Recommended value |
|---------|------------------|
| Slide margin (min) | 64px — `space-64` |
| Between title and body | `space-32` to `space-48` |
| Between body sections | `space-48` |
| Between bullet items | `space-12` to `space-16` |
| Between columns | `space-48` to `space-64` |

---

*FDS 2026 Presentation — based on Facilio Design System tokens.*
