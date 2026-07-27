---
name: prompt-inbox-sweep
type: prompt
description: Every-2h sweep — replies, sales, labels, delisting
---

# Inbox & Sales Sweep (every 2h, 8am–10pm)

Read [[autonomy-mode]], [[pricing-rules]], [[negotiation-defaults]], [[edge-case-flags]], [[safety-limits]] first — they govern every action below.

Steps each run:
1. Via Claude in Chrome, open [[platform-facebook]], [[platform-depop]], and [[platform-grailed]] messages in Breken's logged-in Chrome. Human pace, especially Facebook.
2. For each new buyer message, draft and send a reply per the rules (price questions, availability, meetup logistics, offers within the auto-accept/floor rules).
3. Check for NEW SALES on Depop and Grailed: open the order, print the prepaid shipping label to the default printer, update [[inventory-tracker]] (Sold, date, platform, price), then delist from the other platforms → see [[workflow-sold]].
4. For agreed Facebook local-pickup deals, note meetup details in [[inventory-tracker]].
5. If a platform isn't logged in or won't load, skip and report it — no aggressive retries.

Finish with a short summary: messages answered, offers accepted, sales processed, labels printed, anything flagged.
