# Academiaai AI Voicebot — Team SDE 2

**Repository:** `SDE-intern`  
**Engineer:** Karthik N M (`karthiknm8050@gmail.com`)  
**Assigned Workstream:** W4 — Agentic Workflow Engine  

---

## Project Overview

This repository contains the end-to-end implementation of the **Academiaai AI Voicebot** for **Team SDE 2**. 

### Workstream W4 (Agentic Workflow) Deliverables
- **Days 1–2:** 
  - Schemas: `WorkflowPlan`, `WorkflowStep`, `ToolSpec`, `ApprovalRequest`, `WorkflowResult`
  - Lifecycle Enums: `WorkflowState`, `RiskLevel`, `ApprovalStatus`, `StepStatus`, `ToolFailureBehavior`
  - Engine: `WorkflowStateMachine` with transition validation, audit trail, and automatic approval enforcement for consequential actions.
  - Tests: Comprehensive test suite covering valid/invalid transitions and schema constraints.

---

## Directory Structure

```text
projects/
└── sde-2-voicebot/
    ├── src/
    │   ├── __init__.py
    │   └── workflow/
    │       ├── __init__.py
    │       ├── schemas.py
    │       ├── state_machine.py
    │       └── README.md
    └── tests/
        ├── __init__.py
        └── test_workflow_schemas_and_sm.py
```

---

## Running Tests

```bash
cd projects/sde-2-voicebot
$env:PYTHONPATH="."
python -m pytest tests -v
```
