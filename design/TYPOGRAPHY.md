# Typography Guidelines

## 1. Purpose

This document establishes typography standards for PINTECHRA web projects.

Typography must support readability, visual hierarchy, brand identity, and usability.

## 2. Core Principles

- Readability comes first.
- Typography must support the design concept.
- Use a deliberate type hierarchy.
- Avoid unnecessary font variations.
- Maintain consistency across the interface.
- Choose fonts based on project identity and audience.

## 3. Font Selection

### 3.1 Primary Typeface

The primary typeface is used for most interface content.

Preferred characteristics:
- High readability.
- Clear letterforms.
- Good language support.
- Multiple font weights.
- Suitable for digital interfaces.

Examples:
- Inter.
- Manrope.
- IBM Plex Sans.
- Plus Jakarta Sans.

### 3.2 Secondary Typeface

A secondary typeface may be used to establish a distinct visual character.

Possible use cases:
- Editorial headlines.
- Brand statements.
- Display typography.
- Selected promotional sections.

Examples:
- Instrument Serif.
- Playfair Display.
- DM Serif Display.

Use a secondary typeface only when it strengthens the design concept.

### 3.3 Monospace Typeface

Monospace fonts may be used for:
- Technical information.
- Product specifications.
- Measurements.
- Code snippets.
- System labels.

Examples:
- JetBrains Mono.
- IBM Plex Mono.

## 4. Type Hierarchy

Use a consistent hierarchy.

| Element | Suggested Size | Weight |
|---|---:|---|
| Display | 56–72px | 600–700 |
| H1 | 40–48px | 600–700 |
| H2 | 32–40px | 600 |
| H3 | 24–28px | 500–600 |
| H4 | 20–22px | 500–600 |
| Body Large | 18px | 400 |
| Body | 16px | 400 |
| Small | 14px | 400–500 |
| Caption | 12px | 400–500 |

These values are starting points and should adapt to the project.

## 5. Font Weight

Use font weights intentionally:

- 400: Regular body text.
- 500: Medium emphasis.
- 600: Section headings and important labels.
- 700: Strong headlines and selected emphasis.

Avoid using too many weights within one interface.

## 6. Line Height

Recommended starting values:

- Large headings: 1.05–1.2.
- Body text: 1.5–1.7.
- Small text: 1.4–1.5.

Long-form reading should prioritize comfortable line spacing.

## 7. Letter Spacing

- Large headings may use slightly tighter spacing.
- Body text should remain naturally spaced.
- Uppercase labels may use wider spacing.
- Avoid excessive tracking that reduces readability.

## 8. Responsive Typography

Typography must adapt to screen sizes.

Use fluid sizing where appropriate.

Example:

```css
h1 {
  font-size: clamp(2.25rem, 5vw, 4.5rem);
  line-height: 1.1;
}
```

Avoid headings that overflow or become difficult to read on small screens.

## 9. Content Width

Long-form text should use a comfortable reading width.

Avoid excessively long text lines.

Use appropriate content containers and paragraph spacing.

## 10. Accessibility

- Use semantic heading levels.
- Do not skip heading levels without reason.
- Maintain sufficient text contrast.
- Avoid excessively small text.
- Do not communicate meaning through font weight alone.
- Support browser zoom and text resizing.

## 11. Quality Checklist

Before approving typography:

- Is the font appropriate for the brand?
- Is the hierarchy clear?
- Are headings distinguishable?
- Is body text comfortable to read?
- Is line spacing appropriate?
- Does typography adapt to mobile?
- Are font weights used consistently?
- Does the design remain readable at different zoom levels?

## 12. Final Principle

Typography is not decoration.

It is a fundamental part of communication, hierarchy, and visual identity.
