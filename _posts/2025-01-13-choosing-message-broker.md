---
layout: post
title: "Choosing a Message Broker: A Decision Matrix"
categories: architecture
tags: [messaging, kafka, rabbitmq, nats]
---

Message brokers are less about features and more about operational posture.
Pick the broker that matches your team size, availability needs, and data durability requirements.

## Decision matrix
| Criteria | Kafka | RabbitMQ | NATS |
| --- | --- | --- | --- |
| Throughput | Very high | High | High |
| Ordering | Partitioned | Queue-based | Subject-based |
| Persistence | Strong | Optional | Optional |
| Ops complexity | High | Medium | Low |

## Heuristics
- If you need replayable event streams, Kafka is the default.
- If you need flexible routing and quick setup, RabbitMQ is dependable.
- If you need low-latency pub/sub with simple ops, NATS shines.

No broker is perfect. The best one is the one your team can operate confidently.
