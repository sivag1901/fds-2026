# FDS 2026 — Facilio Design System

A structured design system defining color tokens, typography, and logo usage for Facilio's product.

---

## Color Palette

**7 color families · 11 shades each · 77 total tokens** · Scale: `01` = lightest → `11` = darkest

| Family | Role | Base (06) |
|--------|------|-----------|
| Violet | **Primary** — brand, CTAs, focus | `#623cf6` |
| Blue | Accent — info | `#2b7fff` |
| Yellow | Accent — warning | `#fdc700` |
| Green | Accent — success | `#00c950` |
| Orange | Accent — caution / error | `#ff8904` |
| Charcoal | **Neutral** — text, borders, surfaces | `#62748e` |
| Grey | **Neutral** — structural only | `#737373` |

---

## Spacing

**28 tokens** · 4px steps up to 24px, then 8px steps to 200px max

| Range | Step | Values |
|-------|------|--------|
| 4px – 24px | 4px | 4, 8, 12, 16, 20, 24 |
| 32px – 200px | 8px | 32, 40, 48 … 192, 200 |

```css
@import 'tokens/spacing.css';

.card    { padding: var(--fds-space-16); gap: var(--fds-space-8); }
.section { padding-top: var(--fds-space-64); }
```

---

## Typography

| Role | Font | Applied To |
|------|------|------------|
| Title | **Darker Grotesque** | h1, h2, h3, h4 |
| Body | **Inter** | h5, h6, body copy, labels, inputs |
| Mono | **IBM Plex Mono** | Tags, numericals, code |

All font files are included locally under `fonts/`.

---

## Logo

For web, always use the **classic** variant. Choose dark or white based on background:

| Background | File |
|------------|------|
| Light | `logos/classic/facilio-dark.svg` |
| Dark | `logos/classic/facilio-white.svg` |

---

## File Structure

```
fds-2026/
├── tokens/
│   ├── colors.json         # W3C Design Token format
│   ├── colors.css          # CSS custom properties (--fds-color-*)
│   ├── colors.js           # Plain JavaScript module
│   ├── typography.css      # @font-face + --fds-font-* tokens
│   ├── spacing.json        # W3C Design Token format
│   ├── spacing.css         # CSS custom properties (--fds-space-*)
│   └── spacing.js          # Plain JavaScript module
├── fonts/
│   ├── Darker_Grotesque/   # Variable font (wght 300–900)
│   ├── Inter/              # Variable font (wght 100–900)
│   └── IBM_Plex_Mono/      # Static files (Regular → Bold)
├── logos/
│   ├── classic/            # Web — facilio-dark.svg / facilio-white.svg
│   └── modern/             # Non-web use
├── skills/
│   ├── SKILL.md            # Base rules — all mediums
│   ├── web.md              # Web UI components and pages
│   ├── poster.md           # Poster and large-format graphics
│   ├── pdf.md              # PDF documents and reports
│   └── presentation.md     # Slide decks and presentations
└── README.md
```

---

## Usage

### CSS

```css
@import 'tokens/colors.css';
@import 'tokens/typography.css';

.button-primary {
  background: var(--fds-violet-06);
  color: white;
  font-family: var(--fds-font-body);
}
.button-primary:hover {
  background: var(--fds-violet-07);
}

h1 {
  font-family: var(--fds-font-title);
  color: var(--fds-charcoal-10);
}

.tag {
  font-family: var(--fds-font-mono);
}
```

### JavaScript

```js
import tokens from './tokens/colors.json';
const primaryBrand = tokens.color.violet['06'].$value; // '#623cf6'
```

```js
const fdsColors = require('./tokens/colors.js');
const primaryBrand = fdsColors.violet['06']; // '#623cf6'
```

---

## LLM Usage

Feed the relevant skill file to any LLM as a system prompt or context file.

| Task | File to use |
|------|------------|
| Web UI / components | `skills/web.md` |
| Poster / large-format | `skills/poster.md` |
| PDF / document | `skills/pdf.md` |
| Slide deck | `skills/presentation.md` |
| General / base rules | `skills/SKILL.md` |

```
System: [paste contents of skills/web.md]
User: Create a status badge component using FDS 2026.
```

---

## Source

Extracted from Figma file `fds-2026` (`eFOBPdj9il7u3R5KP7GEns`), Section 1.
