---
artifact_type: mission
lane: planning
status: defined
owner: MComee
dependencies: []
---

# Project name
CPF Console

# One-sentence mission
Build a graphical operator console that makes Control Plane Framework repositories understandable, navigable, and usable through a structured UI.

# Problem being solved
Control Plane Framework is powerful but repository- and document-centric. Using it directly through raw files and command-line validation creates friction and hides the control-plane state from the user.

# Intended users
Developers, technical leads, and operators using Control Plane Framework or evaluating framework-governed projects.

# Target outcome
A Flutter-based desktop-first interface that can inspect a CPF-style repository, visualize artifact state and dependencies, trigger validation, and guide the user through the framework workflow.

# Non-goals
- replacing the Python validation engine
- turning CPF Console into a generic IDE
- building a cloud collaboration platform in v1
- adding autonomous code generation in v1

# Initial assumptions
- Control Plane Framework remains the governing system
- Python validators remain the source of truth for enforcement
- CPF Console will act as the operator interface over framework artifacts
- the first supported use case is local repository inspection and validation

# Open questions
- how Python validator output should be surfaced in the UI
- whether dependency visualization should be static or interactive in v1
- whether project artifacts should live under `project/` or configurable paths in later versions
