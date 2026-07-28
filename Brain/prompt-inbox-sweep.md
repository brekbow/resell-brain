---
name: prompt-inbox-sweep
type: prompt
description: Every-2h sweep - replies, sales, labels, delisting
---

# Inbox & Sales Sweep (every 2h, 8am-10pm)

Read [[autonomy-mode]], [[pricing-rules]], [[negotiation-defaults]], [[edge-case-flags]], [[safety-limits]], [[notifications]] first - they govern every action below.

Steps each run:
1. Via Claude in Chrome, open [[platform-facebook]], [[platform-depop]], [[platform-grailed]], and [[platform-ebay]] messages in Breken's logged-in Chrome. Human pace per [[safety-limits]], response timing per [[negotiation-defaults]].
2. For each new buyer message, draft and send a reply per the rules (price questions, availability, meetup logistics, offers per the auto-accept threshold in [[pricing-rules]]).
   - If the buyer is actively responding, STAY in the conversation - keep replying at human pace until a natural stop: deal agreed, question answered, or ~10 minutes of silence. Do not fire one reply and leave mid-negotiation.
3. Check for NEW SALES on Depop, Grailed, and eBay: open the order, get the shipping label (prepaid on Depop/Grailed; on eBay buy it through the shipping flow) and print it to the default printer. Update [[inventory-tracker]] (Sold, date, platform, price), then delist from the other platforms -> see [[workflow-sold]].
4. For agreed Facebook local-pickup deals, note meetup details in [[inventory-tracker]].
5. If a platform isn't logged in or won't load, skip and report it - no aggressive retries.

Alert Breken ONLY per the 3 triggers in [[notifications]]. Log a short run summary either way: messages answered, offers accepted, sales processed, labels printed, anything flagged.
