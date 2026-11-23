# Layout and Grid Guidelines

## 1. Purpose

This document establishes layout, grid, spacing, and composition standards for PINTECHRA web projects.

The objective is to create structured, balanced, responsive, and visually coherent interfaces.

## 2. Core Principles

- Establish layout before detailed styling.
- Use consistent alignment.
- Maintain deliberate spacing.
- Create clear visual hierarchy.
- Prioritize content structure.
- Use whitespace intentionally.
- Avoid unnecessary layout complexity.

## 3. Container System

Containers define the maximum width of content.

Suggested maximum widths:

| Container | Width |
|---|---:|
| Small | 640px |
| Medium | 768px |
| Large | 1024px |
| Extra Large | 1280px |
| Wide | 1440px |

These are reference values, not mandatory dimensions.

Use responsive side padding to prevent content from touching screen edges.

## 4. Grid System

A grid helps organize content and maintain consistent alignment.

Suggested grid structures:

- Mobile: 4 columns.
- Tablet: 8 columns.
- Desktop: 12 columns.

Use CSS Grid or Flexbox according to the layout requirements.

Example:

```css
.container {
  width: min(100% - 2rem, 1280px);
  margin-inline: auto;
}

.grid {
  display: grid;
  grid-template-columns: repeat(12, minmax(0, 1fr));
  gap: 1.5rem;
}
```

## 5. Spacing System

Use a consistent spacing scale.

Suggested base scale:

| Token | Value |
|---|---:|
| 1 | 4px |
| 2 | 8px |
| 3 | 12px |
| 4 | 16px |
| 5 | 20px |
| 6 | 24px |
| 8 | 32px |
| 10 | 40px |
| 12 | 48px |
| 16 | 64px |
| 20 | 80px |
| 24 | 96px |

Do not use spacing values randomly.

## 6. Section Composition

Each section must have a clear purpose.

Consider:
- Content priority.
- Visual hierarchy.
- Alignment.
- Section spacing.
- Relationship between elements.
- Reading direction.

Avoid making every section use the same layout.

Variation should come from the content and design concept, not arbitrary decoration.

## 7. Whitespace

Whitespace is an important design element.

Use it to:
- Separate content groups.
- Improve readability.
- Establish hierarchy.
- Reduce visual noise.
- Create visual rhythm.

Do not fill every available space.

## 8. Responsive Layout

Layouts must adapt to the available viewport.

Suggested breakpoints:

| Device | Starting breakpoint |
|---|---:|
| Small mobile | 480px |
| Tablet | 768px |
| Laptop | 1024px |
| Desktop | 1280px |

These are starting references. Choose breakpoints based on when the layout actually needs to change.

Mobile layouts should be intentionally designed rather than merely compressed desktop layouts.

## 9. Alignment

Maintain consistent alignment across:
- Headings.
- Paragraphs.
- Images.
- Buttons.
- Navigation.
- Content containers.

Use a deliberate alignment system throughout the page.

## 10. Layout Quality Checklist

Before approving a layout:

- Is the content hierarchy clear?
- Are containers appropriately sized?
- Is alignment consistent?
- Is spacing systematic?
- Is whitespace intentional?
- Does the composition feel balanced?
- Does the layout adapt to mobile?
- Is horizontal overflow avoided?
- Are important actions easy to find?

## 11. Final Principle

Good layout is not about placing elements inside a grid.

It is about creating a clear relationship between content, space, and visual hierarchy.
```

## 8.5 Commit perubahan

Isi:

- Commit message: `Add layout and grid guidelines`
- Branch: `main`
- Klik **Commit changes**.

---

## Checklist Langkah 8

<box border radius="lg" padding={3} gap={2}>
  **Layout & Grid**
  - [ ] File `design/LAYOUT-AND-GRID.md` dibuat.
  - [ ] Konten berhasil ditempel.
  - [ ] Contoh CSS tetap rapi.
  - [ ] File berhasil di-commit.
</box>

Setelah selesai, bilang **"Layout & Grid selesai bro"**.

Berikutnya kita membuat `COMPONENTS.md`, yaitu standar pembuatan tombol, input, navbar, card, modal, dan komponen UI lainnya. Ini akan menjadi fondasi agar komponen di seluruh website PINTECHRA konsisten.
