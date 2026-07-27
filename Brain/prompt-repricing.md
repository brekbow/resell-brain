---
name: prompt-repricing
type: prompt
description: Every-3-days repricing pass on stale listings
---

# Repricing Pass (every 3 days, 9am)

Governed by [[pricing-rules]], [[autonomy-mode]], [[safety-limits]].

Steps each run:
1. Open [[inventory-tracker]]. Find active listings and days since listing / last price change.
2. Items with no buyer messages past the stale threshold in [[pricing-rules]] → compute new price per the drop rule.
3. For the 2–3 stalest items, quick comp check (eBay sold listings) and go lower if comps say it still won't move in 2–3 weeks.
4. Via Claude in Chrome, update the live price on [[platform-facebook]], [[platform-depop]], [[platform-grailed]]. Human pace.
5. Record new prices + date in [[inventory-tracker]].
6. Never price below the lowball floor — flag those instead.

Finish with a summary: repriced (old → new), items at floor needing Breken, failures.
