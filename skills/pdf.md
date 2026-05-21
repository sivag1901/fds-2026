# FDS 2026 — PDF Skill File
> Use this file as LLM context when generating PDF documents, reports, brochures, and data sheets for Facilio.

---

## Foundation

This file extends the base FDS 2026 system. All color, typography, and logo rules from `SKILL.md` apply unless explicitly overridden here for the document/PDF context.

---

## Colors

**Primary:** Violet — section headers, callout boxes, key highlights, table header backgrounds.
**Accent:** Blue (info callouts), Yellow (warnings/notes), Green (success/positive indicators), Orange (caution/alerts).
**Neutral:** Charcoal for all body text and structure. White for page background. Black for titles.

Avoid deep dark backgrounds in multi-page documents — prefer white or `charcoal-01` page backgrounds for readability and ink efficiency.

---

## Typography

| Element | Font | Weight | Color |
|---------|------|--------|-------|
| Document title | Darker Grotesque | 700 | `black` (#000000) |
| Chapter / section heading | Darker Grotesque | 600–700 | `black` (#000000) |
| Sub-heading | Darker Grotesque | 600 | `black` (#000000) |
| h5, h6 / minor heading | Inter | 600 | `black` (#000000) |
| Body copy | Inter | 400 | `charcoal-08` (#314158) |
| Caption | Inter | 400 | `charcoal-06` (#62748e) |
| Table header | Inter | 600 | `black` or `white` (on dark header bg) |
| Table cell | Inter | 400 | `charcoal-08` |
| Stat / numeral | IBM Plex Mono | 500–600 | `charcoal-08` or accent `07` |
| Label / tag / badge | IBM Plex Mono | 500 | Accent `07` shade |
| Code snippet | IBM Plex Mono | 400 | `charcoal-09` |

---

## Spacing

Use `--fds-space-*` token values as reference. For document layouts:

| Context | Suggested value |
|---------|----------------|
| Body text line spacing | 1.5× font size |
| Paragraph spacing | `space-12` to `space-16` |
| Section spacing | `space-32` to `space-48` |
| Page margin | `space-48` to `space-64` |
| Table cell padding | `space-8` to `space-12` |

---

## Logo

<!-- To be defined — placement, sizing, and variant rules for PDF headers/footers -->

---

## Document Structure

<!-- To be filled in — cover page, table of contents, header/footer, page numbering conventions -->

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

Wider margins (56px or 64px) are preferred for text-heavy documents — use 40px only when space is tight.

### Spacing reference at A4 scale
| Context | Recommended token |
|---------|------------------|
| Page margin (min) | `space-40` → use 40px |
| Page margin (comfortable) | `space-56` or `space-64` |
| Section gap | `space-32` to `space-48` |
| Paragraph gap | `space-12` to `space-16` |
| Table cell padding | `space-8` to `space-12` |

---

*FDS 2026 PDF — based on Facilio Design System tokens.*
