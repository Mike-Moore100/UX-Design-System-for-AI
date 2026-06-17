# Signup And Onboarding Playbook

Use this playbook for signup, login, account creation, first run, product activation, and onboarding flows.

---

## Required Modules

- UX
- Design
- Accessibility
- Security
- CRO
- Copywriting
- Analytics
- QA
- AI Product, when onboarding includes generated output or automation

---

## Recommended Methods

- `methods/ux/journey-friction.md`
- `methods/ux/onboarding-momentum.md`
- `methods/ux/goal-gradient.md`
- `methods/security/auth-session-safety.md`
- `methods/security/input-validation.md`
- `methods/cro/form-conversion.md`
- `methods/copywriting/microcopy.md`
- `methods/accessibility/error-identification.md`
- `methods/analytics/activation-metrics.md`
- `methods/qa/regression-checklist.md`

---

## Hard Gates

- first action is obvious
- form labels are visible and associated with inputs
- validation happens at the right time
- errors are specific, recoverable, and accessible
- password and session behaviour are safe
- progress is visible when the flow has multiple steps
- optional setup is deferred until after value when possible
- privacy or data use copy appears near sensitive requests
- activation event is defined when analytics are in scope

---

## Production Rules

- Ask only for information needed to create the account or reach first value.
- Do not use placeholder text as the only label.
- Keep password requirements visible before submission.
- Preserve entered data when errors occur.
- Use progress indicators only for meaningful steps.
- Provide immediate feedback after submit.
- Let users skip optional setup when skipping does not create risk.
- Measure activation as value reached, not only account created.

---

## Common Failure Patterns

- too much setup before first value
- unclear password or auth requirements
- errors appear only after full submission
- users must re-enter information after an error
- onboarding tour blocks actual product use
- optional choices are presented as required
- success state does not tell users what to do next

---

## Evidence Required Before Scoring

- primary signup or next-step action is visible without searching
- form fields have labels, focus states, and recovery paths
- sensitive data requests explain why the data is needed
- loading, error, success, and empty states are handled
- activation metric and key events are defined when measurement is in scope
- keyboard path follows the visual and task order
