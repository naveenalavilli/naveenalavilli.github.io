---
layout: post
title: "Event Streams: Design for the Read You Need"
---

Event streams are powerful, but the schema you choose determines whether
reads are delightful or painful.

## Two design heuristics

1. Emit events that represent business facts, not database actions.
2. Optimize events for downstream reads, not for producer convenience.

## Practical example

Instead of `OrderUpdated`, emit `OrderPlaced`, `OrderCancelled`, and `OrderShipped`.
The first is an action on a database row; the others are facts that can drive
notifications, analytics, and workflows without joins.

## A warning

Streams are not free logs. You are designing an API. Treat it like one:
version events, document semantics, and publish a changelog.
