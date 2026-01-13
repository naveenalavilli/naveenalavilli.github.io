---
layout: post
title: "Layered Architecture Without the Ceremony"
categories: architecture
tags: [layers, modularity, boundaries]
---

Layering is still one of the fastest ways to control complexity, but strict layer rules can slow teams down.
The goal is to create boundaries that are clear, testable, and adaptable.

## A pragmatic layer set
- **API layer**: Handles transport concerns (HTTP, gRPC), auth, and request shaping.
- **Application layer**: Orchestrates use cases, transactions, and workflows.
- **Domain layer**: Contains business rules and invariants.
- **Infrastructure layer**: Adapters for data stores, queues, or external services.

## Rules that keep it simple
- Dependencies point inward (API -> App -> Domain).
- Only the application layer talks to infrastructure.
- Domain objects have no knowledge of transport or persistence.

## When to bend the rules
- Performance hot paths may justify a read model shortcut.
- Integrations might need a pragmatic adapter in the API layer.

Layered architecture works best when it is treated as a tool, not a ritual.
