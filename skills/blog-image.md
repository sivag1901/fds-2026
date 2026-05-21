# FDS 2026 — Blog Image Skill File
> Use this file as LLM context when generating blog cover images, OG images, and in-article visuals for Facilio.

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the blog image context.

---

## Colors

**Primary:** Violet — dominant backgrounds, headline accents, brand presence.
**Accent:** Blue, Yellow, Green, Orange — category labels, highlight bars, icon backgrounds.
**Neutral:** Charcoal, Grey, White `#ffffff`, Black `#000000`.

Blog image backgrounds fall into three categories:
- **Dark** — `black`, `charcoal-10`, `charcoal-11`, or deep violet (`violet-09`, `violet-10`) for high-impact featured images.
- **Light** — `white` or `charcoal-01` for clean, editorial-style images.
- **Brand** — `violet-06` as a full-bleed background for product-focused or announcement posts.

---

## Typography

| Element | Font | Weight | Notes |
|---------|------|--------|-------|
| Article title / headline | Darker Grotesque | 800 | Color `white` on dark bg / `black` on light bg |
| Sub-title / descriptor | Darker Grotesque | 600 | Supporting line below headline |
| Category / tag label | IBM Plex Mono | 500 | Accent `07` shade, all-caps, small size |
| Author / date | Inter | 400 | `charcoal-02` on dark / `charcoal-06` on light |
| Stat / pull quote numeral | IBM Plex Mono | 700 | Large display numerals |

**Heading color rule:** White on dark or violet backgrounds. Black on white or light backgrounds. Never grey for main headline text.

---

## Spacing

Use `--fds-space-*` tokens as reference. Scale proportionally for the canvas size in use.

---

## Logo

Use the **classic** logo variant.
- Dark or violet backgrounds → `logos/classic/facilio-white.svg`
- Light backgrounds → `logos/classic/facilio-dark.svg`

Logo placement: bottom-left or top-left corner, within the safe zone. Never center the logo unless the image is purely brand/announcement with no text headline.

---

## Layout & Composition

Blog images follow a clear visual hierarchy:

1. **Background** — solid color, gradient, or photographic image with overlay.
2. **Category tag** — small mono label at the top-left, inside safe zone.
3. **Headline** — the dominant typographic element, left-aligned or center-aligned depending on format.
4. **Sub-title** — one line below headline, lighter weight.
5. **Logo** — bottom-left corner, always within safe zone.
6. **Author / meta** — optional, bottom-right, small size.

**Alignment:** Prefer left-aligned text for editorial and long-form content. Center-aligned is acceptable for short, punchy announcement images.

**Overlays:** When using a photographic background, always apply a dark semi-transparent overlay (`rgba(0,0,0,0.50)` to `rgba(0,0,0,0.70)`) to ensure text legibility.

---

## Medium-Specific Rules

### Canvas Sizes
Two supported blog image formats:

| Format | Dimensions | Aspect ratio | Use |
|--------|-----------|--------------|-----|
| **Cover / OG** | 1200 × 630px | ~1.91:1 | Blog cover image, Open Graph (Facebook, LinkedIn, social sharing) |
| **In-article** | 1200 × 880px | ~1.36:1 | Images used inside the blog post body |

### Padding
Minimum **48px on all sides** for both formats. No text or logo may appear outside this boundary.

```
Cover / OG (1200 × 630):
  Safe content area: 1104 × 534px
  Origin of content: x: 48px, y: 48px

In-article (1200 × 880):
  Safe content area: 1104 × 784px
  Origin of content: x: 48px, y: 48px
```

Background fills, gradients, photo images, and overlays may extend to the canvas edge — only text, logo, and graphic elements must stay within the 48px safe zone.

### Spacing reference at blog image scale
| Context | Recommended value |
|---------|------------------|
| Canvas padding (min) | 48px — `space-48` |
| Between category tag and headline | `space-16` to `space-24` |
| Between headline and sub-title | `space-12` to `space-16` |
| Between sub-title and author / meta | `space-24` to `space-32` |
| Between icon and label | `space-8` |

### Category tag style
- Font: IBM Plex Mono, 11–12px, weight 500, all-caps
- Color: accent `07` shade matching the topic (e.g. `violet-07` for product, `blue-07` for insights, `green-07` for sustainability)
- Background: matching accent `01` shade with subtle border, or plain text with a colored underline/dot prefix
- Example: `● ENERGY MANAGEMENT` in `violet-07` on `violet-01` pill

---

*FDS 2026 Blog Image — based on Facilio Design System tokens.*
