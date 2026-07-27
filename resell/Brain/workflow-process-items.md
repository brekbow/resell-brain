---
name: workflow-process-items
type: workflow
description: "Stage 2: clean photos, comps, price, write listing"
---

# Stage 2 — Process Items

Say **"process new items"**. Claude:
- Cleans photos (background, crop, brighten) → `02_Processed_Photos`
- Asks for details it can't see (size, brand, flaws, cost)
- Researches sold comps, proposes a price per [[pricing-rules]]
- Writes title + description
- Adds the item to [[inventory-tracker]]

Next → [[workflow-listing]]
