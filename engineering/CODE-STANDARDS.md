# Code Standards

## 1. Purpose

This document defines coding standards for all web development projects under PINTECHRA.

The objective is to maintain code that is readable, maintainable, consistent, scalable, and reliable.

These standards apply to all supported web technologies and programming languages.

## 2. General Principles

All code must follow these principles:

- Readability over unnecessary cleverness.
- Simplicity over unnecessary complexity.
- Consistency across the project.
- Reusability without overengineering.
- Clear separation of responsibilities.
- Maintainability for future development.
- Security and reliability by default.

Write code for both developers and future maintainers.

## 3. Naming Conventions

Use descriptive and meaningful names.

### Variables and Functions

- Use `camelCase` for JavaScript variables and functions.
- Use descriptive names that explain their purpose.
- Avoid unclear abbreviations.
- Use verbs for function names.

Examples:

```js
const productName = "IoT Digital Clock";

function calculateTotalPrice() {
  // Implementation
}
```

### Components and Classes

- Use `PascalCase` for component names and class names.
- Component names should describe their responsibility.

Example:

```jsx
function ProductCard() {
  return null;
}
```

### Constants

- Use `UPPER_SNAKE_CASE` for global constants when appropriate.

Example:

```js
const API_BASE_URL = "/api";
```

### Files and Directories

- Use consistent naming conventions throughout the project.
- Prefer lowercase kebab-case for general filenames.
- Follow the naming conventions required by the selected framework.

## 4. Code Formatting

- Use consistent indentation.
- Avoid unnecessarily long lines.
- Use meaningful whitespace.
- Group related code logically.
- Remove unused imports and variables.
- Avoid deeply nested structures when possible.
- Use formatting tools such as Prettier when appropriate.

Formatting should remain consistent across the entire project.

## 5. Code Organization

Organize code based on responsibility.

Separate:
- UI components.
- Business logic.
- Data and API access.
- Utilities and helper functions.
- Configuration.
- Assets and styles.

Avoid placing unrelated functionality in a single file.

Use a project structure appropriate to the selected framework and project complexity.

## 6. Functions and Logic

- Keep functions focused on one responsibility.
- Avoid unnecessarily large functions.
- Use parameters and return values clearly.
- Avoid duplicated logic.
- Extract reusable logic when it improves maintainability.
- Handle errors explicitly.
- Avoid unnecessary side effects.

Do not create abstractions without a clear benefit.

## 7. Comments and Documentation

Write comments to explain why something is done, not merely repeat what the code already says.

Comments should be:
- Relevant.
- Clear.
- Accurate.
- Updated when implementation changes.

Document complex logic, important decisions, and non-obvious behavior.

Avoid excessive comments.

## 8. HTML and CSS Standards

### HTML

- Use semantic HTML elements.
- Maintain a logical document hierarchy.
- Use accessible labels for form controls.
- Avoid unnecessary wrapper elements.
- Keep markup readable.

### CSS

- Use consistent class naming.
- Prefer reusable design tokens.
- Avoid excessive specificity.
- Avoid unnecessary `!important`.
- Organize styles logically.
- Keep responsive styles maintainable.

Use the project's established styling approach consistently.

## 9. JavaScript Standards

- Prefer `const` by default.
- Use `let` when reassignment is necessary.
- Avoid `var` in modern JavaScript projects.
- Use strict equality (`===`) where appropriate.
- Handle asynchronous operations carefully.
- Avoid unnecessary global variables.
- Validate external data.
- Handle loading, success, and error states.

Use modern JavaScript features when supported by the project environment.

## 10. Error Handling

- Never silently ignore important errors.
- Provide meaningful error messages.
- Validate user input.
- Handle failed network requests.
- Avoid exposing sensitive technical details to end users.
- Log useful debugging information during development.

Error handling must be appropriate to the project's environment.

## 11. Security

- Never expose API keys, passwords, or secrets in public repositories.
- Use environment variables for sensitive configuration.
- Validate and sanitize untrusted input.
- Avoid unsafe HTML injection.
- Follow secure authentication and authorization practices.
- Keep dependencies updated.
- Apply the principle of least privilege.

Security must be considered from the beginning, not added as an afterthought.

## 12. Dependencies

- Use dependencies only when they provide clear value.
- Avoid unnecessary packages.
- Prefer maintained and reputable libraries.
- Check compatibility before installation.
- Keep dependency versions under control.
- Remove unused dependencies.

Do not add a library for functionality that can be implemented simply and safely without it.

## 13. Refactoring

Refactor code when it improves:
- Readability.
- Maintainability.
- Performance.
- Reusability.
- Architecture.

Do not change working behavior unnecessarily.

Preserve existing functionality unless a change is explicitly required.

## 14. AI Coding Requirements

AI coding agents must:

1. Understand the existing project before editing.
2. Inspect relevant files and dependencies.
3. Follow the project's existing architecture.
4. Avoid replacing working code without justification.
5. Explain important implementation decisions.
6. Identify potential breaking changes.
7. Check for errors after implementation.
8. Avoid claiming that code was tested when it was not.

Never invent project files, dependencies, or implementation details.

## 15. Final Code Quality Checklist

Before considering implementation complete, verify:

- [ ] Code is readable and consistently formatted.
- [ ] Naming conventions are consistent.
- [ ] No unnecessary duplicated logic exists.
- [ ] No unused imports or variables remain.
- [ ] Errors are handled appropriately.
- [ ] Sensitive information is protected.
- [ ] Existing functionality is preserved.
- [ ] Relevant tests or checks have been performed.
- [ ] Documentation is updated when necessary.

## 16. Final Principle

Good code is not defined by how complicated it looks.

Good code is understandable, reliable, maintainable, secure, and appropriate for its purpose.
