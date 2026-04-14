---
artifact_type: product-brief
lane: planning
status: defined
owner: MComee
dependencies:
  - mission
---

# Summary
CPF Console is a desktop-first graphical interface for inspecting and operating Control Plane Framework repositories.

# Problem statement
Framework-governed projects are currently easiest to use through raw files, YAML/Markdown artifacts, and command-line validators. This makes the framework harder to understand, harder to demonstrate, and less accessible than it should be.

# Intended users
- developers using Control Plane Framework
- technical reviewers evaluating CPF-governed repositories
- solo builders who want a visual operator surface

# Primary use cases
- inspect planning, governance, execution, and validation artifacts
- visualize artifact state and dependency relationships
- run repository validation from a UI
- show pass/fail results and surface actionable issues
- demonstrate the framework in operation for portfolio and hiring purposes

# Desired outcomes
- a reviewer can understand the framework workflow without reading raw files only
- a user can trigger validation from the UI and see results clearly
- artifact status and dependency chains are visible at a glance

# Success metrics
- CPF Console can load a CPF-style repository locally
- CPF Console can surface artifact metadata and state
- CPF Console can invoke the canonical Python validator
- CPF Console can display validation results and dependency information

# Non-goals
- replacing GitHub workflows
- replacing the framework contract or Python validators
- multi-user cloud sync in v1
- embedded autonomous agent execution in v1

# Assumptions
- Flutter desktop is the right initial UI stack
- Python remains the enforcement engine
- CPF Console is a project-layer application built using the framework, not a rewrite of the framework itself

# Open questions
- how tightly UI state should mirror artifact lifecycle states
- whether graph rendering is a v1 requirement or v1.5 enhancement
- how validator output should be normalized for UI consumption
