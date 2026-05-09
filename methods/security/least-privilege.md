# Least Privilege

## What
Least Privilege means users, roles, services, and components should only have the access needed to complete their legitimate task.

Access should be narrow by default.

## Why it matters
Over-permissioned systems increase the damage from mistakes, account compromise, and implementation bugs.

Least privilege:
- reduces blast radius
- prevents accidental data exposure
- makes roles easier to reason about
- supports safer collaboration
- improves trust in sensitive workflows

The safest permission is the one never granted unnecessarily.

## When to apply
- user roles and teams
- admin tools
- settings and billing
- data exports
- API keys and integrations
- internal dashboards

## How to apply

- define the minimum access needed for each task
- separate view, edit, invite, delete, export, and admin permissions
- make dangerous permissions explicit
- avoid broad default roles
- show permission impact before granting access
- log or confirm high-risk permission changes

Users should understand what access they are granting and why.

## Implementation rules

- default roles must be limited
- admin access must not be granted casually
- permission checks must happen server-side
- hidden UI is not a security boundary
- sensitive permissions must be visible and reviewable
- permission changes must produce clear feedback

## Example

Bad:
- every team member can export customer data
- hiding a delete button is the only protection
- "member" and "admin" are the only roles

Good:
- separate permissions for billing, export, invite, and delete
- server-side authorization checks
- clear access review screens
- explicit confirmation for elevated access

## Fail conditions

- users can access data they do not need
- client-side visibility controls replace authorization
- high-risk roles are granted by default
- permission effects are unclear
- access cannot be audited or reviewed

## Enforcement rule

If access is broader than the task requires, reduce it until the permission boundary is clear and enforceable.
