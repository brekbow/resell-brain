---
name: pricing-rules
type: rule
description: Deep-dive comps, 90% start, 85% auto-accept floor, 7-day drops
---

# Pricing Rules (edit these!)

## Before listing - ALWAYS
- DEEP DIVE every single item before it lists: sold comps (eBay sold listings, Depop/Grailed solds) for the same brand/model/size/condition. Real recent sale prices, not asking prices. No listing goes up without this research.
- Breken gives a brief description and a price estimate -> his estimate is NOT firm. Find the true market anchor yourself. The goal is to MOVE items; they have no value to him sitting unsold.

## Numbers
- List price: 90% of the median sold-comp market price (fair, priced to move)
- Auto-accept: any offer at 85% or more of the list price -> accept
- Below 85% of list: NEVER auto-accept -> alert Breken per [[notifications]] with the offer, wait for his yes/no
- Price drop: -10% after 7 days with no buyer messages, then re-check comps per [[prompt-repricing]]

Used by [[prompt-inbox-sweep]] and [[prompt-repricing]]. Listing flow: [[workflow-process-items]] + [[listing-optimization]].
