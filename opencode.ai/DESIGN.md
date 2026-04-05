# OpenCode Design System Summary

OpenCode employs a "terminal-native, monospace-first aesthetic" built on Berkeley Mono exclusively. The palette centers on warm near-black (`#201d1d`) backgrounds paired with off-white text (`#fdfcfc`), deliberately avoiding pure black/white for a "sophisticated terminal emulator" feel.

## Core Design Elements

**Typography**: Berkeley Mono serves as the sole typeface across all elements. Hierarchy relies on three weight levels -- 700 for headings, 500 for interactive content, 400 for body text -- rather than font variation.

**Color System**: Three primary tones (dark, light, gray) anchor the design, supplemented by Apple HIG semantic colors: blue (`#007aff`), red (`#ff3b30`), green (`#30d158`), orange (`#ff9f0a`).

**Spacing & Borders**: An 8px base grid scales upward; border radius stays at 4px except inputs (6px). Borders use "warm transparent black" (`rgba(15, 0, 0, 0.12)`), not neutral gray.

## Structural Approach

The layout favors a narrow single-column design (~800-900px), flat surfaces without shadows, and section separation through generous vertical spacing rather than dividers. Interactive states follow three-stage sequences (default -> hover -> active) using darkened semantic colors.

This system prioritizes readability and focus through constraint, monospace consistency, and a deliberately warm dark aesthetic that mirrors terminal environments.

---

## Color Palette & Roles

### Primary Colors
- **OpenCode Dark** (`#201d1d`): rgb(32, 29, 29) -- primary background, button fills, link text
- **OpenCode Light** (`#fdfcfc`): primary text on dark surfaces, button text
- **Mid Gray** (`#9a9898`): secondary text, muted links

### Secondary Colors
- **Dark Surface** (`#302c2c`): elevated surfaces, subtle differentiation
- **Border Gray** (`#646262`): stronger borders, outline rings
- **Light Surface** (`#f1eeee`): light mode surface, subtle background variation

### Accent Colors
- **Accent Blue** (`#007aff`): primary accent, links, interactive highlights
- **Accent Blue Hover** (`#0056b3`): darker blue for hover states
- **Accent Blue Active** (`#004085`): deepest blue for pressed/active states

### Semantic Colors
- **Danger Red** (`#ff3b30`): error states, destructive actions
- **Danger Hover** (`#d70015`): darker red for hover
- **Danger Active** (`#a50011`): deepest red for pressed states
- **Success Green** (`#30d158`): success states, positive feedback
- **Warning Orange** (`#ff9f0a`): warning states, caution signals
- **Warning Hover** (`#cc7f08`): darker orange for hover
- **Warning Active** (`#995f06`): deepest orange for pressed states

### Text Colors
- **Text Muted** (`#6e6e73`): muted labels, disabled text, placeholder content
- **Text Secondary** (`#424245`): secondary text on light backgrounds, captions

### Border Colors
- **Border Warm** (`rgba(15, 0, 0, 0.12)`): primary border color with warm transparent black
- **Border Tab** (`#9a9898`): tab underline border, 2px solid bottom
- **Border Outline** (`#646262`): 1px solid outline border for containers

---

## Typography Rules

### Font Family
- **Universal**: Berkeley Mono
- **Fallbacks**: IBM Plex Mono, ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, Liberation Mono, Courier New, monospace

### Hierarchy Table

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Heading 1 | 38px (2.38rem) | 700 | 1.50 |
| Heading 2 | 16px (1.00rem) | 700 | 1.50 |
| Body | 16px (1.00rem) | 400 | 1.50 |
| Body Medium | 16px (1.00rem) | 500 | 1.50 |
| Body Tight | 16px (1.00rem) | 500 | 1.00 |
| Caption | 14px (0.88rem) | 400 | 2.00 |

