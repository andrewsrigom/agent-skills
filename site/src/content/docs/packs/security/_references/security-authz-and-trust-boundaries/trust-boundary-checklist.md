---
title: "Trust Boundary Checklist"
description: "Supporting reference for Security Authz And Trust Boundaries."
slug: "packs/security/security-authz-and-trust-boundaries/references/trust-boundary-checklist"
sidebar:
  hidden: true
---
> Pack: [`security`](/packs/security/)
> Parent skill: [Security Authz And Trust Boundaries](/packs/security/security-authz-and-trust-boundaries/)
> Source: [`security/security-authz-and-trust-boundaries/references/trust-boundary-checklist.md`](https://github.com/andrewsrigom/agent-skills/blob/main/security/security-authz-and-trust-boundaries/references/trust-boundary-checklist.md)
## Always identify

- who is the actor
- what resource is being touched
- which action is happening
- what server-side fact proves the actor is allowed

## Default checks

- session is valid
- actor belongs to the tenant or org
- actor owns the resource or has explicit privilege
- resource lookup is constrained by tenant or owner where appropriate

## Smells

- `if (isAdmin)` with no resource check
- client sends `userId` and server trusts it
- UI hides buttons but backend allows the mutation
