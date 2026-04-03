---
title: "Default Review Map"
description: "Supporting reference for Security Default Review For Web Apps."
slug: "packs/security/security-default-review-for-web-apps/references/default-review-map"
sidebar:
  hidden: true
---
> Pack: [`security`](/packs/security/)
> Parent skill: [Security Default Review For Web Apps](/packs/security/security-default-review-for-web-apps/)
> Source: [`security/security-default-review-for-web-apps/references/default-review-map.md`](https://github.com/andrewsrigom/agent-skills/blob/main/security/security-default-review-for-web-apps/references/default-review-map.md)
## Start here

- What input can an attacker control?
- What action changes privileged state?
- What secret or sensitive data exists?
- What boundary is assumed trusted but probably is not?

## Most common top risks in app code

1. trusting the client too much
2. server-side authz checks missing or inconsistent
3. untrusted input reaching a dangerous sink
4. secrets or privileged tokens leaking to the browser

## Default rule

Find the strongest exploit path first, not the longest checklist.
