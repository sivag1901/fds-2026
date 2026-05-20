# FDS 2026 — Design System Skills File
> Feed this file to any LLM to generate on-brand UI components, screens, and design tokens.

---

## What is FDS 2026?

FDS 2026 is a design system with a structured 7-family color palette sourced from Figma (`fds-2026`, Section 1). Every color has 11 shades numbered `01` (lightest) → `11` (darkest). The mid-point base shade is typically `05` or `06`.

---

## Color Families & Hex Values

### Violet
| Token | Hex | Use |
|-------|-----|-----|
| violet-01 | `#f0ecfe` | Background tints, hover states |
| violet-02 | `#ddd5fd` | Subtle fills |
| violet-03 | `#c0adfb` | Light accents |
| violet-04 | `#a386f9` | Borders, icons |
| violet-05 | `#8560f8` | Secondary elements |
| violet-06 | `#623cf6` | **Base / Primary brand** |
| violet-07 | `#4e2fcc` | Hover on base |
| violet-08 | `#3b23a2` | Active/pressed |
| violet-09 | `#291878` | Dark text on light BG |
| violet-10 | `#180e4f` | Deep backgrounds |
| violet-11 | `#0d0829` | Near-black, darkmode surfaces |

### Blue
| Token | Hex | Use |
|-------|-----|-----|
| blue-01 | `#eff6ff` | Info backgrounds |
| blue-02 | `#dbeafe` | Info tints |
| blue-03 | `#bedbff` | Light info fills |
| blue-04 | `#8ec5ff` | Info icons, borders |
| blue-05 | `#51a2ff` | Info accents |
| blue-06 | `#2b7fff` | **Base / Links** |
| blue-07 | `#155dfc` | Hover on links |
| blue-08 | `#1447e6` | Active links |
| blue-09 | `#193cb8` | Dark info text |
| blue-10 | `#1c398e` | Deep blue surfaces |
| blue-11 | `#162456` | Near-black blue |

### Yellow
| Token | Hex | Use |
|-------|-----|-----|
| yellow-01 | `#fefce8` | Warning backgrounds |
| yellow-02 | `#fef9c2` | Warning tints |
| yellow-03 | `#fff085` | Light warning fills |
| yellow-04 | `#ffdf20` | Warning highlights |
| yellow-05 | `#fdc700` | **Base / Warning** |
| yellow-06 | `#f0b100` | Hover on warning |
| yellow-07 | `#d08700` | Active warning |
| yellow-08 | `#a65f00` | Dark warning text |
| yellow-09 | `#894b00` | Deep amber |
| yellow-10 | `#733e0a` | Dark amber |
| yellow-11 | `#432004` | Near-black amber |

### Green
| Token | Hex | Use |
|-------|-----|-----|
| green-01 | `#f0fdf4` | Success backgrounds |
| green-02 | `#dcfce7` | Success tints |
| green-03 | `#b9f8cf` | Light success fills |
| green-04 | `#7bf1a8` | Success highlights |
| green-05 | `#05df72` | Vivid success |
| green-06 | `#00c950` | **Base / Success** |
| green-07 | `#00a63e` | Hover on success |
| green-08 | `#008236` | Active success |
| green-09 | `#016630` | Dark success text |
| green-10 | `#0d542b` | Deep green |
| green-11 | `#032e15` | Near-black green |

### Orange
| Token | Hex | Use |
|-------|-----|-----|
| orange-01 | `#fff7ed` | Caution backgrounds |
| orange-02 | `#ffedd4` | Caution tints |
| orange-03 | `#ffd6a7` | Light caution fills |
| orange-04 | `#ffb86a` | Caution highlights |
| orange-05 | `#ff8904` | **Base / Caution** |
| orange-06 | `#ff6900` | Hover on caution |
| orange-07 | `#f54900` | Active caution |
| orange-08 | `#ca3500` | Dark caution text |
| orange-09 | `#9f2d00` | Deep orange |
| orange-10 | `#7e2a0c` | Dark orange |
| orange-11 | `#441306` | Near-black orange |

### Charcoal
| Token | Hex | Use |
|-------|-----|-----|
| charcoal-01 | `#f8fafc` | Page backgrounds |
| charcoal-02 | `#f1f5f9` | Card backgrounds |
| charcoal-03 | `#e2e8f0` | Dividers, borders |
| charcoal-04 | `#cad5e2` | Input borders |
| charcoal-05 | `#90a1b9` | Placeholder text |
| charcoal-06 | `#62748e` | **Base / Muted text** |
| charcoal-07 | `#45556c` | Secondary text |
| charcoal-08 | `#314158` | Body text |
| charcoal-09 | `#1d293d` | Strong body text |
| charcoal-10 | `#0f172b` | Headings |
| charcoal-11 | `#020618` | Near-black, darkmode |

