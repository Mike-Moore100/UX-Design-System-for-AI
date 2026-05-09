# Layr Scorecard

Use this scorecard after applying the relevant Layr modules.

A score is not valid unless it includes evidence from the actual interface, content, or implementation.

---

## Hard Gates

If any relevant hard gate fails, the screen cannot score above 84.

- one clear primary action exists when the surface requires action
- primary action is visually dominant
- screen is understandable within 3 seconds
- clickable targets are at least 40x40px on desktop or 44x44px on touch interfaces
- keyboard navigation and focus states work
- text contrast is accessible
- form errors are identifiable and recoverable
- sensitive actions are clear, permissioned, and protected
- user input is validated at the correct trust boundary
- public pages have semantic structure and useful metadata
- public pages targeting AI search have crawlable, quote-ready content and appropriate crawler controls
- conversion surfaces have a clear value proposition and CTA
- empty, loading, error, and success states are handled when relevant
- performance-critical surfaces show stable loading and responsive interaction
- AI outputs are reviewable, correctable, and honest about uncertainty when relevant
- release-critical flows have regression, responsive, and edge-state evidence

---

## Scoring

Score every screen or page out of 100:

- UX clarity and task fit: 0-15
- Flow and friction: 0-15
- Visual design and hierarchy: 0-15
- Accessibility: 0-15
- Trust, safety, security, and privacy: 0-10
- Conversion and action strength: 0-10
- Content and copy clarity: 0-10
- Technical quality, performance, QA, and discoverability: 0-10

Pass: 85+
Fail: below 85

For private app screens where SEO is not relevant, score technical quality and discoverability based on semantic structure, performance, and implementation quality.

---

## Evidence Requirements

For each score category, identify:

- what improved
- what still creates friction or risk
- what was changed or should be changed next

Do not award high scores for intentions.
Score the actual interface, content, and implementation, not the explanation.

---

## Module Evidence

When a module is relevant, include evidence for it:

- UX: primary action, flow, cognitive load, recognition, feedback, user control
- Design: hierarchy, spacing, colour, typography, components, states, responsive composition
- Accessibility: keyboard, focus, names, semantics, contrast, errors, motion, reflow
- Security: permissions, validation, auth, safe defaults, sensitive actions, logging, abuse prevention
- Performance: first useful render, loading, responsiveness, stability, asset cost
- Analytics: event taxonomy, funnels, activation, experiments, privacy-aware measurement
- QA: responsive checks, browser risk, edge states, regression checks, release readiness
- AI Product: prompt input, output trust, human control, fallbacks, evaluation
- CRO: value clarity, message match, proof, objections, pricing, CTA, friction, testing
- SEO: intent, semantic HTML, metadata, indexing, structured data, internal links, performance, AI search visibility, credibility
- Marketing: positioning, segmentation, offer, narrative, proof, differentiation, channel fit
- Copywriting: headlines, clarity, specificity, microcopy, errors, onboarding, pricing, trust copy

---

## Score Guidance

### 95-100

Exceptional. The product surface is obvious, fast, accessible, trustworthy, visually focused, and strongly aligned with the user's goal.

### 85-94

Strong. The surface is usable and clear, with only minor improvements remaining.

### 70-84

Not good enough. The surface may work, but important friction, risk, or missed opportunity remains.

### Below 70

Failed. The user is likely to hesitate, misunderstand, abandon, make errors, or encounter preventable risk.

---

## Improvement Loop

If the score is below 85:

1. identify the lowest scoring category
2. fix the largest source of friction, risk, or ambiguity
3. remove unnecessary elements before adding new ones
4. rescore using evidence
5. repeat until the score is at least 85
