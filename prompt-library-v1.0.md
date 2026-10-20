# Prompt Library v1.0

## Purpose

This library provides reusable, structured prompt templates for AI-assisted exercise-content development.

The templates are designed to support:

- Drafting
- Adaptation
- Translation
- Consistency checking
- Quality assurance
- Review
- Red-team challenge
- Human-in-the-loop validation

They are intended for synthetic/unclassified professional use and should only be used with AI-enabled tools that are authorised for the information being processed.

## Core Prompting Principles

1. **Use approved source material.**
2. **State the Training Objective explicitly.**
3. **Define the Training Audience activity you want to stimulate.**
4. **Constrain the model from inventing facts, authorities, organisations, or doctrine.**
5. **Require uncertainty to be flagged rather than hidden.**
6. **Separate generation from validation.**
7. **Require human review before use.**
8. **Version prompts when they are changed.**

---

# Prompt 1 — Exercise Content Generation

## Purpose

Create a first draft of an exercise trigger, inject, or supporting content item from approved source material.

## Template

```text
ROLE
You are supporting an Exercise Content Analyst responsible for developing coherent, operationally plausible, and Training Objective-aligned exercise content.

TASK
Develop one draft exercise-content item based only on the information provided below.

TRAINING OBJECTIVE
[Insert Training Objective]

EXERCISE PHASE
[Strategy Workshop / Content Development Workshop / Content Refinement Workshop / Execution / Post-exercise]

SCENARIO CONTEXT
[Insert approved scenario information]

ACTORS INVOLVED
[Insert actors]

OPERATIONAL CONDITIONS / CONSTRAINTS
[Insert constraints]

DESIRED TRAINING AUDIENCE ACTIVITY
[Insert expected analysis, coordination, decision, or action]

APPROVED SOURCE MATERIAL
[Insert authorised source material]

INSTRUCTIONS
1. Do not introduce facts, authorities, capabilities, or organisations that are not supported by the source material.
2. Do not invent doctrine or procedures.
3. If information is missing, identify the gap explicitly rather than making an unsupported assumption.
4. Maintain consistency with the scenario and chronology.
5. Ensure the content creates a realistic requirement for Training Audience consideration or action.
6. Do not reveal or prescribe the intended solution.

REQUIRED OUTPUT
1. Trigger / Situation
2. Immediate Effect
3. Affected Function(s)
4. Expected Training Audience Activity
5. Supporting Information Required
6. Assumptions Requiring Human Verification
7. Potential Doctrinal Issues Requiring SME Review
```

## Human Review Focus

Check:

- Training Objective alignment
- Scenario coherence
- Operational plausibility
- Doctrinal risk
- Hallucinations
- Information exposure
- Training Audience suitability

---

# Prompt 2 — Scenario and Consistency Review

## Purpose

Review drafted content for contradictions, drift, duplication, and weak linkage to the Training Objective.

## Template

```text
ROLE
You are acting as a consistency reviewer. You are not the final approving authority.

CONTENT TO REVIEW
[Insert draft content]

APPROVED SCENARIO CONTEXT
[Insert relevant scenario information]

TRAINING OBJECTIVE
[Insert TO]

CHECK FOR
- Scenario contradictions
- Timeline conflicts
- Incorrect actor roles
- Duplicate or overlapping effects
- Unsupported assumptions
- Unrealistic sequencing
- Missing dependencies
- Contradictory information
- Excessive information given to the Training Audience
- Weak or unclear linkage to the Training Objective

REQUIRED OUTPUT
Provide a table with:
1. Review Area
2. Finding
3. Severity: Low / Medium / High
4. Recommended Action

Then provide:
- Suitable for human review: Yes / No
- Issues requiring SME validation
- Missing information that should not be assumed
```

## Human Review Focus

Do not accept the model's conclusion that content is "correct." Use the output only to support professional review.

---

# Prompt 3 — Doctrinal Risk Review

## Purpose

Identify statements that require doctrinal or functional-SME verification.

## Template

```text
ROLE
You are a doctrinal-risk reviewer. Your role is to identify statements that may require verification, not to certify them as doctrinally correct.

CONTENT
[Insert content]

KNOWN AUTHORISED REFERENCES
[Insert approved references if available]

INSTRUCTIONS
1. Identify statements that imply doctrine, authority, command relationships, responsibilities, or procedures.
2. Flag wording that appears uncertain or potentially inconsistent.
3. Explain why verification is required.
4. Identify the type of SME or authoritative source that should validate the statement.
5. Do not invent a doctrinal answer if the reference is not provided.

REQUIRED OUTPUT
Provide a table with:
- Statement
- Why Verification Is Required
- Risk Level: Low / Medium / High
- Suggested Validator
```

## Human Review Focus

Any material issue involving command authority, legal authority, rules, responsibilities, or operational command relationships should be escalated.

---

# Prompt 4 — Approved Content Adaptation

## Purpose

Adapt already approved content into another delivery format without changing the underlying facts.

## Template

