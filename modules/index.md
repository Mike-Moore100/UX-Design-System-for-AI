# Modules Index

Use this file to understand which Layr modules are active.

Layr is modular by design.
The user should still only need one prompt.

---

## Active Modules

These modules are part of the current Layr system and must be applied when relevant.

### UX

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
- recognition over recall
- error tolerance
- user control

### Design

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
- responsive composition
- interface states
- data visualisation

### Accessibility

Primary files:

- `ACCESSIBILITY.md`
- `methods/accessibility/`

Use for:

- WCAG-aligned checks
- keyboard navigation
- focus management
- semantic structure
- error identification
- assistive technology support
- accessible names
- contrast and target size
- reduced motion and reflow

### Security

Primary files:

- `SECURITY.md`
- `methods/security/`

Use for:

- authentication flows
- permission boundaries
- secure defaults
- input validation
- sensitive actions
- abuse prevention
- threat modeling
- audit logging
- secrets and dependency safety

### Performance

Primary files:

- `PERFORMANCE.md`
- `methods/performance/`

Use for:

- first useful render
- interaction responsiveness
- loading strategy
- layout stability
- asset weight
- performance budgets
- critical journeys
- perceived speed

### Analytics

Primary files:

- `ANALYTICS.md`
- `methods/analytics/`

Use for:

- event tracking
- funnel measurement
- activation metrics
- experiment measurement
- privacy-aware analytics
- launch measurement
- product learning

### QA

Primary files:

- `QA.md`
- `methods/qa/`

Use for:

- release readiness
- regression risk
- responsive verification
- cross-browser behaviour
- edge-case states
- critical journey checks
- production confidence

### AI Product

Primary files:

- `AI.md`
- `methods/ai/`

Use for:

- AI generation
- AI agents
- prompt input design
- output trust
- human review and control
- AI fallback states
- AI evaluation
- model-assisted decisions

### Conversion Rate Optimisation

Primary files:

- `CRO.md`
- `methods/cro/`

Use for:

- landing pages
- pricing pages
- checkout
- signup
- onboarding
- trial activation
- funnel friction
- message match
- objection handling
- pricing and forms
- experiments

### SEO

Primary files:

- `SEO.md`
- `methods/seo/`

Use for:

- AI search visibility
- public pages
- search intent
- content structure
- metadata
- crawlability
- semantic HTML
- internal linking
- performance
- structured data
- indexing and canonicalisation
- topical authority
- internationalisation

`AI Search` is not a separate active module.
When the user asks for AI search, GEO, AI answers, ChatGPT search, Copilot visibility, or answer-engine visibility, use the SEO module and include `methods/seo/ai-search-visibility.md`.

### Marketing

Primary files:

- `MARKETING.md`
- `methods/marketing/`

Use for:

- positioning
- audience clarity
- value propositions
- offers
- campaign pages
- product messaging
- differentiation
- segmentation
- narrative framing
- proof and launch sequencing
- channel-message fit

### Copywriting

Primary files:

- `COPYWRITING.md`
- `methods/copywriting/`

Use for:

- headlines
- CTAs
- microcopy
- error messages
- onboarding copy
- empty states
- persuasive clarity
- plain language
- objection and trust copy
- pricing copy

---

## Module Selection Rule

Use only modules that materially improve the current task.

If the user provides explicit `Scope:`, start from that scope instead of auto-selecting every relevant module.

Supported scope values:

- `Auto`
- `UX`
- `Design`
- `Accessibility`
- `Security`
- `Performance`
- `Analytics`
- `QA`
- `AI Product`
- `CRO`
- `SEO`
- `AI Search`
- `Marketing`
- `Copywriting`

Default for product UI:

1. UX
2. Design
3. Accessibility

Add Security when the task involves accounts, permissions, data, payments, admin, user-generated content, or sensitive actions.

Add Performance when the task involves slow pages, heavy interfaces, loading states, media, dashboards, mobile performance, or critical journeys.

Add Analytics when the task involves funnels, activation, launches, experiments, growth, measurement, or product learning.

Add QA when the task involves release readiness, regression risk, browser support, responsive layouts, or critical flows.

Add AI Product when the task involves AI generation, agents, retrieval, model-assisted decisions, prompts, AI outputs, or automation.

Add CRO, Marketing, and Copywriting when the task involves acquisition, activation, pricing, signup, onboarding, landing pages, checkout, or user action.

Add SEO when the task involves public pages, content pages, docs, landing pages, blogs, or discoverability.

Do not apply every module to every task.
Select the smallest set that protects quality.

---

## Depth Selection Rule

If the user provides `Depth:`, use it to limit method selection.

- `Quick` - 2-4 methods
- `Standard` - 4-8 methods
- `Deep` - 8-14 methods

If no depth is provided, use `Standard`.

Load only the module files and method files required by the chosen scope and depth.
