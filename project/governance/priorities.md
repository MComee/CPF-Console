---
artifact_type: priorities
lane: governance
status: defined
owner: MComee
dependencies:
  - roadmap
---

# Current top priorities
1. Preserve Control Plane Framework as the governing source of truth.
2. Make CPF Console a usable visual operator console for the framework.
3. Keep v1 scope narrow enough to ship and demonstrate clearly.

# Priority rules
- prefer clarity over feature count
- prefer calling Python validators over duplicating logic in UI
- prefer desktop-first usability over premature cross-platform expansion
- preserve framework/project/work separation at all times

# Escalation criteria
- if UI work begins to replace framework enforcement logic, correct course immediately
- if project scope drifts toward IDE/platform behavior, reduce scope back to inspection and validation
- if validator integration becomes unreliable, treat it as blocking work
