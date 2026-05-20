# FDS 2026 — Design System

A structured design system color palette extracted from Figma, packaged as design tokens and LLM-ready skills files.

## Color Palette

**7 color families · 11 shades each · 77 total tokens**

| Family | Base (06) | Range |
|--------|-----------|-------|
| 🟣 Violet | `#623cf6` | `#f0ecfe` → `#0d0829` |
| 🔵 Blue | `#2b7fff` | `#eff6ff` → `#162456` |
| 🟡 Yellow | `#fdc700` | `#fefce8` → `#432004` |
| 🟢 Green | `#00c950` | `#f0fdf4` → `#032e15` |
| 🟠 Orange | `#ff8904` | `#fff7ed` → `#441306` |
| 🪨 Charcoal | `#62748e` | `#f8fafc` → `#020618` |
| ⬜ Grey | `#737373` | `#fafafa` → `#0a0a0a` |

Scale: `01` = lightest → `11` = darkest

## File Structure

```
fds-2026/
├── tokens/
│   ├── colors.json          # W3C Design Token format
│   ├── colors.css           # CSS custom properties
│   └── colors.tailwind.js   # Tailwind CSS theme config
├── skills/
│   └── SKILL.md             # LLM skills / prompt context file
└── README.md
```

## Usage

### CSS
```css
@import 'tokens/colors.css';

.button-primary {
  background: var(--color-violet-06);
  color: white;
}
.button-primary:hover {
  background: var(--color-violet-07);
}
```

### Tailwind CSS
```js
// tailwind.config.js
const fdsColors = require('./tokens/colors.tailwind.js');

module.exports = {
  theme: {
    extend: {
      colors: fdsColors,
    },
  },
};
```

```html
<button class="bg-violet-06 hover:bg-violet-07 text-white">
  Click me
</button>
```

### JavaScript / TypeScript
```js
import tokens from './tokens/colors.json';

const primaryBrand = tokens.color.violet['06'].$value; // '#623cf6'
```

## LLM Usage

Feed `skills/SKILL.md` to any LLM (Claude, GPT-4, Gemini, etc.) as a system prompt or context file. It includes:

- Full color table with hex values and semantic use cases
- Semantic role mappings (primary, success, warning, etc.)
- Specific prompt instructions for consistent design generation
- Example component specs (buttons, backgrounds, text)

```
System: [paste contents of skills/SKILL.md]
User: Create a card component with a success badge using FDS 2026 colors.
```

## Source

Extracted from Figma file `fds-2026` (`eFOBPdj9il7u3R5KP7GEns`), Section 1.
