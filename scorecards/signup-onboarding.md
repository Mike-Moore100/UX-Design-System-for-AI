# Signup And Onboarding Scorecard

Score signup, login, account creation, first run, activation, and onboarding flows out of 100.

---

## Categories

- Time to value: 0-15
- Form clarity and completion: 0-15
- Validation and error recovery: 0-15
- Auth safety and privacy trust: 0-15
- Progress and user control: 0-10
- Accessibility and keyboard flow: 0-10
- Activation measurement: 0-10
- State coverage and QA readiness: 0-10

---

## Hard Cap Rules

The flow cannot score above 84 if:

- labels are missing or only placeholders
- errors are not recoverable
- password or auth requirements are unclear
- user must complete unnecessary setup before value
- sensitive data requests lack context

The flow cannot score above 70 if:

- account creation can fail without actionable recovery
- keyboard users cannot complete the flow
- activation is not definable from the implemented journey

---

## Evidence Required

- primary first action is obvious
- required fields, constraints, and errors are visible
- loading, success, and failure states exist
- sensitive requests are explained
- optional setup is deferred or clearly marked
- activation event reflects value reached
