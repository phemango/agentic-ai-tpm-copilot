# Requirements & Success Criteria

## 1. Purpose

This document defines the functional requirements and success criteria for the Agentic AI TPM Copilot portfolio project.

The requirements focus on demonstrating how Agentic AI can be leveraged to support a human TPM managing an AI project.

---

## 2. Functional Requirements

### AR-001 — Understand TPM Requests

The copilot shall interpret a TPM request and identify:

- Objective
- Desired outcome
- Relevant project lifecycle stage
- Constraints
- Required information
- Required human decisions

---

### AR-002 — Retrieve Project Context

The copilot shall use available project information and artifacts to establish relevant context before performing a multi-step TPM task.

The copilot shall distinguish available evidence from missing information.

---

### AR-003 — Execute Multi-Step TPM Workflows

The copilot shall support multi-step workflows rather than limiting its behavior to a single response.

The general workflow is:

**Understand → Plan → Act → Observe → Analyze → Verify → Report**

---

### AR-004 — Maintain Project Context

The copilot shall maintain relevant project context throughout a workflow, including:

- Requirements
- Milestones
- Dependencies
- Risks
- Issues
- Decisions
- Evidence
- Open actions

Where persistent state is unavailable, the copilot shall clearly identify information that must be supplied again.

---

### AR-005 — Identify Gaps

The copilot shall identify:

- Missing information
- Missing evidence
- Unresolved dependencies
- Project risks
- Issues
- Assumptions
- Decisions requiring human input

---

### AR-006 — Propose Actions

The copilot shall propose practical next actions based on available evidence.

Actions shall not be represented as completed unless supporting evidence exists.

---

### AR-007 — Generate TPM Artifacts

The copilot shall support generation of practical TPM artifacts, including:

- Project charter
- Requirements
- Project plan
- Risk and issue register
- Status report
- Evaluation plan
- Readiness assessment
- Stakeholder communication plan
- Release decision support
- Closure documentation

---

### AR-008 — Maintain Evidence Traceability

Where practical, the copilot shall support the following relationship:

**Requirement → Acceptance Criteria → Evidence → Finding → Recommendation / Decision Option → Human Decision**

---

### AR-009 — Support Evaluation and Readiness

The copilot shall support:

- AI evaluation planning
- Test planning
- Evidence review
- Readiness assessment
- Identification of release gaps
- Preparation of release decision support

The copilot shall not claim that testing or validation occurred unless evidence is available.

---

### AR-010 — Handle Uncertainty

The copilot shall explicitly distinguish:

- **VERIFIED FACT**
- **AGENT ANALYSIS**
- **ASSUMPTION**
- **UNKNOWN / MISSING INFORMATION**
- **HUMAN DECISION**

The copilot shall not convert missing information into an implied fact.

---

### AR-011 — Human Approval

The copilot shall identify decisions requiring human approval.

The copilot shall not independently:

- Approve scope changes
- Accept project risks
- Commit resources
- Change requirements
- Approve production release
- Make the final Go/No-Go decision

---

### AR-012 — Protect Project 1

The copilot shall treat the AI Knowledge Assistant project as read-only project context.

It shall not modify:

- Project 1 code
- Project 1 notebook
- Project 1 repository
- Project 1 deployment
- Project 1 implementation

---

# 3. Success Criteria

### SC-001 — Lifecycle Coverage

The workflow demonstrates support across:

**Initiate → Plan → Execute → Monitor & Control → Evaluate/Release → Close**

---

### SC-002 — Multi-Step Agentic Workflow

The copilot demonstrates:

**Understand → Gather Information → Plan → Act → Observe → Analyze → Verify → Report**

---

### SC-003 — Evidence-Based Output

Important project conclusions and recommendations are grounded in available project evidence.

---

### SC-004 — No Fabricated Evidence

The copilot does not invent:

- Project facts
- Dates
- Metrics
- Test results
- Approvals
- Stakeholder decisions
- Production status

---

### SC-005 — Human Oversight

High-impact project decisions remain with the human TPM and authorized stakeholders.

---

### SC-006 — Project 1 Protection

Project 1 remains unchanged and read-only throughout the portfolio project.

---

### SC-007 — Useful TPM Artifacts

The workflow produces practical artifacts that demonstrate TPM value across the AI project lifecycle.

---

# 4. Requirement-to-Evidence Approach

Requirements should be validated using available evidence.

Example:

| Requirement | Acceptance Evidence | Result |
|---|---|---|
| AR-001 | Agent interprets a TPM request and identifies objective/context | To be demonstrated |
| AR-003 | Multi-step TPM workflow documented and demonstrated | Demonstrated |
| AR-005 | Risks/gaps identified in project artifacts | Demonstrated |
| AR-007 | TPM artifacts produced | Demonstrated |
| AR-008 | Traceability model documented | Demonstrated |
| AR-009 | Evaluation/readiness artifacts produced | Demonstrated as planning workflow |
| AR-010 | Evidence classifications used | Demonstrated |
| AR-011 | Human decision boundaries documented | Demonstrated |
| AR-012 | Project 1 read-only boundary established | Demonstrated |

---

# 5. Important Evidence Limitation

This portfolio project demonstrates the **workflow and governance model**.

It does not claim that the underlying AI Knowledge Assistant has:

- passed production validation,
- met proposed performance thresholds,
- completed security certification,
- received production approval,
- or been released based on this portfolio project.

Those would require actual project evidence.

---

# 6. Human Decision Points

The following remain human decisions:

- Final project scope
- Acceptance criteria approval
- Risk acceptance
- Resource commitments
- Release criteria approval
- Release decision
- Go/No-Go decision
- Final project closure

The AI copilot provides analysis and decision support but does not replace authorized decision makers.
