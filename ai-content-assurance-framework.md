# AI-Assisted Exercise Content Assurance Framework v1.0

## Purpose

This framework provides a structured human-in-the-loop method for reviewing AI-assisted exercise content before it is used in training.

AI-assisted products should be assessed against the same standards expected of non-AI-assisted products.

## 1. Training Objective Alignment

Check whether:
- The content is linked to a defined Training Objective.
- The intended Training Audience activity is clear.
- The content creates a legitimate requirement for analysis, coordination, decision, or action.
- The content contributes to the intended training effect.
- The content avoids prescribing the solution.

**Score**
- 5 — Direct and clear alignment
- 4 — Strong alignment; minor refinement
- 3 — Acceptable; clarification required
- 2 — Weak contribution
- 1 — No credible alignment

## 2. Scenario Coherence

Check whether:
- The content matches approved scenario facts.
- Chronology is correct.
- Actors are used consistently.
- Geographic and organisational relationships are coherent.
- Dependencies are recognised.
- No unsupported scenario facts have been introduced.

**Score**
- 5 — Fully coherent
- 4 — Minor inconsistencies
- 3 — Acceptable with correction
- 2 — Significant inconsistencies
- 1 — Contradicts the scenario

## 3. Operational Plausibility

Check whether:
- The event could credibly occur.
- Actor behaviour is realistic.
- Timing is plausible.
- Cause and effect are credible.
- Capabilities are represented realistically.
- Effects are proportionate.
- The Training Audience receives the right level of information.

**Score**
- 5 — Highly credible
- 4 — Credible; minor refinement
- 3 — Plausible; SME review advised
- 2 — Significant realism concerns
- 1 — Operationally implausible

## 4. Doctrinal Accuracy

Check whether:
- NATO terminology is appropriate.
- Command relationships are correct.
- Authorities are accurately represented.
- Functional responsibilities are correctly assigned.
- Procedures align with approved doctrine or exercise direction.
- AI-generated doctrinal claims have been independently verified.

**Score**
- 5 — Verified and accurate
- 4 — Strong confidence
- 3 — Targeted SME verification required
- 2 — Significant uncertainty
- 1 — Incorrect or unsupported

**Automatic escalation:** Any uncertainty involving command authority, legal authority, rules of engagement, doctrinal responsibilities, or operational command relationships requires human SME validation.

## 5. Accuracy and Hallucination Control

Check whether:
- Factual statements are supported.
- No organisations were fabricated.
- No authorities were fabricated.
- No capabilities were invented.
- No references or documents were fabricated.
- Unsupported assumptions are identified.
- Numerical information is verified.
- AI uncertainty is not presented as fact.

**Score**
- 5 — Verified
- 4 — Minor verification required
- 3 — Several items need checking
- 2 — Significant unsupported content
- 1 — Material hallucination detected

## 6. Security and Responsible Use

Confirm:
- The AI tool was authorised.
- The information was appropriate for that tool.
- No unauthorised classified information was entered.
- Sensitive information was sanitised where required.
- Personal data was handled appropriately.
- Output does not expose unnecessary sensitive information.
- Human review occurred before use.
- Version and reviewer are identifiable.

**Security Assessment**
- GREEN — No identified security concern
- AMBER — Further review required
- RED — Stop; content or process must not proceed

**Critical rule:** Security concerns override numerical scoring.

## 7. Training Audience Suitability

Check whether:
- Language is appropriate.
- Information is clear.
- Content is not unnecessarily leading.
- Required ambiguity is preserved.
- Information exposure is proportionate.
- Delivery format is suitable.
- The product supports the intended training effect.

**Score**
- 5 — Ready for delivery
- 4 — Minor editorial refinement
- 3 — Additional review required
- 2 — Significant delivery concerns
- 1 — Unsuitable for delivery

## Overall Assurance Score

| Area | Score |
|---|---:|
| Training Objective Alignment | /5 |
| Scenario Coherence | /5 |
| Operational Plausibility | /5 |
| Doctrinal Accuracy | /5 |
| Accuracy / Hallucination Control | /5 |
| Training Audience Suitability | /5 |

**Total: /30**

Security is assessed separately.

## Decision Thresholds

### GREEN — 25–30
May proceed through normal human approval if:
- No security concern exists
- No unresolved doctrinal issue remains
- No material hallucination remains
- An accountable human reviewer is identified

### AMBER — 19–24
Additional action required, such as:
- SME validation
- Doctrinal verification
- Scenario correction
- Additional source checking
- Prompt revision
- Human rewrite

### RED — 18 or below
Unsuitable for use in current form.

Required action:
- Reject
- Redevelop
- Rewrite
- Correct underlying inputs before re-running the workflow

## Critical Failure Override

The product is automatically RED if:
- Classified or sensitive information was processed using an unauthorised tool
- A material doctrinal claim is demonstrably wrong
- AI fabricated a critical authority, organisation, capability, or event
- Content materially contradicts the approved scenario
- Content could mislead the Training Audience in a way that undermines the Training Objective
- No accountable human reviewer is available

## Human Approval Record

**Product:**  
**AI tool used:**  
**Prompt/workflow version:**  
**Human reviewer:**  
**Functional SME consulted:**  
**Doctrinal SME consulted:**  
**Security review required:** Yes / No  
**Final status:** GREEN / AMBER / RED  
**Corrections required:**  
**Final approval:**  
**Date:**  

## Core Assurance Principle

**AI can accelerate content production, but credibility, security, doctrinal accuracy, and approval remain human responsibilities.**
