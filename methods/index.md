# Methods Index

Use this file to choose the right Layr methods for the task.

Do not apply every method to every screen.
Select only the methods that materially improve the user's current goal.

Layr methods are split by active module:

- `methods/ux/` - behaviour, cognition, interaction, flow, trust, and task completion
- `methods/design/` - visual craft, colour, typography, layout, spacing, contrast, components, and motion
- `methods/accessibility/` - perceivable, operable, understandable, robust, and assistive technology support
- `methods/security/` - safe defaults, permissions, validation, auth, and sensitive actions
- `methods/performance/` - speed, responsiveness, loading, stability, assets, and performance budgets
- `methods/analytics/` - events, funnels, activation, experiments, and privacy-aware measurement
- `methods/qa/` - release readiness, regression, responsive QA, cross-browser checks, and edge states
- `methods/ai/` - AI input design, output trust, human control, fallbacks, and evaluation
- `methods/cro/` - value clarity, proof, risk reduction, CTAs, pricing, forms, and experimentation
- `methods/seo/` - search intent, semantic HTML, AI search visibility, metadata, indexing, structured data, authority, and performance
- `methods/marketing/` - positioning, segmentation, narrative, offers, proof, launches, and differentiation
- `methods/copywriting/` - clarity, headlines, plain language, objections, errors, onboarding, pricing, and trust copy

Use UX methods to decide what the experience should do.
Use design methods to decide how the interface should visually communicate it.
Use specialist modules only when the task needs them.

---

## Universal Production Set

Start from these on most product UI tasks.
Select only the methods that fit the chosen scope and depth:

- `methods/ux/cognitive-load-theory.md` - reduce mental effort
- `methods/ux/fitts-law.md` - make interaction fast and accurate
- `methods/ux/affordance.md` - make interactive elements self-evident
- `methods/ux/feedback-loops.md` - make actions visibly respond
- `methods/design/visual-hierarchy.md` - make the main thing obvious
- `methods/design/signal-to-noise.md` - remove visual and content noise
- `methods/accessibility/wcag-pour.md` - protect baseline accessibility
- `methods/performance/loading-strategy.md` - make waiting visible and stable
- `methods/qa/edge-case-states.md` - protect non-happy-path states

---

## Scope And Depth

Use the user's `Scope:` and `Depth:` values when provided.

If no scope is provided, use `Scope: Auto`.
If no depth is provided, use `Depth: Standard`.

Depth limits:

- `Quick` - select 2-4 methods
- `Standard` - select 4-8 methods
- `Deep` - select 8-14 methods

Do not load every method in this index unless the user asks for a full audit.
Select only the smallest method set that improves the current task.

If the user asks for `AI Search`, treat it as SEO scope and include `methods/seo/ai-search-visibility.md`.
If the user asks for AI features, agents, generation, model outputs, retrieval, or automation, include AI Product methods from `methods/ai/`.

---

## UX Methods

Use when the task involves behaviour, flow, decisions, friction, trust, feedback, or interaction quality.

- `methods/ux/affordance.md`
- `methods/ux/attention-ratio.md`
- `methods/ux/choice-architecture.md`
- `methods/ux/cognitive-load-theory.md`
- `methods/ux/contextual-help.md`
- `methods/ux/decision-fatigue.md`
- `methods/ux/default-bias.md`
- `methods/ux/doherty-threshold.md`
- `methods/ux/error-prevention-recovery.md`
- `methods/ux/error-tolerance.md`
- `methods/ux/feedback-loops.md`
- `methods/ux/fitts-law.md`
- `methods/ux/goal-gradient.md`
- `methods/ux/hicks-law.md`
- `methods/ux/information-scent.md`
- `methods/ux/jakobs-law.md`
- `methods/ux/journey-friction.md`
- `methods/ux/mental-models.md`
- `methods/ux/millers-law.md`
- `methods/ux/onboarding-momentum.md`
- `methods/ux/peak-end-rule.md`
- `methods/ux/perceived-performance.md`
- `methods/ux/progressive-disclosure.md`
- `methods/ux/recognition-over-recall.md`
- `methods/ux/serial-position-effect.md`
- `methods/ux/teslers-law.md`
- `methods/ux/trust-signals.md`
- `methods/ux/user-control-freedom.md`
- `methods/ux/von-restorff-effect.md`
- `methods/ux/zeigarnik-effect.md`

## Design Methods

Use when the task involves visual quality, hierarchy, brand fit, spacing, colour, typography, layout, component polish, or motion.

