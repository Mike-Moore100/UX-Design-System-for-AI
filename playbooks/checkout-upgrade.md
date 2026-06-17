# Checkout And Upgrade Playbook

Use this playbook for checkout, payment, subscription change, upgrade, downgrade, renewal, cancellation, and paid plan confirmation flows.

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
- Performance, when payment or plan screens depend on async loading

---

## Recommended Methods

- `methods/ux/error-prevention-recovery.md`
- `methods/ux/recognition-over-recall.md`
- `methods/security/sensitive-action-confirmation.md`
- `methods/security/secure-error-handling.md`
- `methods/cro/risk-reversal.md`
- `methods/cro/funnel-friction.md`
- `methods/copywriting/trust-copy.md`
- `methods/analytics/funnel-instrumentation.md`
- `methods/qa/release-readiness.md`

---

## Hard Gates

- user can verify what they are buying or changing
- price, billing period, renewal, taxes, and trial terms are visible before confirmation
- payment and billing errors are recoverable
- sensitive plan changes require clear confirmation
- cancellation or downgrade impact is explained when relevant
- security and privacy copy is close to high-trust actions
- duplicate submissions are prevented
- funnel events are defined when analytics are in scope

---

## Production Rules

- Summarize the selected plan or item near the confirmation action.
- Make total cost and billing timing explicit.
- Keep payment form labels visible and accessible.
- Do not hide renewal, cancellation, or trial terms.
- Prevent repeated clicks from creating duplicate side effects.
- Use secure, user-safe error copy that does not expose internals.
- Confirm successful purchase or plan change with the next useful action.
- Track step view, payment submit, payment failure, payment success, plan change, and cancellation intent when relevant.

---

## Common Failure Patterns

- total price is not visible before confirmation
- trial or renewal terms are unclear
- payment failure gives no recovery path
- plan change impact is hidden
- primary action says only "Continue"
- duplicate submits are possible
- success state is a dead end

---

## Evidence Required Before Scoring

- selected plan, cost, billing period, and terms are visible
- sensitive action copy explains impact
- payment and plan-change errors are recoverable
- success state confirms the outcome and next step
- duplicate side effects are prevented
- analytics covers the critical funnel and failure points
