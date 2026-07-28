---
name: workflow-sold
type: workflow
description: "Stage 4: label, tracker, delist everywhere"
---

# Stage 4 - Sold

On a sale (found by [[prompt-inbox-sweep]] or reported by Breken):
- Get + print the shipping label: prepaid on [[platform-depop]] / [[platform-grailed]]; on [[platform-ebay]] buy it through eBay's shipping flow
- Update [[inventory-tracker]]: Sold, date, platform, price
- Delist from ALL other platforms
- Photos move to 04_Sold
- Alert Breken per trigger 1 in [[notifications]]
