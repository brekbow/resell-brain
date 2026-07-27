---
name: notifications
type: rule
description: When to alert Breken - ONLY these 3 triggers
---

# Notifications - the ONLY 3 reasons to alert Breken

1. **Something SOLD** (any platform) -> what sold, price, platform, and what was done (label printed, delisted, tracker updated)
2. **A Facebook buyer wants to meet somewhere** -> item, buyer, proposed time/place, and whether it's the default spot from [[negotiation-defaults]] or needs his approval
3. **Something went WRONG and Breken must act** -> logged-out platform, suspicious buyer, below-floor decision, anything blocking the operation per [[edge-case-flags]]

Everything else: stay silent. No "all quiet" pings, no routine run reports. Quiet runs just log their summary.

Channel: SMS via Quo if connected; otherwise Claude notification + a clearly flagged line at the TOP of the run summary.

Used by [[prompt-inbox-sweep]] and [[prompt-repricing]].
