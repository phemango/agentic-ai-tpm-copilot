
# Risk & Issue Register

## 1. Purpose

This register identifies key risks, issues, assumptions, and dependencies relevant to the Agentic AI TPM Copilot portfolio project and the example AI project it is managing.

The register supports proactive TPM risk management and demonstrates how Agentic AI can help identify, analyze, and track project uncertainty.

---

# 2. Risk Management Approach

Risks are assessed based on:

- Potential impact
- Likelihood
- Evidence available
- Mitigation approach
- Human decision requirements

The AI copilot may identify and analyze risks, but risk acceptance remains a human decision.

---

# 3. Risk Register

| ID | Risk | Description | Potential Impact | Mitigation / Response | Status |
|---|---|---|---|---|---|
| RSK-01 | AI Answer Quality | AI-generated answers may contain unsupported or incorrect information. | Reduced user trust or incorrect decisions. | Use evaluation datasets, evidence checks, citations, and human validation. | Open |
| RSK-02 | Retrieval Quality | Relevant information may not be retrieved or may be incomplete. | Incorrect or incomplete answers. | Evaluate retrieval behavior and identify gaps in available evidence. | Open |
| RSK-03 | Data Processing Quality | Information may lose context or structure during ingestion or processing. | Reduced answer quality or missing information. | Validate representative source material and processing behavior. | Open |
| RSK-04 | Knowledge Staleness | Project or source information may become outdated or conflicting. | Outdated recommendations or decisions. | Establish ownership, update processes, and source validation. | Open |
| RSK-05 | Access / Data Boundary | Users or AI workflows may access information outside the intended project boundary. | Confidentiality or governance risk. | Apply access controls, read-only boundaries, and validation. | Open |
| RSK-06 | Prompt Injection | Malicious or unintended instructions may influence AI behavior. | Unsafe or unauthorized behavior. | Perform adversarial testing and establish guardrails. | Open |
| RSK-07 | Sensitive Data Exposure | Sensitive or personal information may be exposed through AI inputs or outputs. | Privacy or compliance risk. | Minimize sensitive data, apply controls, and perform validation. | Open |
| RSK-08 | Citation / Evidence Trust | Users may not be able to determine whether an answer is supported by evidence. | Reduced trust and decision quality. | Require evidence traceability and citation validation where applicable. | Open |
| RSK-09 | User Expectations | Users may assume the AI is more authoritative or autonomous than intended. | Incorrect reliance on AI output. | Clearly communicate AI limitations and maintain human decision gates. | Open |
| RSK-10 | Performance | AI response time may not meet user expectations under realistic workloads. | Reduced usability. | Define performance criteria and execute appropriate testing. | Open |
| RSK-11 | AI Usage Cost | AI usage may create unexpected or increasing operational costs. | Budget or scalability concerns. | Monitor usage assumptions and establish cost expectations. | Open |
| RSK-12 | Evaluation Coverage | Evaluation may not adequately represent real user questions or failure modes. | False confidence in system quality. | Develop representative evaluation cases and include adversarial/unanswerable cases. | Open |

---

# 4. Risk Response Categories

Each risk may be addressed through one or more of:

- Avoid
- Mitigate
- Transfer
- Accept
- Monitor

Risk acceptance requires an authorized human decision.

---

# 5. Issues

Issues represent known conditions requiring action rather than potential future events.

| ID | Issue | Impact | Required Action | Status |
|---|---|---|---|---|
| ISS-01 | Project requirements and acceptance criteria require formal confirmation. | Release/evaluation criteria may remain ambiguous. | Confirm requirements and acceptance criteria. | Open |
| ISS-02 | Actual evaluation results are not available. | Release readiness cannot be established from evaluation evidence. | Execute planned evaluation. | Open |
| ISS-03 | Security/privacy validation results are not available. | Security readiness cannot be fully assessed. | Complete appropriate validation. | Open |
| ISS-04 | Performance/reliability evidence is not available. | Performance readiness cannot be established. | Execute appropriate testing. | Open |
| ISS-05 | Some project ownership, schedule, and resource information is undefined. | Planning and accountability may remain incomplete. | Confirm ownership and project planning information. | Open |

---

# 6. Assumptions

The following are treated as assumptions or items requiring confirmation rather than verified facts:

- Appropriate project documentation will be available for review.
- Relevant stakeholders can provide required project information.
- Evaluation criteria can be agreed upon by authorized stakeholders.
- Appropriate testing can be performed when required.
- The AI copilot will operate within defined access and governance boundaries.
- Proposed metrics or thresholds will require human confirmation before becoming formal release criteria.

---

# 7. Dependencies

Important dependencies include:

- Approved requirements
- Relevant project evidence
- Stakeholder participation
- Evaluation criteria
- Test execution
- Security/privacy review
- Operational readiness information
- Human approval

A dependency should not be considered complete without supporting evidence.

---

# 8. Risk Escalation

The AI copilot should escalate a risk when:

- Potential impact is significant.
- Required evidence is missing.
- A decision requires human authorization.
- A risk affects security or privacy.
- A risk could affect release readiness.
- A mitigation requires resources or scope changes.

The copilot should present:

1. Evidence
2. Risk analysis
3. Potential impact
4. Proposed response
5. Human decision required

---

# 9. Risk Traceability

Where practical:

**Requirement → Risk → Evidence → Finding → Mitigation → Human Decision**

Example:

```text
Requirement:
Provide trustworthy AI responses
        ↓
Risk:
Unsupported AI answer
        ↓
Evidence:
Evaluation results / source evidence
        ↓
Finding:
Evidence insufficient or quality issue identified
        ↓
Mitigation:
Additional evaluation / remediation
        ↓
Human Decision:
Approve mitigation or accept remaining risk