### Typography Principles
- Single font family across all elements
- Weight hierarchy: 700 (headings), 500 (interactive/medium), 400 (body)
- Standard line-height 1.50 for readability
- Relaxed 2.00 line-height on captions for visual separation
- Tight 1.00 line-height for interactive elements (tabs, labels)

---

## Component Stylings

### Buttons

**Primary (Dark Fill)**
- Background: `#201d1d`
- Text: `#fdfcfc`
- Padding: 4px 20px
- Radius: 4px
- Font: 16px Berkeley Mono, weight 500, line-height 2.00
- Outline: `rgb(253, 252, 252) none 0px`

### Inputs

**Email Input**
- Background: `#f8f7f7`
- Text: `#201d1d`
- Border: `1px solid rgba(15, 0, 0, 0.12)`
- Padding: 20px
- Radius: 6px
- Font: Berkeley Mono, standard size

### Links

**Default Link**
- Color: `#201d1d`
- Decoration: underline 1px
- Font-weight: 500

**Light Link**
- Color: `#fdfcfc`
- Decoration: none

**Muted Link**
- Color: `#9a9898`
- Decoration: none

### Tabs

**Tab Navigation**
- Border-bottom: `2px solid #9a9898` (active indicator)
- Font: 16px, weight 500, line-height 1.00

### Navigation
- Berkeley Mono throughout
- Brand logotype left-aligned in monospace
- Links at 16px, weight 500, with underline decoration
- Dark background matching page (`#201d1d`)
- No backdrop blur or transparency

---

## Layout Principles

### Spacing System
- Base unit: 8px
- Fine scale: 1px, 2px, 4px
- Standard scale: 8px, 12px, 16px, 20px, 24px
- Extended scale: 32px, 40px, 48px, 64px, 80px, 96px
- Follows clean 4/8px grid with consistent doubling

### Grid & Container
- Max content width: approximately 800-900px
- Single-column layout as primary pattern
- Centered content with generous horizontal margins
- Section separation via spacing (48-96px) not borders

### Border Radius Scale
- Micro (4px): Default for all elements
- Input (6px): Form inputs only

---

## Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (Level 0) | No shadow, no border | Default state |
| Border Subtle (Level 1) | `1px solid rgba(15, 0, 0, 0.12)` | Dividers, input borders, rules |
| Border Tab (Level 2) | `2px solid #9a9898` bottom only | Active tab indicator |
| Border Outline (Level 3) | `1px solid #646262` | Container outlines, elevated elements |

**Shadow Philosophy**: Zero shadow values -- depth through borders and background color shifts only. Flat terminal aesthetic with no elevation illusion.

---

## Interaction & Motion

### Hover States
- Link color shift to `#007aff` or underline style change
- Button: subtle background lightening or border emphasis
- Three-stage sequence for semantic colors:
  - Accent Blue: `#007aff` -> `#0056b3` -> `#004085`
  - Danger Red: `#ff3b30` -> `#d70015` -> `#a50011`
  - Warning Orange: `#ff9f0a` -> `#cc7f08` -> `#995f06`

### Focus States
- Border-based focus with increased opacity or solid color
- No shadow-based focus rings
- Uses outline or border color shift to `#007aff`

### Transitions
- Minimal transitions (terminal-inspired, favors instant changes)
- Color transitions: 100-150ms for subtle feedback
- No scale, rotate, or complex transforms

---

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | <640px | Single column, reduced padding, heading scales |
| Tablet | 640-1024px | Content expands, slight padding increase |
| Desktop | >1024px | Full width (~800-900px centered), maximum whitespace |

### Scaling Strategy
- Heading: 38px -> 28px -> 24px on smaller screens
- Section spacing: 96px -> 64px -> 48px on mobile
- Navigation: horizontal links -> hamburger/drawer on mobile
- Feature lists: maintain single-column, reduce padding
- Terminal hero: full-width, reduce internal padding
- Footer columns: multi-column -> stacked single column
