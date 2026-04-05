# Raycast Design System

## Visual Theme & Atmosphere

Raycast's marketing aesthetic draws inspiration from precision instruments, employing an almost-black blue-tinted background (`#07080a`) that evokes macOS native applications. The design leverages multi-layer box-shadows with inset highlights that simulate physical depth, creating the impression of glass elements on a dark surface.

The brand employs Raycast Red (`#FF6363`) strategically as a punctuation accent rather than a dominant color. Typography relies on Inter throughout, with extensive OpenType features enabling `calt`, `kern`, `liga`, and `ss03`. The positive letter-spacing (0.2px-0.4px) distinguishes the dark UI approach, providing an airy, breathable quality.

**Core characteristics:**
- Near-black blue-shifted background (`#07080a`)
- macOS shadow system with inset highlights
- Raycast Red (`#FF6363`) as accent punctuation
- Subtle rgba white borders (0.06-0.1 opacity)
- Keyboard shortcut styling with gradient key caps

## Color Palette & Roles

**Primary colors:**
- Near-Black Blue (`#07080a`): page background
- Pure White (`#ffffff`): headings and high-emphasis elements
- Raycast Red (`#FF6363` / `hsl(0, 100%, 69%)`): brand accent

**Secondary accents:**
- Raycast Blue (`hsl(202, 100%, 67%)` / ~`#55b3ff`)
- Raycast Green (`hsl(151, 59%, 59%)` / ~`#5fc992`)
- Raycast Yellow (`hsl(43, 100%, 60%)` / ~`#ffbc33`)

**Surfaces & backgrounds:**
- Surface 100: `#101111`
- Card Surface: `#1b1c1e`
- Neutral grays: `#f9f9f9` through `#434345`
- Border colors: `hsl(195, 5%, 15%)`, `#2f3031`

## Typography

**Font Families:**
- Primary: `Inter` (humanist sans-serif)
- System: `SF Pro Text` (Apple system font)
- Monospace: `GeistMono` (Vercel's monospace)

**OpenType features:** `calt`, `kern`, `liga`, `ss03` enabled globally; `ss02`, `ss08` on display text; `liga` disabled on hero headings.

**Typography Hierarchy:**

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 64px | 600 | 1.10 | 0px |
| Section Display | 56px | 400 | 1.17 | 0.2px |
| Section Heading | 24px | 500 | normal | 0.2px |
| Card Heading | 22px | 400 | 1.15 | 0px |
| Sub-heading | 20px | 500 | 1.60 | 0.2px |
| Body Large | 18px | 400 | 1.15 | 0.2px |
| Body | 16px | 500 | 1.60 | 0.2px |
| Button | 16px | 600 | 1.15 | 0.3px |
| Nav Link | 16px | 500 | 1.40 | 0.3px |
| Caption | 14px | 500 | 1.14 | 0.2px |
| Small | 12px | 600 | 1.33 | 0px |

## Spacing System

**Base unit:** 8px

**Scale:** 1px, 2px, 3px, 4px, 8px, 10px, 12px, 16px, 20px, 24px, 32px, 40px

**Section padding:** 80px-120px vertical between major sections
**Card padding:** 16px-32px internal spacing
**Component gaps:** 8px-16px between related elements

## Depth & Elevation

| Level | Treatment |
|-------|-----------|
| 0 (Void) | No shadow, `#07080a` surface |
| 1 (Subtle) | `rgba(0, 0, 0, 0.28) 0px 1.189px 2.377px` |
| 2 (Ring) | Outer: `rgb(27, 28, 30) 0px 0px 0px 1px` + Inset: `rgb(7, 8, 10) 0px 0px 0px 1px` |
| 3 (Button) | Inset: `rgba(255, 255, 255, 0.05) 0px 1px 0px 0px` + Border: `rgba(255, 255, 255, 0.25) 0px 0px 0px 1px` |
| 5 (Floating) | Outer: `rgba(0, 0, 0, 0.5) 0px 0px 0px 2px` + Glow: `rgba(255, 255, 255, 0.19) 0px 0px 14px` |

## Border Radius

- 2px-3px: Micro-elements, code spans
- 4px-5px: Keyboard keys, small interactive elements
- 6px: Buttons, badges, tags
- 8px: Input fields, inline components
- 12px: Standard cards, product screenshots
- 16px: Large cards, feature sections
- 20px: Hero cards, prominent containers
- 86px+: Pill buttons, nav CTAs

## Buttons / CTAs

- **Primary Pill:** Transparent bg, white text, 86px radius, inset shadow
- **Secondary Button:** Transparent bg, white text, 6px radius, 1px border
- **Ghost Button:** No bg/border, gray text (#6a6b6c), 86px radius
- **CTA (Download):** Semi-transparent white bg `hsla(0, 0%, 100%, 0.815)`, dark text (#18191a), pill shape
- **Transition:** All buttons use opacity transition for hover

## Cards & Containers

- **Standard Card:** `#101111` surface, `1px solid rgba(255, 255, 255, 0.06)` border, 12px-16px border-radius
- **Elevated Card:** Outer ring `rgb(27, 28, 30) 0px 0px 0px 1px` + inner inset
- **Feature Card:** 16px-20px border-radius, warm glow `rgba(215, 201, 175, 0.05) 0px 0px 20px 5px`

## Layout & Grid

- **Max width:** ~1200px container, centered
- **Column patterns:** Single-column hero, 2-3 column feature grids
- **Responsive breakpoints:** <600px mobile, 600-768px small tablet, 768-1024px tablet, 1024-1200px desktop, >1200px large desktop
