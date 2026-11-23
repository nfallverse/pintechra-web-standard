# Responsive Design Guidelines

## 1. Purpose

This document defines responsive design standards for PINTECHRA web projects.

The objective is to ensure that every website remains usable, readable, accessible, and visually consistent across different screen sizes and devices.

Responsive design must be considered from the beginning of the design process.

## 2. Core Principles

- Mobile-friendly by default.
- Content-first layout decisions.
- Consistent visual hierarchy.
- Flexible and adaptive components.
- Readable typography.
- Touch-friendly interactions.
- No unnecessary horizontal scrolling.
- Consistent functionality across devices.

Responsive design is not simply shrinking a desktop layout.

## 3. Device Categories

Consider the following general viewport ranges:

| Device | Width |
|---|---:|
| Small Mobile | 320–374px |
| Mobile | 375–767px |
| Tablet | 768–1023px |
| Laptop | 1024–1439px |
| Desktop | 1440px and above |

These ranges are starting references, not strict rules.

Choose breakpoints based on when the content or layout needs to change.

## 4. Mobile-First Approach

Start with a layout that works well on small screens.

Then progressively enhance the layout for larger screens.

Mobile layouts should prioritize:

- Essential content.
- Clear navigation.
- Readable text.
- Simple interactions.
- Appropriate spacing.
- Fast loading.
- Touch accessibility.

Do not force desktop layouts into mobile screens.

## 5. Responsive Layout

Layouts must adapt naturally to available space.

### Containers

- Use flexible container widths.
- Apply reasonable maximum widths.
- Maintain consistent horizontal padding.
- Prevent content from touching screen edges.
- Avoid unnecessarily wide text blocks.

### Grid Systems

- Use fewer columns on smaller screens.
- Increase columns when screen space allows.
- Allow cards and content sections to reflow.
- Avoid fixed widths that break smaller layouts.

### Navigation

- Simplify navigation on mobile when necessary.
- Use accessible menu controls.
- Keep navigation behavior consistent.
- Ensure important actions remain easy to reach.

## 6. Typography Responsiveness

Typography must remain readable across devices.

- Use fluid typography when appropriate.
- Adjust heading sizes for smaller screens.
- Maintain comfortable line heights.
- Prevent text overflow.
- Avoid excessively small body text.
- Keep line lengths readable on large screens.

Use CSS `clamp()` when it provides a suitable fluid scale.

Example:

```css
.page-title {
  font-size: clamp(2rem, 5vw, 4rem);
}
```

## 7. Images and Media

Images and media must adapt to their containers.

- Use responsive image dimensions.
- Preserve aspect ratios.
- Prevent unwanted image distortion.
- Use appropriate cropping.
- Optimize image file sizes.
- Avoid oversized media on mobile.
- Provide meaningful alternative text for informative images.

Use modern image formats when supported and beneficial.

## 8. Responsive Components

Every interactive component must work across screen sizes.

Consider:

- Buttons.
- Forms.
- Cards.
- Navigation menus.
- Dialogs.
- Tables.
- Dropdowns.
- Tabs.
- Sidebars.

Avoid controls that become too small or difficult to use on touch devices.

## 9. Touch and Pointer Interaction

Support both touch and pointer-based interaction.

- Provide comfortable touch targets.
- Do not depend exclusively on hover.
- Make interactive states visible.
- Avoid tightly packed controls.
- Ensure keyboard interaction remains supported.

Use approximately 44 × 44 CSS pixels as a practical touch-target guideline where possible.

## 10. Responsive Spacing

Spacing should adapt to screen size.

- Reduce excessive padding on mobile.
- Maintain sufficient whitespace.
- Preserve visual hierarchy.
- Keep related elements visually connected.
- Avoid cramped layouts.

Use consistent spacing tokens rather than arbitrary values.

## 11. Horizontal Overflow

Prevent unintended horizontal scrolling.

Check for:
- Fixed-width elements.
- Oversized images.
- Long unbroken text.
- Wide tables.
- Navigation overflow.
- Incorrect positioning.
- Large decorative elements.

Some content, such as data tables, may require controlled horizontal scrolling.

## 12. Responsive Performance

Consider device limitations.

- Optimize images.
- Avoid unnecessary animations.
- Reduce expensive visual effects on weaker devices.
- Avoid loading unnecessary resources.
- Keep interactions responsive.
- Test on realistic mobile conditions.

Responsive design must consider performance as well as appearance.

## 13. Testing Requirements

Test important layouts at multiple viewport sizes.

At minimum, check:

- 320px.
- 375px.
- 768px.
- 1024px.
- 1366px.
- 1440px.

Also test intermediate widths where layout transitions occur.

Check both portrait and landscape orientations when relevant.

## 14. AI Responsive Implementation Requirements

AI coding agents must:

1. Inspect existing responsive behavior.
2. Identify the layout's critical breakpoints.
3. Preserve the intended visual hierarchy.
4. Avoid arbitrary breakpoint additions.
5. Test navigation and interactive components.
6. Check for horizontal overflow.
7. Verify typography and spacing.
8. Avoid hiding important content simply to fit smaller screens.
9. Explain significant responsive layout decisions.
10. Never claim device testing was performed when it was not.

## 15. Responsive Quality Checklist

- [ ] Layout works on small mobile screens.
- [ ] Content adapts to tablet screens.
- [ ] Desktop layout uses available space effectively.
- [ ] Navigation remains usable.
- [ ] Typography remains readable.
- [ ] Images preserve their intended appearance.
- [ ] Interactive elements are touch-friendly.
- [ ] No unintended horizontal overflow exists.
- [ ] Important content remains accessible.
- [ ] Performance is acceptable on mobile devices.

## 16. Final Principle

A responsive website should feel intentionally designed for every screen size.

Do not treat mobile as a reduced version of desktop.

Adapt the experience to the device while preserving the project's identity and usability.
