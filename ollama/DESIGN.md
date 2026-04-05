# Ollama Design System

## Philosophy

Radical minimalism — strip away everything unnecessary until only the essential tool remains. Pure-white canvas, exclusively grayscale palette. The interface communicates that this tool "gets out of your way."

## Color Palette

| Token            | Hex       | Usage                          |
|------------------|-----------|--------------------------------|
| Pure Black       | #000000   | Primary text, CTA backgrounds  |
| Near Black       | #262626   | Secondary text                 |
| Darkest Surface  | #090909   | Dark surface variant           |
| Mid Gray         | #525252   | Tertiary text                  |
| Stone            | #737373   | Secondary/muted text           |
| Silver           | #a3a3a3   | Placeholder text               |
| Button Text Dark | #404040   | Button text (secondary)        |
| Border Light     | #d4d4d4   | Borders (secondary buttons)    |
| Light Gray       | #e5e5e5   | Borders, button backgrounds    |
| Snow             | #fafafa   | Alternate backgrounds          |
| Pure White       | #ffffff   | Primary background             |
| Ring Blue        | #3b82f6   | Focus ring (accessibility)     |

## Typography

| Role            | Font              | Size         | Weight | Line-Height |
|-----------------|-------------------|--------------|--------|-------------|
| Display         | SF Pro Rounded    | 48px (3rem)  | 500    | 1.00        |
| Section Heading | SF Pro Rounded    | 36px (2.25rem) | 500  | 1.11        |
| Body            | ui-sans-serif     | 16px (1rem)  | 400    | 1.50        |
| Link            | ui-sans-serif     | 16px (1rem)  | 500    | 1.50        |
| Code            | ui-monospace      | 16px (1rem)  | 400    | 1.50        |

Only two weights: 400 (regular) and 500 (medium).

## Spacing

4px, 6px, 8px, 9px, 10px, 12px, 14px, 16px, 20px, 24px, 32px, 40px, 48px, 88px, 112px

Generous vertical spacing (88-112px) between sections. Low content density.

## Border Radius

- Containers (cards, code blocks): 12px
- Interactive elements (buttons, inputs, tabs, tags): 9999px (pill)

## Shadows

Zero shadows. Depth comes exclusively from background color shifts and borders.

## Breakpoints

- Mobile: <640px
- Small Tablet: 640-768px
- Tablet: 768-850px
- Desktop: 850-1024px
- Large Desktop: 1024-1280px

## Components

### Buttons

**Gray Pill (Primary)**: bg #e5e5e5, text #262626, border 1px solid #e5e5e5, padding 10px 24px, radius 9999px

**White Pill (Secondary)**: bg #ffffff, text #404040, border 1px solid #d4d4d4, padding 10px 24px, radius 9999px

**Black Pill (CTA)**: bg #000000, text #ffffff, padding 10px 24px, radius 9999px

### Cards

bg #ffffff or #fafafa, border 1px solid #e5e5e5, radius 12px, no shadow, padding 24-32px

### Navigation

Transparent bg, black logo, links #000000 16px weight 400, pill-shaped search, black pill CTA

### Hero

bg #ffffff, headline 48px SF Pro Rounded weight 500, line-height 1.0, centered llama illustration

### Code Blocks

bg #ffffff, border 1px solid #e5e5e5, radius 12px, font ui-monospace 16px weight 400

### Inputs

bg #ffffff, border 1px solid #e5e5e5, radius 9999px, focus ring #3b82f6, placeholder #a3a3a3

### Tags

bg #e5e5e5, text #262626, radius 9999px, font 12px
