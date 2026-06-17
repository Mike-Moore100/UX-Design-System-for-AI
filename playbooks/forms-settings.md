# Forms And Settings Playbook

Use this playbook for forms, settings, configuration, profile screens, permissions, preferences, and admin setup.

---

## Required Modules

- UX
- Design
- Accessibility
- Security, when user data, permissions, auth, billing, or destructive actions are involved
- Copywriting
- QA
- Analytics, when form completion or configuration quality must be measured

---

## Recommended Methods

- `methods/ux/error-prevention-recovery.md`
- `methods/ux/error-tolerance.md`
- `methods/accessibility/accessible-names.md`
- `methods/accessibility/error-identification.md`
- `methods/security/input-validation.md`
- `methods/security/sensitive-action-confirmation.md`
- `methods/copywriting/microcopy.md`
- `methods/copywriting/error-message-copy.md`
- `methods/design/component-consistency.md`
- `methods/qa/edge-case-states.md`

---

## Hard Gates

- every input has a visible label
- helper text clarifies unfamiliar or risky inputs
- validation occurs at the correct trust boundary
- errors identify the field, issue, and recovery action
- save state is visible
- destructive or sensitive actions require deliberate confirmation
- keyboard flow is predictable
- settings changes are confirmed or reversible when risk exists

---

## Production Rules

- Group related fields by user intent, not database structure.
- Put constraints near the input.
- Validate client-side for speed and server-side for trust.
- Avoid disabling submit without explaining what is missing.
- Preserve user input after failed submission.
- Separate destructive actions from routine settings.
- Use plain language for errors and confirmations.
- Make unsaved changes visible before navigation.

---

## Common Failure Patterns

- placeholder text is used as the only label
- validation messages are vague
- save state is invisible
- errors clear user input
- destructive actions sit beside routine actions
- settings are organized by internal system terms
- keyboard users cannot reach or complete the form

---

## Evidence Required Before Scoring

- labels, helper text, and errors are visible and accessible
- submit, saving, saved, failed, and unsaved states exist when relevant
- sensitive and destructive actions are protected
- validation happens both where users need guidance and where the system needs trust
- field order matches the user's task
- recovery path is clear for every likely failure
