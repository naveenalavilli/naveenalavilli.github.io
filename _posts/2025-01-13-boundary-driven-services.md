---
layout: post
title: "Boundary-Driven Services: Drawing the Right Lines"
date: 2025-01-13 09:00:00 -0500
categories: architecture
---

When a system starts to grow, the first architectural question is not "microservices or monolith". It is "where are the seams". Strong boundaries reduce cognitive load, keep teams autonomous, and avoid hidden coupling.

Key ideas I use when sketching boundaries:

- **Business capability first**: align services to stable business capabilities, not to current org charts or tech stacks.
- **Own your data**: each boundary should own its data model and expose only what others need.
- **Optimize for change**: boundaries should isolate high-churn areas so change does not cascade.
- **Design for failure**: assume downstream failure and define explicit contracts, timeouts, and retries.

A good boundary usually shows up as a sentence that starts with "the system should allow...". If the sentence is too broad, split. If it is too narrow, merge.
