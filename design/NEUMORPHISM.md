# Neumorphism Design Guidelines

## 1. Purpose

This document defines how Neumorphism should be applied across PINTECHRA web projects.

Neumorphism is a preferred visual language, not a mandatory design system.

Its purpose is to create subtle depth and tactile interaction without compromising usability.

## 2. Core Concepts

### 2.1 Surface

The surface is the background from which interface elements appear to emerge.

Raised and inset elements should generally relate to the same surface color.

### 2.2 Light Source

Use a consistent light direction across related components.

Do not mix random shadow directions within the same interface.

### 2.3 Raised Elements

Raised elements appear to sit above the surface.

Use them selectively for:
- Primary interactive controls.
- Selected interface elements.
- Important visual components.

### 2.4 Inset Elements

Inset elements appear pressed into the surface.

Use them selectively for:
- Input fields.
- Display areas.
- Selected control states.

## 3. Shadow System

A typical raised component may use two complementary shadows:

- A light shadow on the upper-left side.
- A dark shadow on the lower-right side.

Example:

```css
.neumorphic-raised {
  box-shadow:
    -6px -6px 12px rgba(255, 255, 255, 0.8),
    6px 6px 12px rgba(0, 0, 0, 0.12);
}
```

An inset component may use the reverse visual relationship:

```css
.neumorphic-inset {
  box-shadow:
    inset 4px 4px 8px rgba(0, 0, 0, 0.10),
    inset -4px -4px 8px rgba(255, 255, 255, 0.8);
}
```

These values are examples, not universal constants.

Always adapt shadow intensity to the background, component size, and visual context.

## 4. Surface and Color

- Use related surface and shadow colors.
- Avoid excessive contrast between neighboring surfaces.
- Maintain readable foreground text.
- Do not rely on shadows alone to communicate meaning.
- Dark interfaces require independently tuned shadow values.

## 5. Interaction States

Interactive components must have distinguishable states:

### Default
The component appears in its normal state.

### Hover
Use a subtle visual response where appropriate.

### Active
A pressed or inset appearance may communicate interaction.

### Focus
Provide a clearly visible keyboard focus indicator.

### Disabled
Make disabled states understandable without relying only on reduced opacity.

## 6. Accessibility

Neumorphism can reduce visible boundaries between components.

Therefore:

- Maintain sufficient text contrast.
- Use explicit labels for form controls.
- Provide visible focus indicators.
- Preserve clear component boundaries.
- Do not communicate state through shadows alone.
- Ensure interactive areas are large enough.

## 7. Responsive Behavior

Neumorphic effects must remain appropriate across screen sizes.

Avoid:
- Excessive shadows on small screens.
- Large blur radii that reduce clarity.
- Unnecessary decorative depth.
- Effects that reduce performance.

## 8. When Not to Use Neumorphism

Do not force Neumorphism onto:

- Dense data tables.
- Complex dashboards.
- Long-form reading content.
- Interfaces requiring strong visual separation.
- Components where conventional borders improve clarity.

Use conventional UI patterns when they provide a better user experience.

## 9. Quality Checklist

Before approving a Neumorphic component, verify:

- Is the surface clearly identifiable?
- Is the light direction consistent?
- Are shadows subtle and intentional?
- Is the component still recognizable?
- Is text readable?
- Are interaction states distinguishable?
- Does keyboard focus remain visible?
- Does the component work on mobile?

## 10. Final Principle

Neumorphism should enhance the interface, not become the interface.

Depth is a design tool, not a substitute for hierarchy, usability, or accessibility.
