# Surface Playbooks

Use surface playbooks after `SYSTEM.md` identifies the product surface and before selecting detailed methods.

Playbooks turn the system kernel into direct production guidance for common product work. They define required modules, recommended methods, hard gates, production rules, failure patterns, and evidence required before scoring.

---

## Available Playbooks

- `playbooks/pricing.md` - pricing pages, plan comparison, upgrade entry points, and sales qualification paths
- `playbooks/signup-onboarding.md` - signup, login, account creation, first run, activation, and onboarding flows
- `playbooks/dashboards-workspaces.md` - dashboards, workspaces, lists, tables, command surfaces, and operational views
- `playbooks/forms-settings.md` - forms, settings, configuration, profile, permissions, and preference screens
- `playbooks/checkout-upgrade.md` - checkout, payment, subscription change, upgrade, downgrade, and renewal flows
- `playbooks/public-pages-docs.md` - public pages, docs, blogs, content pages, landing pages, and discoverable resources
- `playbooks/ai-features.md` - generation, retrieval, recommendations, agents, automation, and reviewable generated output

---

## Selection Rule

Use one primary playbook for the main surface.

Add a second playbook only when the task crosses a meaningful production boundary.

Examples:

- pricing page with checkout entry: use pricing first, then checkout-upgrade
- onboarding flow with account creation: use signup-onboarding first, then forms-settings
- generated output editor: use ai-features first, then forms-settings if configuration is involved
- public docs with signup CTA: use public-pages-docs first, then signup-onboarding only for the conversion path

---

## Evidence Rule

Do not score a surface until the playbook evidence requirements have been checked.

If evidence is missing, either inspect the implementation, state the remaining risk, or lower the score.
