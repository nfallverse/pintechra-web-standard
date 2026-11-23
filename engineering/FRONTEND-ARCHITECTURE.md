# Frontend Architecture Guidelines

## 1. Purpose

This document defines frontend architecture standards for PINTECHRA web projects.

The objective is to establish frontend systems that are organized, maintainable, scalable, reusable, and easy to understand.

Architecture decisions must match the project's actual complexity and requirements.

## 2. Core Principles

All frontend architecture should follow these principles:

- Separation of concerns.
- Reusable components.
- Clear data flow.
- Maintainable structure.
- Consistent conventions.
- Minimal unnecessary complexity.
- Scalability when justified.
- Performance and accessibility by design.

Do not introduce architectural complexity without a clear reason.

## 3. Architecture Planning

Before implementation, identify:

- Project type.
- Selected framework or technology.
- Main pages and routes.
- Shared components.
- Data sources.
- API requirements.
- State management requirements.
- Authentication requirements, if applicable.
- Build and deployment environment.

Choose an architecture based on these requirements.

Do not select a framework or library simply because it is popular.

## 4. Project Structure

Use a structure that separates responsibilities.

A general example:

```text
src/
├── assets/
├── components/
├── layouts/
├── pages/
├── services/
├── hooks/
├── utils/
├── styles/
├── types/
└── main.js
```

This is a reference structure, not a mandatory structure for every project.

Adapt it to the framework and project complexity.

### Directory Responsibilities

**assets/**
- Images.
- Icons.
- Fonts.
- Static visual resources.

**components/**
- Reusable interface components.
- Buttons.
- Cards.
- Navigation elements.
- Form elements.

**layouts/**
- Shared page structures.
- Header and footer arrangements.
- Application shells.

**pages/**
- Page-level components.
- Route-specific content.

**services/**
- API communication.
- External service integrations.
- Data access logic.

**hooks/**
- Reusable stateful logic.
- Custom React hooks when using React.

**utils/**
- General helper functions.
- Formatting and validation utilities.

**styles/**
- Global styles.
- Design tokens.
- Shared styling resources.

**types/**
- Shared type definitions when using TypeScript.

Only create directories that are actually needed.

## 5. Component Architecture

Components should have clear responsibilities.

### Component Guidelines

- Keep components focused.
- Prefer composition over unnecessary complexity.
- Reuse components when appropriate.
- Keep presentation and business logic reasonably separated.
- Avoid excessively large components.
- Avoid deeply nested component structures.
- Use clear and consistent props.

### Component Categories

**Basic Components**
- Button.
- Input.
- Badge.
- Icon.
- Label.

**Composite Components**
- Product card.
- Navigation menu.
- Search form.
- Feature section.

**Layout Components**
- Header.
- Footer.
- Sidebar.
- Page container.

**Page Components**
- Home page.
- Product detail page.
- About page.
- Contact page.

Do not create abstractions for components that are unlikely to be reused unless separation improves clarity.

## 6. Data Flow

Data flow must be predictable and understandable.

- Define where data originates.
- Keep data ownership clear.
- Pass data through explicit interfaces.
- Avoid unnecessary prop drilling.
- Avoid unnecessary global state.
- Separate API communication from presentation when appropriate.

Use the simplest suitable data flow for the project.

## 7. State Management

Choose state management based on actual requirements.

### Local State

Use local component state for:
- Dropdown visibility.
- Modal visibility.
- Form input.
- Tabs.
- Simple interactions.

### Shared State

Use shared state when multiple components genuinely need the same data.

### Server State

Handle remotely fetched data separately from local interface state when appropriate.

Avoid introducing global state management libraries for small projects.

## 8. Routing

Routing must be organized and predictable.

- Use clear and meaningful route paths.
- Keep route definitions organized.
- Handle unknown routes.
- Provide appropriate loading and error states.
- Protect restricted routes when authentication is required.
- Keep navigation consistent.

Use the routing solution appropriate to the selected framework.

## 9. API and Data Integration

Keep external data communication organized.

- Centralize API configuration when appropriate.
- Separate request logic from UI components.
- Handle loading states.
- Handle failed requests.
- Validate received data.
- Avoid exposing secret credentials.
- Use environment variables for sensitive configuration.

Never assume external API responses are always valid.

## 10. Styling Architecture

Maintain consistent styling across the application.

- Use shared design tokens.
- Keep global and component styles organized.
- Avoid conflicting style systems.
- Follow the project's established styling approach.
- Avoid excessive inline styles.
- Support responsive layouts.
- Maintain accessible contrast and focus states.

Visual consistency must be supported by the architecture.

## 11. Environment Configuration

Separate environment-specific configuration.

Examples:

- Development.
- Testing.
- Production.

Requirements:

- Do not hardcode secrets.
- Document required environment variables.
- Provide safe example configuration files.
- Keep environment-specific behavior explicit.

Never commit real credentials or private keys.

## 12. Scalability and Maintainability

Architecture should support reasonable future growth.

- Group related functionality.
- Keep dependencies between modules understandable.
- Avoid circular dependencies.
- Avoid unnecessary abstractions.
- Refactor when complexity increases.
- Document important architectural decisions.

Do not overengineer a small website for hypothetical future requirements.

## 13. Framework-Specific Adaptation

These guidelines are framework-independent.

When using a specific framework:

- Follow its official conventions.
- Use its recommended project structure where appropriate.
- Respect its rendering and data-fetching model.
- Avoid mixing incompatible architectural patterns.
- Document important framework-specific decisions.

Examples include React, Next.js, Vue, Nuxt, Svelte, and other suitable technologies.

## 14. AI Architecture Requirements

AI coding agents must:

1. Inspect the existing project before making architectural changes.
2. Identify the framework and current conventions.
3. Understand existing dependencies.
4. Propose architecture appropriate to project size.
5. Explain significant structural decisions.
6. Preserve existing functionality.
7. Avoid unnecessary migrations.
8. Update documentation when architecture changes.
9. Verify imports, routes, and component relationships.
10. Never invent files or dependencies.

Do not restructure an entire project without a clear reason.

## 15. Architecture Quality Checklist

- [ ] Project structure is understandable.
- [ ] Responsibilities are separated.
- [ ] Components have clear purposes.
- [ ] Data flow is predictable.
- [ ] State management is appropriate.
- [ ] Routing is organized.
- [ ] API logic is maintainable.
- [ ] Environment configuration is secure.
- [ ] No unnecessary dependencies exist.
- [ ] Architecture matches project complexity.

## 16. Final Principle

Good frontend architecture makes a project easier to understand, maintain, test, and improve.

Choose clarity over complexity and use architecture as a tool to solve real problems.
