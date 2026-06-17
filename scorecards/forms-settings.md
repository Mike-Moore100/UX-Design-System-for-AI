# Forms And Settings Scorecard

Score forms, settings, configuration, profile screens, permissions, and preference surfaces out of 100.

---

## Categories

- Field clarity and grouping: 0-15
- Validation and recovery: 0-15
- Save state and confirmation: 0-15
- Security and sensitive action safety: 0-15
- Accessibility and keyboard flow: 0-10
- Copy and helper text quality: 0-10
- State coverage: 0-10
- QA and measurement readiness: 0-10

---

## Hard Cap Rules

The surface cannot score above 84 if:

- inputs lack visible labels
- errors do not explain recovery
- save state is unclear
- destructive or sensitive actions are not protected
- keyboard flow is broken

The surface cannot score above 70 if:

- users can lose entered data during normal recovery
- validation only happens after preventable failure
- settings changes have unclear impact

---

## Evidence Required

- labels, constraints, helper text, and errors are visible
- validation is useful to the user and safe for the system
- save, saved, failed, and unsaved states are clear
- destructive actions require deliberate confirmation
- keyboard path supports completion
- field grouping matches user intent
