# Dashboards And Workspaces Playbook

Use this playbook for dashboards, workspaces, admin panels, lists, tables, operational views, command surfaces, and recurring work screens.

---

## Required Modules

- UX
- Design
- Accessibility
- Performance
- QA
- Analytics, when usage or workflow quality must be measured
- Security, when private data, permissions, admin, or sensitive actions are present
- Copywriting, for labels, empty states, and error recovery

---

## Recommended Methods

- `methods/ux/information-scent.md`
- `methods/ux/recognition-over-recall.md`
- `methods/design/information-density.md`
- `methods/design/visual-hierarchy.md`
- `methods/design/data-visualisation.md`
- `methods/performance/interaction-responsiveness.md`
- `methods/performance/rendering-stability.md`
- `methods/accessibility/keyboard-navigation.md`
- `methods/qa/edge-case-states.md`

---

## Hard Gates

- main job of the screen is clear
- scan path supports the user's priority
- primary action is visible and reachable
- data states are covered: empty, loading, error, partial, success
- filters and search preserve orientation
- tables or dense lists remain usable at supported sizes
- permission boundaries are visible when relevant
- actions provide immediate feedback
- performance does not block repeated work

---

## Production Rules

- Put the most decision-relevant data first.
- Avoid equal visual weight across metrics, filters, and actions.
- Keep bulk actions, destructive actions, and permission changes deliberate.
- Use stable loading states that match final layout.
- Prefer visible labels over memory-based icons for critical controls.
- Preserve filter and search state when users move through detail views.
- Show empty states that guide a real next action.
- Keep dense screens compact but not cramped.

---

## Common Failure Patterns

- dashboard becomes a wall of cards
- metrics lack context or change meaning between views
- filters reset unexpectedly
- tables overflow without a usable small-screen strategy
- loading causes layout shift
- empty states are decorative instead of actionable
- permission errors appear only after an attempted action

---

## Evidence Required Before Scoring

- user can identify the most important state or task within seconds
- table, list, filter, and search behaviours are clear
- empty, loading, error, and permission states are represented
- primary and destructive actions are visually distinct
- responsive behaviour has a defined fallback
- performance risk is considered for expensive updates or large data
