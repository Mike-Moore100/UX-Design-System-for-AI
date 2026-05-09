# Modules Index

Use this file to understand which Layr modules are active and which modules are planned.

Layr is modular by design.
The user should still only need one prompt.

---

## Active Modules

These modules are part of the current Layr system and must be applied when relevant.

### UX

Status: Active

Primary files:

- `UX.md`
- `methods/ux/`

Use for:

- user intent
- task flow
- interaction quality
- cognitive load
- friction reduction
- trust
- feedback
- time to value

### Design

Status: Active

Primary files:

- `DESIGN.md`
- `methods/design/`

Use for:

- visual hierarchy
- colour
- typography
- spacing
- composition
- components
- motion
- design system consistency

---

## Planned Modules

These modules are planned but not active yet.
Do not treat them as complete Layr systems until their rule files and methods exist.

### Accessibility

Use when active for:

- WCAG checks
- keyboard navigation
- focus management
- semantic structure
- colour contrast
- reduced motion
- screen reader support

### Conversion Rate Optimisation

Use when active for:

- landing pages
- pricing pages
- checkout
- signup
- onboarding
- trial activation
- funnel friction

### SEO

Use when active for:

- public pages
- content structure
- metadata
- crawlability
- semantic HTML
- internal linking
- search intent

### Marketing

Use when active for:

- positioning
- audience clarity
- value propositions
- offers
- campaign pages
- product messaging

### Copywriting

Use when active for:

- headlines
- CTAs
- microcopy
- error messages
- onboarding copy
- empty states
- persuasive clarity

---

## Module Selection Rule

Use active modules only.

If the task would benefit from a planned module, apply the active UX and Design rules first.
Do not invent missing Layr module rules.

When a planned module becomes active, add:

1. a module rule file
2. a matching methods folder
3. routing in `methods/index.md`
4. a changelog entry
