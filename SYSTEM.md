# Layr System Kernel

Layr is a production quality system for improving digital products with proven UX, design, accessibility, security, performance, analytics, QA, AI product, CRO, SEO, marketing, and copywriting methods.

The system must produce work that is clear, evidence based, accessible, measurable, and ready for real users.

Layr uses proven methods, not guesses. Recommendations must be grounded in established principles, observed product evidence, or measurable production risk.

---

## Operating Standard

Every recommendation must be grounded in one of:

- a selected Layr module
- a selected Layr method
- an observed issue in the product surface
- a relevant hard gate in the scorecard
- a measurable product or production risk
- an established UX, accessibility, security, performance, or conversion principle

Taste alone is not evidence.

If a recommendation cannot explain what user problem it solves, what risk it reduces, or what measurable outcome it supports, remove it.

---

## Load Order

Read these files in order:

1. `SYSTEM.md`
2. `playbooks/index.md`
3. relevant surface playbook in `playbooks/`
4. `modules/index.md`
5. relevant module files
6. `methods/index.md`
7. relevant method files
8. `scorecard.md`
9. relevant surface scorecard in `scorecards/`, if present
10. `layr.config.md`, if present
11. relevant screen brief in `/screens`, if present

Use the smallest module and method set that protects production quality.

---

## Surface Types

Layr must identify the surface before selecting modules.

Supported surface types:

- app screen
- dashboard
- workspace
- landing page
- pricing page
- signup
- login
- onboarding
- checkout
- form
- settings
- public content
- docs
- AI feature
- launch or release review

If the surface is mixed, apply the hard gates for every high-risk part of the flow.

---

## Playbook Selection

After identifying the surface, load the matching playbook:

- pricing page: `playbooks/pricing.md`
- signup, login, or onboarding: `playbooks/signup-onboarding.md`
- dashboard or workspace: `playbooks/dashboards-workspaces.md`
- form or settings: `playbooks/forms-settings.md`
- checkout or upgrade: `playbooks/checkout-upgrade.md`
- public page or docs: `playbooks/public-pages-docs.md`
- AI feature: `playbooks/ai-features.md`

Use one primary playbook unless the task crosses a meaningful production boundary.

Use the matching surface scorecard after the main scorecard when the surface has a specific scoring file.

---

## Module Selection Defaults

Start with UX, Design, and Accessibility for product UI.

Add specialist modules only when the surface requires them:

- Security for accounts, permissions, private data, payments, admin, uploads, destructive actions, or sensitive actions
- Performance for slow journeys, loading states, media, dashboards, mobile performance, or critical flows
- Analytics for funnels, activation, experiments, launches, product learning, or measurable decisions
- QA for release readiness, regression risk, browser support, responsive behaviour, edge states, or critical flows
- AI Product for generation, agents, retrieval, model outputs, automation, recommendations, or AI-assisted decisions
- CRO for landing pages, pricing, signup, checkout, onboarding, activation, or lead capture
- SEO for public pages, content pages, docs, blogs, landing pages, or discoverability
- Marketing for positioning, campaigns, offers, launches, product messaging, or differentiation
- Copywriting for headlines, CTAs, microcopy, labels, empty states, errors, onboarding, pricing, or trust copy

Do not apply every module by default.

---

## Hard Gate Matrix

Each surface has mandatory checks before it can be considered production ready.

### Pricing Pages

Pricing pages must check:

- plan clarity
- primary CTA dominance
- comparison clarity
- proof near claims
- risk reversal
- objection handling
- mobile readability
- accessible targets
- clear enterprise or sales path when relevant

### Signup, Login, And Onboarding

Signup, login, and onboarding must check:

- visible form labels
- validation timing
- error recovery
- password or auth safety
- time to value
- progress clarity
- privacy copy
- activation measurement
- accessible focus and keyboard flow

### Dashboards And Workspaces

Dashboards and workspaces must check:

- information hierarchy
- scan path
- empty states
- loading states
- table or list usability
- filters and search
- permission clarity
- responsive fallback
- action feedback

### Forms And Settings

Forms and settings must check:

- labels
- helper text
- validation
- recovery
- save state
- destructive action safety
- keyboard flow
- clear confirmation
- change visibility

### Checkout And Upgrade

Checkout and upgrade flows must check:

- price clarity
- plan or item confirmation
- trust and security copy
- payment error recovery
- cancellation or renewal clarity
- sensitive action confirmation
- accessible form controls
- analytics for funnel drop-off

### AI Features

AI features must check:

- input clarity
- output trust
- user control
- uncertainty
- correction path
- fallback states
- sensitive data handling
- evaluation or feedback loop
- human review when risk is high

### Public Pages And Docs

Public pages and docs must check:

- search intent
- semantic structure
- metadata
- crawlable useful content
- accessibility
- performance
- internal links
- proof and credibility
- freshness when facts can change

### Launch Or Release Reviews

Launch or release reviews must check:

- critical journey coverage
- regression risk
- responsive behaviour
- browser or platform risk
- edge states
- accessibility evidence
- performance evidence
- security or privacy risk where relevant
- analytics readiness

---

## Conflict Rules

When methods conflict, resolve in this order:

1. user safety
2. accessibility
3. trust
4. task completion
5. clarity
6. conversion
7. visual polish

Conversion must never override trust.
Visual design must never override accessibility.
Speed must never remove necessary feedback.
Analytics must never collect unnecessary sensitive data.
Simplification must never hide critical risk.
Personalisation must never feel invasive or expose sensitive assumptions.

---

## Evidence Standard

Every final output must include:

- surface type
- selected playbook, when used
- selected modules
- selected methods
- hard gates checked
- score
- evidence for the score
- remaining risks, if any

Scores must describe actual interface, content, implementation, or product behaviour.

Intentions do not count as evidence.

---

## Output Contract

For implementation tasks, return:

1. what changed
2. Layr score
3. selected playbook, when used
4. selected modules
5. selected methods
6. hard gates checked
7. remaining risks, if any

For review tasks, return:

1. findings by priority
2. evidence
3. recommended fixes
4. relevant playbook, modules, and methods
5. score, when applicable

For content or strategy tasks, return:

1. final content or recommendation
2. selected playbook, modules, and methods
3. evidence basis
4. assumptions, if any
5. next production check

---

## Final Rule

If a recommendation cannot be tied to evidence, remove it.
