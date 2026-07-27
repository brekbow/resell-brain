---
name: workflow-sold
type: workflow
description: "Stage 4: label, tracker, delist everywhere"
---

# Stage 4 — Sold

On a sale (found by [[prompt-inbox-sweep]] or reported by Breken):
- Print the platform's prepaid shipping label (Depop/Grailed)
- Update [[inventory-tracker]]: Sold, date, platform, price
- Delist from all other platforms
- Photos move to `04_Sold`
