---
title: "Render Cost And State Boundaries"
description: "Supporting reference for React Render Performance And State Boundaries."
slug: "packs/react/react-render-performance-and-state-boundaries/references/render-cost-and-state-boundaries"
sidebar:
  hidden: true
---
> Pack: [`react`](/packs/react/)
> Parent skill: [React Render Performance And State Boundaries](/packs/react/react-render-performance-and-state-boundaries/)
> Source: [`react/react-render-performance-and-state-boundaries/references/render-cost-and-state-boundaries.md`](https://github.com/andrewsrigom/agent-skills/blob/main/react/react-render-performance-and-state-boundaries/references/render-cost-and-state-boundaries.md)
## Default order of attack

1. Identify the state change
2. Reduce who depends on it
3. Split hot and cold UI
4. Re-measure
5. Memoize only if needed

## Good default boundaries

- local form state stays local
- hover and open state stay near the interactive component
- expensive lists get isolated from unrelated page state
- providers stay narrow when their values change often

## Bad default boundaries

- root-level client state for one local interaction
- large providers wrapping the app for frequently changing values
- derived state copied into multiple components
