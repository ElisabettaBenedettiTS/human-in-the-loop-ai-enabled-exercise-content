# AI-Assisted Exercise Content Workflow v1.0

## Objective

Provide a repeatable, human-in-the-loop process for using authorised AI-enabled tools to support exercise-content production.

The workflow is designed to ensure that AI-generated or AI-assisted outputs are never treated as approved solely because they were produced by an AI system.

## End-to-End Workflow

### Step 1 — Define the Requirement

**Human-owned activity**

Identify:
- Training Objective
- Desired Training Audience activity
- Exercise phase
- Scenario context
- Actors
- Operational constraints
- Relevant doctrine
- Required output format
- Security considerations

**Output:** Structured content-development requirement.

### Step 2 — Validate Inputs

Before using an AI-enabled tool:
- Confirm the tool is authorised.
- Confirm the information is suitable for that tool.
- Remove or sanitise sensitive information where required.
- Verify that source material is current and approved.
- Identify known information gaps.

**Decision Gate:** If information cannot be processed safely, stop.

### Step 3 — Use a Structured Prompt

The prompt should define:
- Role
- Task
- Training Objective
- Scenario context
- Actors
- Constraints
- Source material
- Prohibited assumptions
- Required output format
- Validation questions

**Core instruction:** If required information is missing, flag the gap rather than inventing an answer.

### Step 4 — Generate AI-Assisted Draft

The AI may support:
- Drafting
- Adaptation
- Translation
- Consistency checking
- Quality assurance
- Review

The AI has no authority to approve content.

### Step 5 — Run Consistency Review

Check for:
- Scenario contradictions
- Timeline conflicts
- Incorrect actor roles
- Duplicate effects
- Unsupported assumptions
- Missing dependencies
- Unrealistic sequencing
- Weak Training Objective linkage
- Excessive information exposure

**Output:** Review findings and issues requiring human attention.

### Step 6 — Human Content Review

The Content Analyst reviews:
- Relevance
- Clarity
- Operational plausibility
- Training value
- Scenario coherence
- Training Audience suitability

The Content Analyst may:
- Accept
- Revise
- Reject
- Escalate to an SME

### Step 7 — SME / Doctrinal Validation

Where required, an appropriate SME validates:
- Doctrine
- Command relationships
- Authorities
- Functional responsibilities
- Operational procedures
- Technical realism

**Important:** AI-generated doctrinal claims are not accepted without verification.

### Step 8 — Security and Responsible-Use Check

Confirm:
- Approved tool used
- No unauthorised sensitive information entered
- Inputs were sanitised where required
- Output does not expose restricted information
- Human reviewer is identified
- Version and provenance are recorded

**Decision Gate:** Any unresolved security concern stops release.

### Step 9 — Final Approval and Release

A designated human authority approves the content for use.

Potential delivery formats:
- Training Audience portal
- Exercise management system
- EXCON product
- HICON communication
- Simulated media item
- SME brief
- Supporting document

AI has no release authority.

### Step 10 — Capture Lessons

Record:
- Prompt version
- Issues detected
- Human corrections
- SME feedback
- Assurance score
- Rework required
- Lessons for next iteration

Use the results to improve:
- Prompt templates
- Review checklists
- User guidance
- Assurance thresholds
- Training materials

## Workflow Summary

```text
Requirement
   ↓
Input Validation
   ↓
Structured Prompt
   ↓
AI-Assisted Draft
   ↓
Consistency Review
   ↓
Human Content Review
   ↓
SME / Doctrinal Validation
   ↓
Security Check
   ↓
Final Human Approval
   ↓
Release
   ↓
Lessons & Improvement
```

## Human Authority Matrix

| Activity | AI | Content Analyst | SME | Final Approver |
|---|---|---|---|---|
| Generate draft | Support | Owns task | — | — |
| Check consistency | Support | Owns review | Support | — |
| Verify doctrine | Flag only | Coordinates | Owns validation | — |
| Assess plausibility | Support | Owns initial judgement | Validates | — |
| Assess security | No authority | Checks | Support | Escalates/approves |
| Release content | None | Recommends | Validates where required | Owns decision |

## Core Principle

**AI may accelerate content production, but judgement, validation, security responsibility, and approval remain human responsibilities.**
