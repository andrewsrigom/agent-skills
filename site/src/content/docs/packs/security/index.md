---
title: "security"
description: "4 skills in the security pack."
sidebar:
  label: "Overview"
  order: 0
---
> Pack path: `security/`

## Skills

- [Security Authz And Trust Boundaries](/packs/security/security-authz-and-trust-boundaries/) — Use when the real security question is whether the current actor is allowed to do the thing, not whether they are merely authenticated. Covers server-side authorization, ownership checks, tenant boundaries, role use, and avoiding trust in user-controlled identifiers.
- [Security Client Server Boundary And Secret Exposure](/packs/security/security-client-server-boundary-and-secret-exposure/) — Use when a web app risks exposing secrets or privileged behavior across the client-server boundary. Covers server-only logic, public env variables, scoped tokens, browser trust assumptions, and moving sensitive work out of the client.
- [Security Default Review For Web Apps](/packs/security/security-default-review-for-web-apps/) — Use when reviewing a web app for practical security risk before coding or shipping. Covers trust boundaries, attacker-controlled input, privileged actions, secret exposure, and routing the problem to narrower security skills without pretending to do a full security audit.
- [Security Input Validation And Dangerous Sinks](/packs/security/security-input-validation-and-dangerous-sinks/) — Use when untrusted input may reach SQL, HTML, filesystem, shell, redirects, or other dangerous sinks. Covers validation, normalization, parameterization, output encoding, and refusing vague “sanitize everything” advice.