- `methods/design/aesthetic-usability.md`
- `methods/design/colour-theory.md`
- `methods/design/component-consistency.md`
- `methods/design/contrast-and-emphasis.md`
- `methods/design/data-visualisation.md`
- `methods/design/design-tokens.md`
- `methods/design/empty-state-design.md`
- `methods/design/gestalt-principles.md`
- `methods/design/grid-systems.md`
- `methods/design/iconography.md`
- `methods/design/imagery-art-direction.md`
- `methods/design/information-density.md`
- `methods/design/layout-composition.md`
- `methods/design/motion-clarity.md`
- `methods/design/responsive-composition.md`
- `methods/design/signal-to-noise.md`
- `methods/design/spacing-rhythm.md`
- `methods/design/state-design.md`
- `methods/design/typography.md`
- `methods/design/visual-hierarchy.md`
- `methods/design/visual-weight.md`

## Accessibility Methods

Use when the task involves any user-facing interface, especially forms, navigation, state changes, or assistive technology support.

- `methods/accessibility/accessible-names.md`
- `methods/accessibility/alt-text-decision-tree.md`
- `methods/accessibility/aria-authoring.md`
- `methods/accessibility/captions-transcripts.md`
- `methods/accessibility/contrast-minimums.md`
- `methods/accessibility/error-identification.md`
- `methods/accessibility/focus-management.md`
- `methods/accessibility/keyboard-navigation.md`
- `methods/accessibility/live-regions.md`
- `methods/accessibility/plain-language.md`
- `methods/accessibility/reduced-motion.md`
- `methods/accessibility/semantic-structure.md`
- `methods/accessibility/target-size.md`
- `methods/accessibility/wcag-pour.md`
- `methods/accessibility/zoom-reflow.md`

## Security Methods

Use when the task involves accounts, permissions, data, payments, admin, uploads, user-generated content, or sensitive actions.

- `methods/security/audit-logging.md`
- `methods/security/auth-session-safety.md`
- `methods/security/csrf-protection.md`
- `methods/security/data-minimisation.md`
- `methods/security/dependency-safety.md`
- `methods/security/input-validation.md`
- `methods/security/least-privilege.md`
- `methods/security/rate-limiting.md`
- `methods/security/secrets-management.md`
- `methods/security/secure-defaults.md`
- `methods/security/secure-error-handling.md`
- `methods/security/secure-file-uploads.md`
- `methods/security/sensitive-action-confirmation.md`
- `methods/security/threat-modeling.md`
- `methods/security/xss-prevention.md`

## Performance Methods

Use when the task involves speed, loading, responsiveness, stability, mobile performance, dashboards, media, or critical journeys.

- `methods/performance/asset-optimization.md`
- `methods/performance/interaction-responsiveness.md`
- `methods/performance/loading-strategy.md`
- `methods/performance/performance-budget.md`
- `methods/performance/rendering-stability.md`

## Analytics Methods

Use when the task involves measurement, funnels, activation, experiments, launches, product learning, or analytics implementation.

- `methods/analytics/activation-metrics.md`
- `methods/analytics/event-taxonomy.md`
- `methods/analytics/experiment-measurement.md`
- `methods/analytics/funnel-instrumentation.md`
- `methods/analytics/privacy-aware-analytics.md`

## QA Methods

Use when the task involves release readiness, regression risk, responsive behaviour, browser support, edge cases, or production confidence.

- `methods/qa/cross-browser-qa.md`
- `methods/qa/edge-case-states.md`
- `methods/qa/regression-checklist.md`
- `methods/qa/release-readiness.md`
- `methods/qa/responsive-qa.md`

## AI Product Methods

Use when the task involves AI generation, agents, retrieval, model-assisted decisions, prompts, outputs, automation, or AI evaluation.

- `methods/ai/ai-evaluation.md`
- `methods/ai/ai-fallbacks.md`
- `methods/ai/human-control.md`
- `methods/ai/output-trust.md`
- `methods/ai/prompt-input-design.md`

## CRO Methods

Use when the task involves conversion, activation, signup, pricing, checkout, trials, or lead capture.

- `methods/cro/commitment-consistency.md`
- `methods/cro/cta-specificity.md`
- `methods/cro/ethical-urgency.md`
- `methods/cro/experiment-hypothesis.md`
- `methods/cro/form-conversion.md`
- `methods/cro/funnel-friction.md`
- `methods/cro/landing-page-flow.md`
- `methods/cro/lead-magnet.md`
- `methods/cro/message-match.md`
- `methods/cro/objection-handling.md`
- `methods/cro/price-anchoring.md`
- `methods/cro/risk-reversal.md`
- `methods/cro/segmentation-personalisation.md`
- `methods/cro/social-proof.md`
- `methods/cro/value-proposition-clarity.md`

