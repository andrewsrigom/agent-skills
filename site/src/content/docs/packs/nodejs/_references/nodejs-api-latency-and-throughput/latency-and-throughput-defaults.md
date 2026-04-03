---
title: "Latency And Throughput Defaults"
description: "Supporting reference for Node.js API Latency And Throughput."
slug: "packs/nodejs/nodejs-api-latency-and-throughput/references/latency-and-throughput-defaults"
sidebar:
  hidden: true
---
> Pack: [`nodejs`](/packs/nodejs/)
> Parent skill: [Node.js API Latency And Throughput](/packs/nodejs/nodejs-api-latency-and-throughput/)
> Source: [`nodejs/nodejs-api-latency-and-throughput/references/latency-and-throughput-defaults.md`](https://github.com/andrewsrigom/agent-skills/blob/main/nodejs/nodejs-api-latency-and-throughput/references/latency-and-throughput-defaults.md)
## High-leverage first checks

- per-request client construction
- repeated config or schema parsing
- N+1 remote calls
- oversized response payloads
- unbounded parallel work

## Default priorities

1. tail latency
2. repeated setup cost
3. I/O amplification
4. bounded concurrency
5. CPU hotspots

## Rule

Do not trade observability, cancellation, and correctness for benchmark theater.
