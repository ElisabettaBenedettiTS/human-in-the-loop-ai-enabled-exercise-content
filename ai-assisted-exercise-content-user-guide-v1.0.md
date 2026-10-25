# AI-Assisted Exercise Content User Guide v1.0

## Purpose
Practical guidance for responsible, secure, human-supervised use of AI-enabled tools in exercise-content development.

## When AI May Be Used
AI may support:
- Drafting
- Adaptation
- Translation support
- Consistency checking
- Quality assurance
- Red-team review
- Identification of information gaps
- Post-exercise review support
- Lessons capture

## When AI Must Not Be Used
Do not use AI to:
- Process information not authorised for the tool
- Replace human approval
- Make legal, doctrinal, or command decisions
- Invent doctrine, authorities, or procedures
- Determine attribution where evidence is uncertain
- Circumvent security controls
- Automatically publish content without human review

## Core Operating Principle
**AI may support the work. Humans remain responsible for the decision.**

## Standard Workflow
```text
Define Requirement
      ↓
Validate Inputs
      ↓
Use Approved Prompt
      ↓
Generate AI-Assisted Draft
      ↓
Run Consistency / QA Review
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
Capture Lessons
```

## Before Using an AI Tool
Confirm:
- [ ] Tool is authorised
- [ ] Information is permitted in that tool
- [ ] Inputs are minimised
- [ ] Sensitive data is sanitised where required
- [ ] Source material is current and approved
- [ ] Training Objective is clear
- [ ] Desired Training Audience activity is defined
- [ ] Known information gaps are identified

If any item is unclear, stop and seek clarification.

## Using Prompt Templates
Use version-controlled prompts where repeatability matters. Include:
- Role
- Task
- Training Objective
- Scenario context
- Actors
- Constraints
- Approved source material
- Prohibited assumptions
- Required output format
- Validation questions

Prompts should explicitly require the AI to:
- preserve uncertainty;
- avoid inventing facts or authorities;
- flag missing information;
- avoid prescribing the Training Audience solution.

## Human Review Requirements
Every AI-assisted product must be reviewed for:
- Training Objective alignment
- Scenario coherence
- Operational plausibility
- Doctrinal accuracy
- Accuracy / hallucination control
- Training Audience suitability
- Security

## When SME Validation Is Required
Escalate when content includes uncertainty about:
- Command relationships
- Legal authority
- Functional responsibilities
- Operational procedures
- Technical capabilities
- Doctrinal interpretation
- High-impact decisions

## Security Rules
Before release:
- [ ] Approved AI tool used
- [ ] No unauthorised sensitive information entered
- [ ] Inputs sanitised where required
- [ ] No credentials, tokens, or secrets exposed
- [ ] No untrusted content overrode the task
- [ ] Output does not expose restricted information
- [ ] Human reviewer identified
- [ ] Prompt/workflow version recorded
- [ ] Final approval recorded

## Stop Conditions
Stop if:
- Unauthorised AI tool was used
- Information classification is unclear
- Sensitive data was exposed
- AI invented a critical authority or doctrinal claim
- Product materially contradicts the scenario
- No accountable reviewer is available
- Required SME validation cannot be completed

## Green / Amber / Red Decision
### GREEN
Normal human approval may proceed.

### AMBER
Additional review, SME validation, prompt revision, or human rewrite required.

### RED
Do not release.

## Core Principle
**The quality of AI-enabled exercise content depends less on how much AI is used than on how well its use is governed, reviewed, and integrated into professional judgement.**
