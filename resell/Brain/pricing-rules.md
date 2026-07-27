---
name: pricing-rules
type: rule
description: List price, auto-accept, floor, drop schedule
---

# Pricing Rules (edit these!)

- Default list price: ~90% of median sold-comp price (priced to move)
- Auto-accept: offers within 15% of asking = say yes
- Lowball floor: never below 60% of asking without checking with Breken → below-floor goes to [[edge-case-flags]]
- Stale threshold: drop price 10% if no messages after 10 days

Used by [[prompt-inbox-sweep]] and [[prompt-repricing]].
