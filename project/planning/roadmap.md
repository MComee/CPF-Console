---
artifact_type: roadmap
lane: planning
status: defined
owner: MComee
dependencies:
  - mission
  - product-brief
---

# Horizon 1: immediate work
- establish CPF Console project artifacts
- define canonical repository structure for framework + project + work layers
- scaffold Flutter desktop application
- define validator integration path
- implement basic repository loader and artifact metadata reader

# Horizon 2: near-term work
- display artifact list by lane
- display artifact state and metadata
- invoke Python validator from UI
- show validation results in a usable inspection panel
- add project summary/dashboard view

# Horizon 3: longer-term work
- add dependency graph visualization
- add richer issue navigation and remediation guidance
- support configurable project paths and multiple CPF-style repositories
- refine review/demo experience for hiring and portfolio presentation

# Dependencies
- Control Plane Framework remains intact and available as governing system
- project-layer artifacts are maintained in this repository
- Flutter desktop application scaffold exists under work/app/
- Python validator invocation strategy is defined

# Risks
- duplicating validation logic in Flutter instead of calling Python
- muddying framework files with app-specific implementation
- over-scoping v1 into IDE-like behavior
- weak UX around validator output if output is not normalized
