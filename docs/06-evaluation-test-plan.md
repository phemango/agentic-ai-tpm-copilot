# AI Evaluation & Test Plan

## 1. Purpose

This document defines how the example AI project could be evaluated before production release.

The plan demonstrates how the Agentic AI TPM Copilot can help a TPM define evaluation objectives, test coverage, evidence requirements, risks, and release criteria.

No actual test results are claimed by this portfolio project.

---

# 2. Evaluation Objectives

The evaluation should determine whether the AI system:

- Produces useful responses for intended use cases.
- Grounds answers in available project knowledge.
- Provides appropriate supporting evidence or citations where applicable.
- Handles unknown or unsupported questions appropriately.
- Resists common adversarial inputs.
- Protects sensitive information.
- Meets agreed performance expectations.
- Provides an acceptable user experience.

---

# 3. Evaluation Dimensions

| Dimension | Evaluation Focus |
|---|---|
| Functional Quality | Does the system perform its intended functions? |
| Answer Quality | Are responses accurate, relevant, and useful? |
| Groundedness | Are answers supported by available evidence? |
| Retrieval / Evidence | Is relevant information identified and used? |
| Citation Quality | Can users trace important claims to supporting evidence? |
| Safety / Security | Does the system resist inappropriate or malicious inputs? |
| Privacy | Does the system protect sensitive information? |
| Performance | Does response time meet agreed expectations? |
| User Experience | Can intended users effectively use the system? |

---

# 4. Evaluation Dataset

A representative evaluation dataset should be established before formal evaluation.

The dataset should include categories such as:

- In-scope factual questions
- Questions requiring information from multiple sources
- Unanswerable or out-of-scope questions
- Ambiguous questions
- Edge cases
- Adversarial or security-related prompts

A proposed starting point is approximately **100–150 evaluation cases**.

This number is a proposed planning target, not an established project requirement.

The final dataset size and composition should be confirmed by the appropriate human stakeholders.

---

# 5. Test Categories

## TC-01 — Functional Testing

Validate that intended system functions operate correctly.

Examples:

- User submits a supported request.
- System processes the request.
- System returns an appropriate response.
- Expected supporting information is available when applicable.

**Evidence:** Test execution results and documented findings.

---

## TC-02 — AI Quality Evaluation

Evaluate response quality using representative questions.

Potential measures include:

- Answer correctness
- Relevance
- Groundedness / faithfulness
- Completeness
- Citation accuracy

Any formal thresholds must be approved before they become release criteria.

---

## TC-03 — Adversarial / Security Testing

Evaluate behavior under potentially unsafe or malicious inputs.

Examples include:

- Direct prompt injection
- Indirect prompt injection
- Attempts to bypass instructions
- Attempts to access restricted information
- Attempts to cause unauthorized actions

Security findings should be reviewed by appropriate human stakeholders.

---

## TC-04 — Privacy / Data Boundary Testing

Validate that the system respects intended information boundaries.

Testing should consider:

- Sensitive information
- Personal information
- Unauthorized information requests
- Access-control boundaries
- Information leakage through generated responses

A zero-tolerance requirement for specific types of sensitive-data exposure may be proposed where appropriate, but formal acceptance criteria require human approval.

---

## TC-05 — Performance Testing

Evaluate system responsiveness under representative usage.

Potential measurements include:

- Response latency
- Percentile latency
- Time to first response
- Throughput
- Resource consumption

Actual performance targets should be defined and approved before testing.

---

## TC-06 — Human / SME Validation

Appropriate subject-matter experts should review representative outputs.

Human reviewers may assess:

- Correctness
- Relevance
- Usefulness
- Evidence quality
- Appropriate handling of uncertainty

Human validation should supplement automated evaluation rather than being replaced by it.

---

## TC-07 — User Acceptance Testing

A representative pilot group may evaluate the system in realistic scenarios.

Potential feedback areas include:

- Ease of use
- Trust
- Usefulness
- Response quality
- Workflow fit
- Missing capabilities

Pilot results should be documented as evidence before being used in release decisions.

---

# 6. Proposed Metrics

Potential metrics include:

| Metric | Purpose |
|---|---|
| Answer Correctness | Measures factual correctness |
| Groundedness / Faithfulness | Measures whether answers are supported by evidence |
| Context Recall | Measures whether relevant information was retrieved |
| Context Precision | Measures relevance of retrieved information |
| Citation Accuracy | Measures whether citations support claims |
| Refusal Accuracy | Measures appropriate handling of unsupported requests |
| Security Test Pass Rate | Measures results of defined security tests |
| Privacy Leakage | Measures unintended exposure of sensitive information |
| Response Latency | Measures system responsiveness |
| User Satisfaction | Measures user-perceived usefulness |

These metrics are proposed evaluation measures.

They are not actual results.

---

# 7. Proposed Release Thresholds

Thresholds should be established by the appropriate human stakeholders based on business requirements, risk tolerance, and intended use.

Illustrative examples may include:

- High-quality answer performance above an agreed threshold.
- Strong evidence grounding.
- High citation validity.
- Appropriate refusal of unsupported questions.
- No unacceptable sensitive-data leakage.
- Security controls passing required tests.
- Performance meeting agreed service expectations.
- Acceptable user feedback during validation.

Numeric thresholds should not become formal release criteria until approved.

---

# 8. Evaluation Evidence

Each evaluation should produce traceable evidence.

Example:

```text
Requirement
    ↓
Acceptance Criterion
    ↓
Test Case
    ↓
Test Result
    ↓
Finding
    ↓
Risk / Issue
    ↓
Recommendation
    ↓
Human Decision