## SEO Methods

Use when the task involves public pages, content pages, landing pages, docs, blogs, discoverability, AI search visibility, GEO, AI answers, or answer-engine visibility.

- `methods/seo/ai-search-visibility.md`
- `methods/seo/canonicalisation.md`
- `methods/seo/content-refresh.md`
- `methods/seo/core-web-vitals.md`
- `methods/seo/eeat-signals.md`
- `methods/seo/hreflang-international.md`
- `methods/seo/image-seo.md`
- `methods/seo/internal-linking.md`
- `methods/seo/local-seo.md`
- `methods/seo/metadata-snippets.md`
- `methods/seo/pagination-faceted-navigation.md`
- `methods/seo/robots-indexing.md`
- `methods/seo/search-intent-alignment.md`
- `methods/seo/semantic-html.md`
- `methods/seo/structured-data.md`
- `methods/seo/topical-authority.md`

## Marketing Methods

Use when the task involves positioning, launch pages, campaigns, product messaging, offers, or differentiation.

- `methods/marketing/audience-message-fit.md`
- `methods/marketing/brand-voice.md`
- `methods/marketing/category-design.md`
- `methods/marketing/channel-message-fit.md`
- `methods/marketing/competitive-alternatives.md`
- `methods/marketing/customer-segmentation.md`
- `methods/marketing/differentiation.md`
- `methods/marketing/jtbd-positioning.md`
- `methods/marketing/launch-sequencing.md`
- `methods/marketing/message-hierarchy.md`
- `methods/marketing/narrative-framing.md`
- `methods/marketing/offer-architecture.md`
- `methods/marketing/positioning.md`
- `methods/marketing/problem-agitation-solution.md`
- `methods/marketing/proof-stack.md`

## Copywriting Methods

Use when the task involves headlines, CTAs, microcopy, empty states, errors, onboarding copy, or persuasive clarity.

- `methods/copywriting/benefit-led-copy.md`
- `methods/copywriting/clarity-first.md`
- `methods/copywriting/cta-copy.md`
- `methods/copywriting/empty-state-copy.md`
- `methods/copywriting/error-message-copy.md`
- `methods/copywriting/headline-clarity.md`
- `methods/copywriting/jobs-to-be-done-copy.md`
- `methods/copywriting/microcopy.md`
- `methods/copywriting/objection-copy.md`
- `methods/copywriting/onboarding-copy.md`
- `methods/copywriting/plain-language-copy.md`
- `methods/copywriting/pricing-copy.md`
- `methods/copywriting/specificity.md`
- `methods/copywriting/trust-copy.md`
- `methods/copywriting/voice-and-tone.md`

---

## By Surface Type

### App Screen, Dashboard, Workspace

Use:

- UX
- Design
- Accessibility
- Performance
- QA

Add Security if the screen handles private data, permissions, admin, uploads, or sensitive actions.

Common methods:

- `methods/ux/cognitive-load-theory.md`
- `methods/ux/information-scent.md`
- `methods/ux/progressive-disclosure.md`
- `methods/ux/recognition-over-recall.md`
- `methods/design/visual-hierarchy.md`
- `methods/design/layout-composition.md`
- `methods/design/information-density.md`
- `methods/accessibility/wcag-pour.md`
- `methods/accessibility/keyboard-navigation.md`
- `methods/performance/interaction-responsiveness.md`
- `methods/qa/edge-case-states.md`

### Landing, Hero, Marketing, Conversion

Use:

- UX
- Design
- Accessibility
- CRO
- Marketing
- Copywriting
- Performance
- Analytics
- SEO, if public

Common methods:

- `methods/cro/value-proposition-clarity.md`
- `methods/cro/message-match.md`
- `methods/cro/landing-page-flow.md`
- `methods/marketing/positioning.md`
- `methods/marketing/message-hierarchy.md`
- `methods/marketing/proof-stack.md`
- `methods/copywriting/clarity-first.md`
- `methods/copywriting/headline-clarity.md`
- `methods/design/visual-hierarchy.md`
- `methods/seo/search-intent-alignment.md`
- `methods/performance/asset-optimization.md`
- `methods/analytics/funnel-instrumentation.md`

### Signup, Login, Onboarding

Use:

- UX
- Design
- Accessibility
- Security
- CRO
- Copywriting
- Analytics
- QA

Common methods:

