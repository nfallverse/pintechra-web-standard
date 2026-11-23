# Build Process — Product Catalog Website

## 1. Purpose

This document defines the engineering workflow for implementing PINTECHRA product catalog websites.

The goal is to translate approved project requirements and design specifications into a functional, responsive, accessible, secure, and maintainable website.

Follow the root `AGENTS.md` and relevant engineering documentation throughout implementation.

## 2. Development Principles

- Understand before implementing.
- Plan before modifying code.
- Follow the approved design direction.
- Keep code organized and maintainable.
- Prioritize functionality and usability.
- Avoid unnecessary dependencies and complexity.
- Test changes before delivery.
- Never claim unverified functionality works.

## 3. Phase 1 — Project Inspection

Before writing code, inspect the existing project.

Understand:

- Current directory structure
- Existing files and components
- Technology stack
- Dependencies
- Build and development commands
- Existing design system
- Available assets
- Existing functionality
- Hosting and deployment constraints

For existing projects, preserve working functionality unless a change is required.

Do not overwrite or remove important files without understanding their purpose.

## 4. Phase 2 — Implementation Planning

Translate the project brief and design handoff into an implementation plan.

Define:

- Pages and routes
- Component hierarchy
- Data structure
- Product information model
- Required functionality
- Asset requirements
- API or backend requirements
- Responsive behavior
- Testing strategy

Identify dependencies between tasks.

Separate essential features from optional improvements.

## 5. Phase 3 — Project Setup

Prepare the development environment.

Depending on the chosen stack:

- Configure project dependencies.
- Establish the directory structure.
- Configure environment variables.
- Set up development scripts.
- Establish formatting and linting tools.
- Configure version control.
- Prepare required assets.

Do not expose credentials, API keys, or private configuration in public repositories.

## 6. Phase 4 — Design System Implementation

Implement the approved design foundation.

Establish:

- Color tokens
- Typography tokens
- Spacing scale
- Layout containers
- Grid system
- Border and shadow styles
- Responsive breakpoints
- Reusable interaction patterns

Keep design tokens consistent across the website.

Avoid introducing unrelated visual styles during implementation.

## 7. Phase 5 — Component Development

Build reusable components based on project requirements.

Possible components include:

- Header
- Navigation
- Footer
- Product card
- Product grid
- Product gallery
- Product specification table
- Category navigation
- Search and filter controls
- Inquiry buttons
- Contact form

Not every project needs every component.

Keep components focused on clear responsibilities.

Avoid unnecessary abstraction for simple features.

## 8. Phase 6 — Page Implementation

Implement pages according to the approved information architecture.

Typical pages may include:

### Home

- Brand introduction
- Main product highlights
- Catalog entry point
- Supporting information
- Contact action

### Product Catalog

- Product listing
- Product categories
- Search or filtering, if required
- Product summaries
- Product detail links

### Product Details

- Product overview
- Images and gallery
- Features and benefits
- Technical specifications
- Availability or status
- Inquiry action

### About

- Brand background
- Business information
- Relevant supporting content

### Contact

- Contact methods
- Inquiry form, if required
- Relevant business information

Adapt page structure to actual project scope.

## 9. Phase 7 — Product Data Integration

Determine how product information will be managed.

Possible approaches:

- Static data files
- Local JSON
- CMS
- Backend API
- Database

Choose the simplest approach that satisfies current and expected requirements.

Ensure:

- Product information is consistent.
- Data is validated.
- Missing information is handled clearly.
- Images have appropriate alternatives.
- Unverified specifications are not displayed as facts.

Do not introduce a database or backend when static data is sufficient.

## 10. Phase 8 — Feature Implementation

Implement required functionality.

Possible features:

- Product search
- Category filtering
- Product sorting
- Product image gallery
- Product comparison
- Inquiry forms
- WhatsApp contact links
- External purchasing links

Validate user input and handle errors appropriately.

Do not implement optional features without a clear project requirement.

## 11. Phase 9 — Responsive Implementation

Ensure the website adapts to:

- Mobile phones
- Tablets
- Laptops
- Desktop screens

Test:

- Navigation
- Product grids
- Product images
- Typography
- Spacing
- Forms
- Interactive controls
- Content overflow

Use responsive layouts rather than simply scaling down desktop designs.

## 12. Phase 10 — Integration and Refinement

Verify that all components and pages work together.

Review:

- Navigation and routing
- Product data
- Image loading
- Internal links
- External links
- Contact methods
- Interactive states
- Error handling
- Visual consistency

Refine spacing, alignment, typography, and interactions.

## 13. Phase 11 — Testing

Perform appropriate testing before delivery.

Check:

- Main user flows
- Product browsing
- Product detail access
- Search and filtering, if implemented
- Forms and contact actions
- Responsive behavior
- Accessibility
- Performance
- SEO fundamentals
- Security
- Browser compatibility

Use automated tests where appropriate.

Do not claim tests passed unless they were actually executed.

## 14. Phase 12 — Deployment Preparation

Before deployment:

- Verify production build.
- Check environment configuration.
- Confirm asset paths.
- Verify metadata.
- Check routing behavior.
- Remove unintended debug output.
- Review security-sensitive settings.
- Confirm hosting compatibility.

Deployment must follow the project's hosting requirements.

Do not deploy without authorization.

## 15. Phase 13 — Delivery

Provide a clear implementation report containing:

1. Completed pages
2. Implemented features
3. Important technical decisions
4. Project structure overview
5. How to run the project
6. Testing performed and results
7. Known limitations
8. Recommended next improvements

Include relevant commands and configuration instructions.

## 16. AI Engineering Requirements

AI assistants must:

- Inspect the existing codebase before modifying it.
- Identify affected files before implementation.
- Explain significant architectural decisions.
- Preserve unrelated functionality.
- Avoid unnecessary rewrites.
- Follow the documented standards.
- Validate changes with appropriate tests.
- Report errors honestly.
- Never invent test results or deployment status.

For multi-step tasks, implement and verify changes incrementally.

The final implementation must reflect the approved requirements and design direction.
