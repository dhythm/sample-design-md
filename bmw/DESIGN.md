# BMW Design System

BMW's design identity prioritizes **precision, performance, and German industrial confidence** through specific technical choices.

## Core Visual Language

The system uses BMWTypeNextLatin Light (weight 300) for massive uppercase display headings paired with sharp angular geometry. Dark hero sections featuring automotive photography alternate with clean white content areas, creating "showroom lighting rhythm."

## Color System

### Primary Brand Colors

| Color Name      | Hex       | Usage                                                    |
| --------------- | --------- | -------------------------------------------------------- |
| Pure White      | `#ffffff` | Primary surface, card backgrounds, --site-context-theme-color |
| BMW Blue        | `#1c69d4` | Interactive accents, --site-context-highlight-color, focus states |
| BMW Focus Blue  | `#0653b6` | Keyboard focus, active states, --site-context-focus-color |

### Neutral Scale

| Color Name | Hex       | Usage                                                |
| ---------- | --------- | ---------------------------------------------------- |
| Near Black | `#262626` | Primary text on light surfaces, dark link text       |
| Meta Gray  | `#757575` | Secondary text, metadata, --site-context-metainfo-color |
| Silver     | `#bbbbbb` | Tertiary text, muted links, footer elements          |

### CSS Custom Properties

```css
--site-context-highlight-color: #1c69d4;
--site-context-focus-color: #0653b6;
--site-context-metainfo-color: #757575;
--site-context-theme-color: #ffffff;
```

### Key Rules

- BMW Blue used **only for interactive elements and focus states, never decoratively**
- Hover state: links transition to white (#ffffff)
- Depth created through dark/light contrast, not shadows

## Typography

### Font Family

**Primary**: BMWTypeNextLatin with fallback: Helvetica, Arial, Hiragino Kaku Gothic ProN, Hiragino Sans, Meiryo

### Hierarchy

| Element             | Size           | Weight | Line Height | Notes                    |
| ------------------- | -------------- | ------ | ----------- | ------------------------ |
| Display Hero        | 60px (3.75rem) | 300    | 1.30        | Uppercase transformation |
| Section Heading     | 32px (2.00rem) | 400    | 1.30        | Major section titles     |
| Navigation Emphasis | 18px (1.13rem) | 900    | 1.30        | Navigation primary links |
| Body Text           | 16px (1.00rem) | 400    | 1.15        | Standard paragraph text  |
| Button (Bold)       | 16px (1.00rem) | 700    | 1.20–2.88   | Primary CTA buttons      |
| Button (Standard)   | 16px (1.00rem) | 400    | 1.15        | Secondary buttons        |

### Weight Scale

- 300: Display authority (whispered)
- 400: Body efficiency
- 700: Button emphasis
- 900: Navigation stark authority

## Spacing

- **Base unit**: 8px
- **Scale**: 1px, 5px, 8px, 10px, 12px, 15px, 16px, 20px, 24px, 30px, 32px, 40px, 45px, 56px, 60px

## Components

### Buttons

- Font: 16px, weight 700 (primary) / 400 (secondary)
- Border: 1px solid white bottom-border on dark surfaces
- Border-radius: 0px (sharp rectangular)
- No shadows

### Navigation

- Font: 18px, weight 900, white text on dark background
- BMW logo: 54x54px
- Horizontal on desktop, hamburger on mobile

### Hero Section

- Full-bleed dark automotive photography
- 60px uppercase heading, weight 300, white text
- Generous showroom-like spacing

### Cards / Containers

- Border-radius: 0px
- White background on light sections
- No borders, no shadows — flat surfaces

### Footer

- Multi-column link grid, stacks on mobile
- Meta gray and silver text

## Non-Negotiable Elements

- **Zero border-radius** throughout — angular, sharp-cornered, uncompromisingly geometric
- Full-bleed automotive photography as primary visual content
- CSS variable-driven theming using `--site-context-*` tokens

## Responsive Breakpoints

| Breakpoint    | Range         |
| ------------- | ------------- |
| Mobile Small  | <375px        |
| Mobile        | 375–480px     |
| Mobile Large  | 480–640px     |
| Tablet Small  | 640–768px     |
| Tablet        | 768–920px     |
| Desktop Small | 920–1024px    |
| Desktop       | 1024–1280px   |
| Large Desktop | 1280–1440px   |
| Ultra-wide    | 1440–1600px   |
