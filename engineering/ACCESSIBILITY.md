# Accessibility Guidelines

## 1. Purpose

This document defines accessibility standards for PINTECHRA web projects.

The objective is to make websites usable by people with different abilities, needs, devices, and interaction methods.

Accessibility must be considered throughout design, development, and testing.

## 2. Core Principles

Follow the four core principles of WCAG:

### Perceivable
Users must be able to perceive the information presented.

### Operable
Users must be able to operate the interface.

### Understandable
Content and interactions must be clear and predictable.

### Robust
Content must work with different browsers, assistive technologies, and devices.

Aim for WCAG 2.2 Level AA where applicable.

## 3. Semantic HTML

Use HTML elements according to their intended meaning.

- Use headings in a logical hierarchy.
- Use `<button>` for actions.
- Use `<a>` for navigation.
- Use `<nav>` for navigation sections.
- Use `<main>` for primary content.
- Use `<header>` and `<footer>` appropriately.
- Use semantic form elements.
- Avoid using generic elements when semantic alternatives exist.

Do not use HTML elements only because of their default appearance.

## 4. Keyboard Accessibility

All essential functionality must be accessible through a keyboard.

Requirements:

- Interactive elements must be keyboard accessible.
- Maintain a logical tab order.
- Provide visible focus indicators.
- Avoid keyboard traps.
- Support Enter and Space where appropriate.
- Ensure dialogs and menus handle keyboard interaction correctly.
- Provide a way to skip repetitive navigation when appropriate.

Do not require mouse interaction for essential functionality.

## 5. Color and Contrast

Color must not be the only way to communicate information.

Requirements:

- Maintain sufficient text contrast.
- Use additional visual indicators for status and errors.
- Avoid relying only on color differences.
- Ensure important interface elements remain distinguishable.

Recommended WCAG contrast ratios:

| Element | Minimum Contrast |
|---|---:|
| Normal text | 4.5:1 |
| Large text | 3:1 |
| UI components and graphical objects | 3:1 |

Test contrast across light and dark themes when both are supported.

## 6. Typography and Readability

Text must remain comfortable to read.

- Use readable font sizes.
- Maintain sufficient line height.
- Avoid overly long paragraphs.
- Use clear headings.
- Provide meaningful link text.
- Avoid unnecessary uppercase text.
- Support browser text resizing.
- Do not communicate essential information through visual styling alone.

## 7. Images and Alternative Text

Provide appropriate alternative text for informative images.

Requirements:

- Describe the purpose or relevant information of an image.
- Use empty alternative text for purely decorative images.
- Avoid redundant descriptions.
- Do not place essential information only inside images without an accessible alternative.
- Provide captions or transcripts for relevant media.

Alternative text must describe the image's function in context.

## 8. Forms and Input Fields

Forms must be understandable and accessible.

- Provide visible labels.
- Associate labels with their inputs.
- Explain required fields.
- Provide clear validation messages.
- Identify errors in text, not only through color.
- Preserve user input when validation fails.
- Provide instructions when input formats are required.
- Ensure controls are keyboard accessible.

Placeholder text must not replace a proper label.

## 9. Navigation and Interaction

Navigation must be predictable.

- Use descriptive link text.
- Maintain consistent navigation patterns.
- Provide clear active states.
- Ensure menus can be operated with a keyboard.
- Avoid unexpected context changes.
- Make interactive controls visually identifiable.
- Provide clear feedback after important actions.

## 10. Motion and Animation

Motion must not create accessibility barriers.

- Respect the `prefers-reduced-motion` setting.
- Avoid unnecessary continuous animations.
- Avoid flashing content that may trigger seizures.
- Do not use motion as the only way to communicate information.
- Allow users to pause or stop relevant moving content.
- Keep transitions purposeful and restrained.

## 11. Responsive Accessibility

Accessibility must remain consistent across screen sizes.

- Support browser zoom.
- Avoid clipped text.
- Maintain readable contrast.
- Preserve keyboard functionality.
- Keep touch targets usable.
- Ensure content reflows appropriately.
- Avoid hiding essential information on mobile.

## 12. Screen Reader Support

Use semantic structure and accessible names.

- Provide accessible names for controls.
- Use appropriate ARIA attributes when necessary.
- Announce important dynamic updates when appropriate.
- Maintain meaningful heading structure.
- Identify page language.
- Avoid unnecessary ARIA attributes.

Prefer native HTML semantics over custom ARIA implementations.

## 13. Dialogs and Dynamic Content

Interactive overlays and dynamic content must remain accessible.

For dialogs:

- Provide an accessible title.
- Manage keyboard focus.
- Prevent interaction with background content when modal behavior is intended.
- Support Escape when appropriate.
- Return focus to the triggering element when closed.

For dynamic updates:

- Communicate important status changes.
- Avoid unexpected focus movement.
- Provide understandable loading and error feedback.

## 14. Accessibility Testing

Use a combination of automated and manual testing.

Recommended checks:

- Keyboard-only navigation.
- Visible focus indicators.
- Browser zoom and text resizing.
- Color contrast evaluation.
- Screen reader testing.
- Form validation behavior.
- Reduced-motion behavior.
- Responsive layout inspection.

Automated accessibility tools are useful but cannot identify every accessibility issue.

## 15. AI Accessibility Requirements

AI coding agents must:

1. Use semantic HTML whenever possible.
2. Include accessible labels for controls.
3. Provide appropriate image alternative text.
4. Maintain keyboard accessibility.
5. Preserve visible focus indicators.
6. Check text and UI contrast.
7. Respect reduced-motion preferences.
8. Avoid unnecessary ARIA attributes.
9. Identify accessibility limitations.
10. Never claim full accessibility compliance without adequate testing.

## 16. Accessibility Quality Checklist

- [ ] Semantic HTML is used appropriately.
- [ ] Essential functionality works with a keyboard.
- [ ] Focus indicators are visible.
- [ ] Text contrast meets applicable requirements.
- [ ] Color is not the only information indicator.
- [ ] Images have appropriate alternative text.
- [ ] Forms have accessible labels and errors.
- [ ] Navigation is understandable.
- [ ] Motion preferences are respected.
- [ ] Dynamic content is communicated appropriately.
- [ ] Screen reader behavior has been considered.
- [ ] Accessibility testing has been performed where possible.

## 17. Final Principle

Accessibility is not an optional visual enhancement.

It is a fundamental part of building inclusive, usable, and reliable digital experiences.
