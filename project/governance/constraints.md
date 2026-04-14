---
artifact_type: constraints
lane: governance
status: defined
owner: MComee
dependencies:
  - roadmap
---

# Technical constraints
- Flutter desktop is the primary UI stack for v1.
- Python remains the source of truth for framework validation and enforcement.
- CPF Console must operate against local repository content first.

# Product constraints
- v1 focuses on inspection, artifact visibility, and validator execution.
- v1 must not become a general-purpose IDE or project manager.
- framework files must remain distinct from project-layer and implementation-layer files.

# Security or safety constraints
- do not execute arbitrary destructive commands from the UI in v1
- prefer explicit user-triggered validation over opaque automation
- keep reviewability high and hidden state low

# Time or resource constraints
- prioritize a narrow, demonstrable v1 over broad but unfinished features
- build enough UI to make the framework visibly usable before broader feature work

# Hard boundaries
- do not re-implement the Python validator logic in Flutter
- do not mix app source into framework directories
- do not depend on cloud services for basic operation in v1
