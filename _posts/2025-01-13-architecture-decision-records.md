---
layout: post
title: "Architecture Decision Records That Age Well"
categories: architecture
tags: [adr, decisions, documentation]
---

Architecture Decision Records (ADRs) are most useful when they capture the trade-offs that *felt risky* at the time.
A good ADR is short, biased toward context, and explicit about what you are **not** doing.

## When to write an ADR
- A decision changes the direction of a system or team.
- The decision has a long half-life (months or years).
- The decision has multiple plausible alternatives.

## A lightweight ADR template
1. **Context**: What is happening now? What constraints matter?
2. **Decision**: What did we choose?
3. **Alternatives**: What else was considered and why not?
4. **Consequences**: What are the trade-offs we accept?

## Make ADRs durable
- Link to telemetry or incident evidence when possible.
- Avoid internal code names that expire quickly.
- Revisit ADRs after 1-2 releases to confirm the decision still stands.

ADRs are less about governance and more about preserving intent. That makes them powerful onboarding tools and a reliable map of architectural evolution.
