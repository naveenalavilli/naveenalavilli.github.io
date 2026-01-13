---
layout: post
title: "Architecture Is Trade-offs, Not Checklists"
---

Most architecture debates collapse into preferences because the trade-offs are not made explicit.
A design is only good relative to a context: latency targets, team size, failure tolerance,
and the cost of change.

## A simple framing

Start with three axes:

- Change velocity: How often do you expect business rules to change?
- Operational risk: What is the blast radius of a failure?
- Cost envelope: What ongoing spend is acceptable?

Every pattern (microservices, event-driven, modular monoliths) is just a point in this space.
Make the axes visible and your decisions get easier to defend.

## A practice that works

When proposing a design, include a one-paragraph "no-go" case:

- If feature churn is low, a monolith is cheaper.
- If data consistency is critical, avoid asynchronous flows.
- If the team is small, centralize ownership.

This turns architecture into a shared decision instead of a religious argument.
