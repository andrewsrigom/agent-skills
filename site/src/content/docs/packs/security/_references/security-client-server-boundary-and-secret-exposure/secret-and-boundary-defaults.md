---
title: "Secret And Boundary Defaults"
description: "Supporting reference for Security Client Server Boundary And Secret Exposure."
slug: "packs/security/security-client-server-boundary-and-secret-exposure/references/secret-and-boundary-defaults"
sidebar:
  hidden: true
---
> Pack: [`security`](/packs/security/)
> Parent skill: [Security Client Server Boundary And Secret Exposure](/packs/security/security-client-server-boundary-and-secret-exposure/)
> Source: [`security/security-client-server-boundary-and-secret-exposure/references/secret-and-boundary-defaults.md`](https://github.com/andrewsrigom/agent-skills/blob/main/security/security-client-server-boundary-and-secret-exposure/references/secret-and-boundary-defaults.md)
## Server-only by default

- private API keys
- signing keys
- admin credentials
- billing and permission decisions
- internal service-to-service trust

## Public only when intentionally designed that way

- publishable keys
- static feature metadata
- non-sensitive identifiers

## Never trust from the client

- role
- price
- tenant or ownership claims
- hidden form values
- local storage flags
