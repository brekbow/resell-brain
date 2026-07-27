---
name: prompt-repricing
type: prompt
description: Repricing pass on stale listings (schedule follows pricing-rules)
---

# Repricing Pass (every 3 days, 9am)

Governed by [[pricing-rules]], [[autonomy-mode]], [[safety-limits]], [[notifications]].

Steps each run:
1. Open [[inventory-tracker]]. Find active listings and days since listing / last price change / last buyer message.
2. Items past the stale threshold in [[pricing-rules]] with no buyer messages -> compute the new price per its drop rule.
3. For the 2-3 stalest items, re-run the comp check (eBay sold listings and platform solds) and go lower if comps say it still won't move in 2-3 weeks.
4. Via Claude in Chrome, update the live price on [[platform-facebook]], [[platform-depop]], [[platform-grailed]]. Human pace per [[safety-limits]]. Refresh/bump listings for free where allowed per [[listing-optimization]].
5. Record new prices + date in [[inventory-tracker]].
6. Never set a price that makes the auto-accept math nonsensical - if an item would need to go below what Breken would plausibly take, alert him per [[notifications]] instead.

Alert Breken ONLY per the 3 triggers in [[notifications]]. Log a run summary: repriced (old -> new), items needing Breken, failures.