- `methods/ux/journey-friction.md`
- `methods/ux/onboarding-momentum.md`
- `methods/security/auth-session-safety.md`
- `methods/security/csrf-protection.md`
- `methods/cro/funnel-friction.md`
- `methods/cro/form-conversion.md`
- `methods/copywriting/microcopy.md`
- `methods/copywriting/onboarding-copy.md`
- `methods/accessibility/error-identification.md`
- `methods/design/component-consistency.md`
- `methods/analytics/activation-metrics.md`
- `methods/qa/regression-checklist.md`

### Pricing, Plans, Checkout, Upgrade

Use:

- UX
- Design
- Accessibility
- Security
- CRO
- Marketing
- Copywriting
- Analytics
- QA
- SEO, if public

Common methods:

- `methods/ux/hicks-law.md`
- `methods/ux/choice-architecture.md`
- `methods/cro/risk-reversal.md`
- `methods/cro/social-proof.md`
- `methods/cro/price-anchoring.md`
- `methods/copywriting/cta-copy.md`
- `methods/copywriting/pricing-copy.md`
- `methods/security/sensitive-action-confirmation.md`
- `methods/design/contrast-and-emphasis.md`
- `methods/analytics/funnel-instrumentation.md`
- `methods/qa/release-readiness.md`

### Forms, Settings, Configuration

Use:

- UX
- Design
- Accessibility
- Security, if user data or permissions are involved
- Copywriting
- QA

Common methods:

- `methods/ux/error-prevention-recovery.md`
- `methods/ux/error-tolerance.md`
- `methods/accessibility/error-identification.md`
- `methods/accessibility/accessible-names.md`
- `methods/security/input-validation.md`
- `methods/cro/form-conversion.md`
- `methods/copywriting/microcopy.md`
- `methods/copywriting/error-message-copy.md`
- `methods/design/component-consistency.md`
- `methods/qa/edge-case-states.md`

### Public Content, Blog, Docs

Use:

- UX
- Design
- Accessibility
- SEO
- Copywriting
- Performance

Common methods:

- `methods/seo/search-intent-alignment.md`
- `methods/seo/semantic-html.md`
- `methods/seo/metadata-snippets.md`
- `methods/seo/structured-data.md`
- `methods/seo/eeat-signals.md`
- `methods/copywriting/clarity-first.md`
- `methods/copywriting/plain-language-copy.md`
- `methods/design/typography.md`
- `methods/accessibility/semantic-structure.md`
- `methods/performance/asset-optimization.md`

### AI Feature, Agent, Generation, Retrieval

Use:

- AI Product
- UX
- Design
- Accessibility
- Security, when data or actions are sensitive
- Performance, when responses are slow or streaming
- Analytics, when quality or adoption must be measured
- QA

Common methods:

- `methods/ai/prompt-input-design.md`
- `methods/ai/output-trust.md`
- `methods/ai/human-control.md`
- `methods/ai/ai-fallbacks.md`
- `methods/ai/ai-evaluation.md`
- `methods/security/data-minimisation.md`
- `methods/performance/loading-strategy.md`
- `methods/analytics/privacy-aware-analytics.md`
- `methods/qa/edge-case-states.md`

### Launch, Release, Production Readiness

Use:

- QA
- Performance
- Analytics
- Accessibility
- Security, if risk exists
- relevant product modules for the surface

Common methods:

- `methods/qa/release-readiness.md`
- `methods/qa/regression-checklist.md`
- `methods/qa/responsive-qa.md`
- `methods/performance/performance-budget.md`
- `methods/analytics/event-taxonomy.md`
- `methods/analytics/experiment-measurement.md`

---

## By Problem

### User does not know what to do

- `methods/ux/information-scent.md`
- `methods/ux/attention-ratio.md`
- `methods/ux/affordance.md`
- `methods/ux/mental-models.md`
- `methods/design/visual-hierarchy.md`
- `methods/copywriting/clarity-first.md`

### Screen feels cluttered

- `methods/design/signal-to-noise.md`
- `methods/design/spacing-rhythm.md`
- `methods/design/layout-composition.md`
- `methods/design/grid-systems.md`
- `methods/design/information-density.md`
- `methods/ux/millers-law.md`

### Screen feels slow or unstable

- `methods/performance/performance-budget.md`
- `methods/performance/loading-strategy.md`
- `methods/performance/interaction-responsiveness.md`
- `methods/performance/rendering-stability.md`
- `methods/performance/asset-optimization.md`
- `methods/ux/perceived-performance.md`

### Page does not convert

