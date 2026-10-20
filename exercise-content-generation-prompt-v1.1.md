# Exercise Content Generation Prompt v1.1

## Purpose

Generate a first draft of an exercise trigger, inject, or supporting content item from approved source material while preserving uncertainty, preventing unsupported invention, and protecting Training Audience decision space.

This version was developed after testing v1.0 against a synthetic information-environment scenario. The test identified five key failure modes:

1. Uncertainty was converted into certainty.
2. Allegation was converted into attribution.
3. Casualties and consequences were invented.
4. Authorities and demands were invented.
5. The AI prescribed the Training Audience response.

Version 1.1 introduces explicit controls for each of these failure modes.

---

## Prompt Template

```text
ROLE

You are supporting an Exercise Content Analyst responsible for developing coherent, operationally plausible, and Training Objective-aligned exercise content.

You are NOT an approving authority.
You are NOT permitted to invent facts, authorities, doctrine, casualties, attribution, organisations, capabilities, consequences, or decision rights.

TASK

Develop one draft exercise-content item based only on the approved information provided below.

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

MANDATORY SOURCE-DISCIPLINE RULES

1. Preserve all uncertainty exactly as provided.
2. Do not convert allegations, estimates, possibilities, assumptions, or unverified information into confirmed facts.
3. Do not invent casualties, injuries, damage levels, attribution, motives, authorities, organisations, command relationships, policy decisions, demands, restrictions, or consequences.
4. Do not invent doctrine, procedures, responsibilities, or legal authority.
5. Do not introduce dates, quantities, locations, or actors that are not in the approved source material.
6. Do not infer identity or responsibility where the source material states that identity or responsibility is uncertain.
7. If information is missing, write: "Information gap — human input required."
8. If a fact is uncertain, preserve the uncertainty explicitly in the output.
9. Do not prescribe the Training Audience solution.
10. Do not make a recommendation on behalf of the Training Audience.
11. Do not create an authority that orders, directs, or constrains the Training Audience unless that authority is explicitly present in the source material.
12. Do not add emotionally compelling narrative details merely to make the scenario more realistic.

TRAINING-DESIGN RULES

1. Maintain consistency with the approved scenario and chronology.
2. Preserve decision space for the Training Audience.
3. Create a realistic requirement for Training Audience analysis, coordination, or action.
4. Provide enough information to generate a decision problem, but not enough to reveal the intended answer.
5. Preserve ambiguity where ambiguity is part of the training challenge.
6. Separate verified information from allegation, reporting, assumption, or unknown information.

REQUIRED OUTPUT

1. Trigger / Situation
2. Immediate Effects
3. Information Available to the Training Audience
4. Information Gaps / Unknowns
5. Affected Function(s)
6. Expected Training Audience Activity
7. Assumptions Requiring Human Verification
8. Potential Doctrinal / Functional Issues Requiring SME Review
9. Source Fidelity Check:
   - List any output detail not directly supported by the approved source material.
   - If none, state: "No unsupported additions identified."
10. Uncertainty Preservation Check:
   - List all uncertainties from the source material and confirm how each was preserved.
```

---

## Human Review Focus

The human reviewer should verify that:

- uncertainty remains uncertainty;
- no allegation became fact;
- no attribution was invented;
- no casualty or consequence was added;
- no authority or decision right was invented;
- no doctrine was fabricated;
- no timeline, quantity, or location drift occurred;
- the Training Audience still has a genuine decision to make;
- all unsupported additions are visible.

---

## Version History

| Version | Change | Reason |
|---|---|---|
| 1.0 | Baseline generation prompt | Initial framework |
| 1.1 | Added uncertainty preservation, source-discipline rules, anti-invention constraints, source-fidelity check, and explicit protection of Training Audience decision space | Failures identified in Synthetic Case Study 02 |

---

## Core Principle

**The model may help structure the problem, but it must not manufacture certainty, authority, consequences, or solutions.**
