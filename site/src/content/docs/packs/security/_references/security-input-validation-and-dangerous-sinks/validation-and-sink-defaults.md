---
title: "Validation And Sink Defaults"
description: "Supporting reference for Security Input Validation And Dangerous Sinks."
slug: "packs/security/security-input-validation-and-dangerous-sinks/references/validation-and-sink-defaults"
sidebar:
  hidden: true
---
> Pack: [`security`](/packs/security/)
> Parent skill: [Security Input Validation And Dangerous Sinks](/packs/security/security-input-validation-and-dangerous-sinks/)
> Source: [`security/security-input-validation-and-dangerous-sinks/references/validation-and-sink-defaults.md`](https://github.com/andrewsrigom/agent-skills/blob/main/security/security-input-validation-and-dangerous-sinks/references/validation-and-sink-defaults.md)
## Match the protection to the sink

- SQL -> parameterized queries
- HTML -> output-context escaping or sanitization
- shell -> no interpolation, structured args only
- filesystem -> fixed roots and allowlisted names
- redirect or URL fetch -> allowlists and scheme checks

## Default rule

If you cannot name the dangerous sink, you are probably validating too vaguely.
