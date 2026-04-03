---
title: "Render Cost Defaults"
description: "Supporting reference for Next.js Performance And Render Cost."
slug: "packs/nextjs/nextjs-performance-and-render-cost/references/render-cost-defaults"
sidebar:
  hidden: true
---
> Pack: [`nextjs`](/packs/nextjs/)
> Parent skill: [Next.js Performance And Render Cost](/packs/nextjs/nextjs-performance-and-render-cost/)
> Source: [`nextjs/nextjs-performance-and-render-cost/references/render-cost-defaults.md`](https://github.com/andrewsrigom/agent-skills/blob/main/nextjs/nextjs-performance-and-render-cost/references/render-cost-defaults.md)
## Cheapest default path

- server-first route
- narrow client islands
- cached or static data when possible
- minimal root providers
- delayed or removed third-party scripts

## Most common expensive mistakes

- large `'use client'` trees
- dynamic routes without a product reason
- providers or stateful wrappers at the app root
- shipping large browser-only SDKs to every route