- `methods/cro/value-proposition-clarity.md`
- `methods/cro/message-match.md`
- `methods/cro/funnel-friction.md`
- `methods/cro/social-proof.md`
- `methods/cro/objection-handling.md`
- `methods/copywriting/cta-copy.md`
- `methods/marketing/offer-architecture.md`
- `methods/marketing/proof-stack.md`
- `methods/analytics/funnel-instrumentation.md`

### Page will be public and discoverable

- `methods/seo/search-intent-alignment.md`
- `methods/seo/semantic-html.md`
- `methods/seo/metadata-snippets.md`
- `methods/seo/internal-linking.md`
- `methods/seo/core-web-vitals.md`
- `methods/seo/structured-data.md`
- `methods/seo/canonicalisation.md`

### Page should appear in AI answers

- `methods/seo/ai-search-visibility.md`
- `methods/seo/search-intent-alignment.md`
- `methods/seo/semantic-html.md`
- `methods/seo/structured-data.md`
- `methods/seo/eeat-signals.md`
- `methods/seo/content-refresh.md`
- `methods/copywriting/plain-language-copy.md`
- `methods/marketing/proof-stack.md`

### Flow handles sensitive data or actions

- `methods/security/least-privilege.md`
- `methods/security/secure-defaults.md`
- `methods/security/input-validation.md`
- `methods/security/auth-session-safety.md`
- `methods/security/sensitive-action-confirmation.md`
- `methods/security/audit-logging.md`
- `methods/security/secure-error-handling.md`
- `methods/analytics/privacy-aware-analytics.md`

### Copy feels vague or weak

- `methods/copywriting/clarity-first.md`
- `methods/copywriting/specificity.md`
- `methods/copywriting/jobs-to-be-done-copy.md`
- `methods/copywriting/headline-clarity.md`
- `methods/copywriting/benefit-led-copy.md`
- `methods/marketing/positioning.md`
- `methods/marketing/differentiation.md`

### User hesitates before acting

- `methods/cro/objection-handling.md`
- `methods/cro/risk-reversal.md`
- `methods/copywriting/objection-copy.md`
- `methods/copywriting/trust-copy.md`
- `methods/ux/trust-signals.md`
- `methods/marketing/proof-stack.md`

### Content needs to scale across audiences

- `methods/marketing/customer-segmentation.md`
- `methods/cro/segmentation-personalisation.md`
- `methods/marketing/channel-message-fit.md`
- `methods/marketing/jtbd-positioning.md`
- `methods/copywriting/voice-and-tone.md`

### Interface states feel unfinished

- `methods/design/state-design.md`
- `methods/design/empty-state-design.md`
- `methods/copywriting/empty-state-copy.md`
- `methods/copywriting/error-message-copy.md`
- `methods/accessibility/live-regions.md`
- `methods/ux/feedback-loops.md`
- `methods/qa/edge-case-states.md`

### Product impact is hard to measure

- `methods/analytics/event-taxonomy.md`
- `methods/analytics/funnel-instrumentation.md`
- `methods/analytics/activation-metrics.md`
- `methods/analytics/experiment-measurement.md`
- `methods/analytics/privacy-aware-analytics.md`

### Release risk is unclear

- `methods/qa/release-readiness.md`
- `methods/qa/regression-checklist.md`
- `methods/qa/responsive-qa.md`
- `methods/qa/cross-browser-qa.md`
- `methods/qa/edge-case-states.md`

### AI output feels risky or unreliable

- `methods/ai/output-trust.md`
- `methods/ai/human-control.md`
- `methods/ai/ai-fallbacks.md`
- `methods/ai/ai-evaluation.md`
- `methods/ai/prompt-input-design.md`
- `methods/security/data-minimisation.md`

---

## Selection Rule

Pick 4-8 methods for normal tasks.
Start with UX, Design, and Accessibility.

Add specialist modules only when the surface requires them:

- Security for sensitive data, accounts, permissions, admin, uploads, or destructive actions
- Performance for speed, loading, responsiveness, media, dashboards, and critical journeys
- Analytics for funnels, activation, experiments, launches, and product measurement
- QA for release readiness, regression risk, responsive QA, browser support, and edge states
- AI Product for AI generation, agents, retrieval, model outputs, automation, and AI-assisted decisions
- CRO for conversion, signup, pricing, checkout, activation, or lead capture
- SEO for public discoverable pages
- AI Search for AI answers, ChatGPT search, Copilot visibility, GEO, or answer-engine visibility
- Marketing for positioning, campaigns, offers, and product messaging
- Copywriting for headlines, CTAs, microcopy, labels, errors, and empty states

If two methods conflict, choose the one that better supports user trust and the primary action.
