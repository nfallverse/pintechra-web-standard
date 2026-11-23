# Color System Guidelines

## 1. Purpose

This document defines a structured color system for PINTECHRA web projects.

Colors must support brand identity, readability, usability, hierarchy, and accessibility.

## 2. Core Principles

- Every color must have a defined purpose.
- Use a limited and consistent palette.
- Prioritize readability and contrast.
- Avoid arbitrary color combinations.
- Maintain consistency across components.
- Select colors based on the project's identity and audience.

## 3. Color Categories

### 3.1 Primary

The primary color represents the main visual identity of a project.

Common use cases:
- Primary actions.
- Brand elements.
- Important interface highlights.

### 3.2 Secondary

Secondary colors support the primary palette.

Use them for:
- Supporting interface elements.
- Secondary actions.
- Visual variation.

### 3.3 Accent

Accent colors create emphasis.

Use them selectively for:
- Important information.
- Selected states.
- Small visual highlights.

### 3.4 Surface

Surface colors define interface backgrounds.

Examples:
- Main background.
- Elevated surfaces.
- Input backgrounds.
- Inset surfaces.
- Navigation backgrounds.

### 3.5 Text

Define text colors according to hierarchy:

- Primary text.
- Secondary text.
- Muted text.
- Inverse text.
- Disabled text.

### 3.6 Border

Border colors define separation and component boundaries.

Use them only when they improve structure or clarity.

## 4. Semantic Colors

Semantic colors communicate interface states.

| Token | Meaning |
|---|---|
| Success | Successful actions |
| Warning | Caution or pending states |
| Error | Failed actions or critical issues |
| Info | Neutral informational messages |

Do not rely on color alone to communicate meaning.

## 5. Color Tokens

Use semantic design tokens instead of hardcoding unrelated colors throughout the interface.

Example:

```css
:root {
  --color-primary: #173B57;
  --color-secondary: #52738A;
  --color-accent: #D6A85F;

  --color-background: #F3F5F7;
  --color-surface: #FFFFFF;

  --color-text-primary: #17212B;
  --color-text-secondary: #5C6873;

  --color-border: #DCE2E8;

  --color-success: #23865A;
  --color-warning: #B7791F;
  --color-error: #C0392B;
  --color-info: #2876B8;
}
```

These values are illustrative examples, not mandatory brand colors.

## 6. Neumorphic Color Considerations

For Neumorphic interfaces:

- Keep surface colors consistent within a component group.
- Derive shadows from the surface and lighting context.
- Avoid shadows that make controls difficult to identify.
- Maintain sufficient text contrast.
- Use borders when shadows alone are insufficient.

## 7. Light and Dark Themes

Projects may support light mode, dark mode, or both.

Each theme must define its own:
- Background.
- Surface.
- Text.
- Border.
- Interactive states.
- Semantic colors.

Do not simply invert all colors to create a dark theme.

## 8. Accessibility

- Maintain WCAG contrast requirements.
- Aim for at least 4.5:1 contrast for normal text.
- Aim for at least 3:1 for large text.
- Ensure interactive components remain distinguishable.
- Provide additional labels or icons for semantic states.
- Test colors in different display conditions.

## 9. Quality Checklist

Before approving a color palette:

- Does it fit the project identity?
- Is the palette consistent?
- Is text readable?
- Are primary actions identifiable?
- Are semantic colors distinguishable?
- Does the dark theme work independently?
- Does the palette remain accessible?
- Are color tokens used consistently?

## 10. Final Principle

A strong color system is not about using many colors.

It is about assigning the right color to the right purpose.
```
