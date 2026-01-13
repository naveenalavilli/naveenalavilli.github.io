---
layout: post
title: "A Practical Checklist for Scalable Architecture"
date: 2025-01-13 11:00:00 -0500
categories: architecture
---

Scalability is rarely a single decision. It is a sequence of trade-offs that add up. Here is a short checklist I review before a big launch.

- **Traffic model**: peak QPS, steady state, and tail spikes.
- **State shape**: what must be consistent, what can be eventual.
- **Cache strategy**: where to cache and how to invalidate.
- **Data partitions**: keys that scale evenly and avoid hotspots.
- **Failure modes**: timeouts, circuit breakers, and graceful degradation.
- **Observability**: traces, metrics, and logs tied to user outcomes.

Most scale problems are solved by removing unnecessary coupling and clarifying ownership.
