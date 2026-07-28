---
name: safety-limits
type: rule
description: Human pace, ban-sensitivity, hard limits
---

# Safety & Limits

- Keep automation **human-paced** - rapid-fire actions can trip [[platform-facebook]] bot detection
- No aggressive retries when a page fails; skip and report
- Claude can't watch inboxes 24/7 - coverage comes from the scheduled sweeps
- **Publishing does NOT need approval.** When Breken sends photos + a description, run the full flow (comps deep dive -> price -> optimized listing -> publish to all platforms) and publish without asking. Decided 2026-07-28.
- Still always flagged, never auto-handled: everything in [[edge-case-flags]]