```text
ROLE
You are adapting approved exercise content into a new format.

APPROVED SOURCE CONTENT
[Insert approved content]

TARGET FORMAT
Choose one:
- Training Audience portal message
- Simulated media article
- HICON communication
- EXCON note
- SME brief
- Situation update
- Translation / language adaptation

RULES
1. Preserve all approved facts.
2. Do not introduce new actors, authorities, effects, or events.
3. Do not alter timing or causality.
4. Adjust tone, length, and structure only.
5. Clearly flag any point that cannot be adapted without clarification.

REQUIRED OUTPUT
1. Adapted Product
2. Changes Made
3. Facts Preserved
4. Items Requiring Human Verification
```

## Human Review Focus

Confirm that adaptation has not altered:

- Meaning
- Chronology
- Authority
- Cause and effect
- Information exposure

---

# Prompt 5 — Translation Support

## Purpose

Support controlled translation while protecting meaning, terminology, and factual accuracy.

## Template

```text
ROLE
You are supporting translation of approved exercise content.

SOURCE LANGUAGE
[Insert]

TARGET LANGUAGE
[Insert]

APPROVED SOURCE TEXT
[Insert]

TERMINOLOGY / GLOSSARY
[Insert approved terms if available]

INSTRUCTIONS
1. Preserve meaning and factual content.
2. Do not simplify technical or military terminology unless requested.
3. Do not invent equivalents for terms that are unclear.
4. Flag ambiguous phrases.
5. Preserve names, dates, quantities, and authorities exactly unless an approved translation exists.

REQUIRED OUTPUT
1. Translation
2. Terms Requiring Human Verification
3. Ambiguities Identified
4. Any terminology that may require SME review
```

## Human Review Focus

Human review is mandatory where:

- terminology has operational meaning;
- authority or responsibility could change through wording;
- translation affects the Training Audience's interpretation.

---

# Prompt 6 — Quality Assurance Review

## Purpose

Conduct a structured pre-approval review against defined quality criteria.

## Template

```text
ROLE
You are supporting quality assurance for exercise content.

CONTENT
[Insert draft]

TRAINING OBJECTIVE
[Insert]

SCENARIO CONTEXT
[Insert]

ASSESS AGAINST
- Training Objective alignment
- Scenario coherence
- Operational plausibility
- Doctrinal risk
- Factual accuracy
- Hallucination risk
- Training Audience suitability
- Clarity
- Unnecessary leading
- Missing assumptions

REQUIRED OUTPUT
For each criterion:
- Finding
- Confidence level
- Issue severity
- Recommended human action

FINAL OUTPUT
- Ready for human approval
- Human revision required
- SME validation required
- Reject and redevelop
```

## Human Review Focus

This prompt supports the assurance process; it does not replace the formal human checklist.

---

# Prompt 7 — Red-Team Review

## Purpose

Challenge draft content and deliberately search for weaknesses before approval.

## Template

```text
ROLE
Act as a critical red-team reviewer.

CONTENT
[Insert draft]

TRAINING OBJECTIVE
[Insert]

SCENARIO CONTEXT
[Insert]

CHALLENGE THE CONTENT FOR
- Hallucinated facts
- Unsupported assumptions
- Unrealistic actor behaviour
- Unrealistic timing
- Weak operational logic
- Doctrinal risk
- Too much information for the Training Audience
- Too little information for the Training Audience
- Missing dependencies
- Contradictions
- Weak Training Objective linkage
- Potential security concerns
- Ambiguous wording
- Unintended leading of the Training Audience

REQUIRED OUTPUT
1. Critical Issues
2. Moderate Issues
3. Minor Issues
4. Questions for the Content Analyst
5. Recommendation:
   - Proceed to human review
   - Revise before human review
   - SME validation required
   - Reject and redevelop
```

## Human Review Focus

Red-team findings should be compared against the assurance framework, not accepted automatically.

---

# Prompt 8 — Post-Exercise Review Support

## Purpose

Support structured review of exercise-content performance after delivery.

## Template

```text
ROLE
You are supporting post-exercise analysis of exercise content.

CONTENT ITEM
[Insert]

TRAINING OBJECTIVE
[Insert]

OBSERVED TRAINING AUDIENCE RESPONSE
[Insert]

EXCON / SME OBSERVATIONS
[Insert]

ASSESS
- Did the content stimulate the intended Training Audience activity?
- Was the level of difficulty appropriate?
- Was the information sufficient?
- Was the content too leading?
- Were there scenario or doctrinal issues?
- Were any AI-assisted elements problematic?
- What should be retained, revised, or removed?

REQUIRED OUTPUT
1. What Worked
2. What Did Not Work
3. Training Effect Achieved: Yes / Partially / No
4. Recommended Changes
5. Lessons for Prompt / Workflow Improvement
```

## Human Review Focus

Use post-exercise findings to improve:

- Prompt templates
- Assurance criteria
- Review thresholds
- User guidance
- Future content development

---

# Prompt Version Control

Each prompt should carry:

- Prompt name
- Version number
- Date
- Owner
- Intended use
- Changes from previous version
- Test case used
- Known limitations

## Example

```text
Prompt: Exercise Content Generation
Version: 1.1
Change: Added explicit prohibition on inventing authorities
Reason: v1.0 generated unsupported command relationships
Test Case: Synthetic Logistics Case Study 01
Status: Approved for further testing
```

---

## Core Principle

**Structured prompts improve repeatability, but they do not transfer accountability from humans to AI.**
