# Wise Design System

## Brand Overview

Wise (formerly TransferWise) is an international money transfer and multi-currency account platform. The design system communicates confidence, clarity, and approachability through massive typography and a distinctive lime-green accent.

## Core Design Philosophy

- **Extreme boldness IS the brand** — visual weight communicates authority
- **Confidence, not lightness** — body text defaults to weight 600
- **Physical interaction** — buttons grow and compress rather than changing color
- **Minimal depth** — ring shadows replace traditional box shadows
- **Intentional density** — tight line-heights create stamped, pressed, physical text

## Color Palette

### Primary Colors

| Token              | Hex       | Usage                              |
| ------------------ | --------- | ---------------------------------- |
| Wise Green         | `#9fe870` | Primary CTA buttons, key accents   |
| Dark Green         | `#163300` | Text on green buttons              |
| Near Black         | `#0e0f0c` | Primary text color                 |
| Off White          | `#f2f0e6` | Page background                    |
| White              | `#ffffff` | Card backgrounds                   |

### Semantic Colors

| Token           | Hex       | Usage              |
| --------------- | --------- | ------------------ |
| Positive Green  | `#2e7d32` | Success states      |
| Danger Red      | `#d03238` | Error states        |
| Warning Yellow  | `#ffd11a` | Warning states      |
| Info Blue       | `#1565c0` | Informational       |

### Extended Palette

| Token            | Hex       | Usage                        |
| ---------------- | --------- | ---------------------------- |
| Navy             | `#163300` | Dark section backgrounds     |
| Light Green      | `#d4f4bc` | Subtle green accents/badges  |
| Medium Gray      | `#6b6b6b` | Secondary text               |
| Border Gray      | `#e0e0d8` | Dividers, card borders       |

## Typography

### Font Stack

- **Display / Headlines**: Wise Sans, weight 900
- **Body / UI**: Inter, weight 600 (default), weight 400 (secondary)
- **Monospace**: 'SF Mono', 'Fira Code', monospace

### Type Scale

| Role         | Font        | Size   | Weight | Line Height | Letter Spacing |
| ------------ | ----------- | ------ | ------ | ----------- | -------------- |
| Display XL   | Wise Sans   | 72px   | 900    | 0.85        | -2px           |
| Display      | Wise Sans   | 56px   | 900    | 0.85        | -1.5px         |
| Heading 1    | Wise Sans   | 48px   | 900    | 0.9         | -1px           |
| Heading 2    | Wise Sans   | 36px   | 900    | 0.95        | -0.5px         |
| Heading 3    | Inter       | 24px   | 700    | 1.2         | -0.25px        |
| Body Large   | Inter       | 18px   | 600    | 1.5         | 0              |
| Body         | Inter       | 16px   | 600    | 1.5         | 0              |
| Body Small   | Inter       | 14px   | 400    | 1.4         | 0              |
| Caption      | Inter       | 12px   | 400    | 1.3         | 0.5px          |

### OpenType Features

All text should include `font-feature-settings: "calt"` for contextual alternates.

## Spacing System

| Token | Value |
| ----- | ----- |
| xs    | 4px   |
| sm    | 8px   |
| md    | 16px  |
| lg    | 24px  |
| xl    | 32px  |
| 2xl   | 48px  |
| 3xl   | 64px  |
| 4xl   | 96px  |
| 5xl   | 128px |

## Border Radius

| Element  | Radius  |
| -------- | ------- |
| Buttons  | 9999px  |
| Cards    | 16px    |
| Inputs   | 12px    |
| Badges   | 8px     |
| Large    | 40px    |

## Shadows

Wise avoids traditional box shadows. Instead, use ring shadows:

```css
/* Ring shadow for cards */
box-shadow: 0 0 0 1px rgba(14, 15, 12, 0.08);

/* Ring shadow for focus */
box-shadow: 0 0 0 3px rgba(159, 232, 112, 0.4);

/* Elevated ring */
box-shadow: 0 0 0 1px rgba(14, 15, 12, 0.08), 0 2px 8px rgba(14, 15, 12, 0.04);
```

## Buttons

### Primary Button

```css
.btn-primary {
  background: #9fe870;
  color: #163300;
  font-family: 'Inter', sans-serif;
  font-weight: 700;
  font-size: 16px;
  padding: 14px 32px;
  border-radius: 9999px;
  border: none;
  cursor: pointer;
  transition: transform 0.2s cubic-bezier(0.34, 1.56, 0.64, 1);
}
.btn-primary:hover {
  transform: scale(1.05);
}
.btn-primary:active {
  transform: scale(0.95);
}
```

### Secondary Button

```css
.btn-secondary {
  background: transparent;
  color: #0e0f0c;
  font-weight: 700;
  padding: 14px 32px;
  border-radius: 9999px;
  border: 2px solid #0e0f0c;
  cursor: pointer;
  transition: transform 0.2s cubic-bezier(0.34, 1.56, 0.64, 1);
}
.btn-secondary:hover {
  transform: scale(1.05);
}
.btn-secondary:active {
  transform: scale(0.95);
}
```

## Interactive Behavior

- **Hover**: `transform: scale(1.05)` with spring-like cubic-bezier
- **Active/Press**: `transform: scale(0.95)`
- **Transition**: `0.2s cubic-bezier(0.34, 1.56, 0.64, 1)` for bouncy feel
- **Focus**: Ring shadow `0 0 0 3px rgba(159, 232, 112, 0.4)`
- All interactive elements must include scale animations

## Cards

```css
.card {
  background: #ffffff;
  border-radius: 16px;
  padding: 32px;
  box-shadow: 0 0 0 1px rgba(14, 15, 12, 0.08);
  transition: transform 0.2s cubic-bezier(0.34, 1.56, 0.64, 1);
}
.card:hover {
  transform: scale(1.02);
  box-shadow: 0 0 0 1px rgba(14, 15, 12, 0.08), 0 2px 8px rgba(14, 15, 12, 0.04);
}
```

## Layout

- **Max width**: 1200px
- **Content padding**: 24px (mobile), 32px (tablet), 48px (desktop)
- **Section spacing**: 96px–128px between major sections
- **Grid**: 12-column grid, 24px gap

## Key Design Rules

1. Wise Sans weight 900 is identity — never use lighter weights for display
2. The 0.85 line-height on display creates intentional density
3. Lime green (`#9fe870`) is reserved for buttons and key accents only
4. Minimal shadows — ring shadows replace traditional depth
5. Scale animations required on all interactive elements
6. Body text at weight 600 creates a consistently confident voice
7. Off-white background (`#f2f0e6`) — never pure white for page backgrounds