### Grey
| Token | Hex | Use |
|-------|-----|-----|
| grey-01 | `#fafafa` | Page backgrounds |
| grey-02 | `#f5f5f5` | Subtle surfaces |
| grey-03 | `#e5e5e5` | Borders, dividers |
| grey-04 | `#d4d4d4` | Input borders |
| grey-05 | `#a1a1a1` | Placeholder text |
| grey-06 | `#737373` | **Base / Muted** |
| grey-07 | `#525252` | Secondary text |
| grey-08 | `#404040` | Body text |
| grey-09 | `#262626` | Strong text |
| grey-10 | `#171717` | Headings |
| grey-11 | `#0a0a0a` | Near-black |

---

## Semantic Roles (How to Use Colors)

```
Primary action:       violet-06  (#623cf6)
Primary hover:        violet-07  (#4e2fcc)
Primary active:       violet-08  (#3b23a2)
Primary subtle bg:    violet-01  (#f0ecfe)

Link / info:          blue-06    (#2b7fff)
Link hover:           blue-07    (#155dfc)
Info background:      blue-01    (#eff6ff)

Success:              green-06   (#00c950)
Success background:   green-01   (#f0fdf4)
Success text:         green-09   (#016630)

Warning:              yellow-05  (#fdc700)
Warning background:   yellow-01  (#fefce8)
Warning text:         yellow-09  (#894b00)

Caution / danger:     orange-06  (#ff6900)
Caution background:   orange-01  (#fff7ed)
Caution text:         orange-09  (#9f2d00)

Body text:            charcoal-08 (#314158)
Muted text:           charcoal-06 (#62748e)
Page background:      charcoal-01 (#f8fafc)
Border:               charcoal-03 (#e2e8f0)

Neutral text:         grey-08    (#404040)
Neutral border:       grey-03    (#e5e5e5)
Neutral surface:      grey-01    (#fafafa)
```

---

## LLM Prompt Instructions

When generating UI components using FDS 2026:

1. **Always use token names** (e.g. `violet-06`) in reasoning, then resolve to hex for code output.
2. **Light mode defaults**: backgrounds use `charcoal-01` or `grey-01`; body text uses `charcoal-08` or `charcoal-09`.
3. **Dark mode**: flip — backgrounds use `charcoal-10` or `charcoal-11`; text uses `charcoal-01` or `charcoal-02`.
4. **Primary brand color** is `violet-06`. Use violet shades for buttons, active states, and focus rings.
5. **Never use grey for interactive elements** — grey is for neutral/structural use only. Use charcoal for text hierarchy.
6. **Accessibility**: Ensure contrast ratios. Light text on `violet-06` passes AA. Dark text (`charcoal-09+`) on `01`–`03` tints passes AA.
7. **Status colors**: green = success, yellow = warning, orange = caution/error, blue = info.
8. **11-step scale rule**: Steps `01`–`03` = tint backgrounds. Steps `04`–`05` = light accents. Step `06` = base. Steps `07`–`08` = hover/active. Steps `09`–`11` = dark text / deep surfaces.

---

## File References

| File | Description |
|------|-------------|
| `tokens/colors.json` | W3C Design Token Community Group format |
| `tokens/colors.css` | CSS custom properties (`:root` variables) |
| `tokens/colors.tailwind.js` | Tailwind CSS `theme.colors` config |
| `skills/SKILL.md` | This file — LLM prompt context |

---

## Example: Button Component Spec

```
Primary Button:
  background:       violet-06 (#623cf6)
  text:             white
  hover background: violet-07 (#4e2fcc)
  active:           violet-08 (#3b23a2)
  focus ring:       violet-04 (#a386f9) at 3px offset
  disabled:         charcoal-04 bg, charcoal-06 text

Secondary Button:
  background:       transparent
  border:           violet-06 (#623cf6)
  text:             violet-06 (#623cf6)
  hover background: violet-01 (#f0ecfe)

Danger Button:
  background:       orange-06 (#ff6900)
  text:             white
  hover:            orange-07 (#f54900)
```

---

*FDS 2026 — Sourced from Figma file `eFOBPdj9il7u3R5KP7GEns`, Section 1. 77 tokens across 7 families.*
