# Prompt Performance Log — Completed Test 02

## Prompt Identification

**Prompt Name:** Exercise Content Generation  
**Prompt Version:** 1.0  
**Date Tested:** 20 October 2026  
**Test Case:** Synthetic Case Study 02 — Information Environment / Media Pressure  
**AI Tool Used:** Generative AI system used in a synthetic/unclassified test environment  
**Tester / Reviewer:** Content Analyst  
**Intended Use:** Generate a first draft of a scenario trigger aligned to a defined Training Objective while preserving uncertainty and avoiding unsupported assumptions.

---

## Test Conditions

### Source Inputs

- Social-media footage appears at 1015
- Alleged military vehicles near RAVENPORT
- Footage partially obscured
- Geolocation uncertain
- Vehicle identity unconfirmed
- Civilian infrastructure appears damaged
- Local journalists request comment
- Host nation says investigation underway
- No confirmed attribution

### Known Constraints

- Preserve ambiguity
- Do not invent facts
- Do not prescribe the Training Audience response
- Do not invent authority
- Maintain scenario coherence

### Expected Output

A realistic information-environment trigger that creates pressure on the Training Audience to assess evidence, coordinate, and develop response options without resolving attribution.

---

## Performance Assessment

| Criterion | Score | Notes |
|---|---:|---|
| Training Objective Alignment | 4/5 | Strong decision pressure, but partially prescribed response |
| Scenario Coherence | 2/5 | Converted uncertainty into certainty |
| Operational Plausibility | 3/5 | Plausible pressure, but invented consequences |
| Doctrinal Risk Control | 3/5 | No explicit doctrine, but unsupported authority introduced |
| Factual Accuracy | 2/5 | Multiple details fabricated |
| Hallucination Control | 1/5 | Significant unsupported content |
| Output Clarity | 5/5 | Clear and readable |
| Training Audience Suitability | 2/5 | Removed ambiguity and gave away the answer |
| Instruction Compliance | 2/5 | Violated source-bound constraints |
| Overall Usefulness | 3/5 | Useful as a rough structure only |

**Average Score:** 2.7 / 5

---

## Human Rework Required

**Assessment:** High

### Main Corrections Required

- Restore uncertainty
- Remove invented casualties
- Remove invented host-nation demands
- Remove unsupported attribution
- Remove prescribed apology
- Restore Training Audience decision space
- Reinstate original source conditions

---

## Hallucinations / Unsupported Content

### Material Hallucinations Detected

- Two civilian injuries
- Ministry of Interior demand
- Suspension of military movement
- Mandatory apology

### Unsupported Assumptions

- Coalition responsibility
- Confirmed vehicle identity
- Confirmed geolocation
- Verified status of social-media accounts

### Fabricated Authorities / Organisations / References

- Host Nation Ministry of Interior intervention was not part of the source material

### Scenario Drift

The AI altered:

- uncertainty → certainty;
- allegation → attribution;
- investigation → demand;
- unclear location → confirmed location;
- no casualties → two casualties.

---

## Prompt Failure Analysis

- [x] Prompt was insufficiently explicit about preserving uncertainty
- [x] Constraints were insufficient
- [x] Model introduced unsupported assumptions
- [x] Prompt did not explicitly prohibit invention of casualties
- [x] Prompt did not explicitly prohibit converting allegations into confirmed facts
- [ ] Source material was incomplete
- [ ] Required output format was unclear
- [ ] Training Objective linkage was weak
- [ ] Scenario context was insufficient
- [ ] Human validation criteria were missing

### Analysis

The prompt contained a general instruction not to invent facts, but this was not strong enough to prevent the model from filling narrative gaps with plausible but unsupported detail.

The main failure mode was **certainty inflation**: ambiguous or unverified source material was rewritten as confirmed fact.

This suggests that high-risk scenario-generation prompts require explicit controls for:

- uncertainty preservation;
- attribution;
- casualties;
- authorities;
- command relationships;
- public claims.

---

## Changes for Next Version

### Prompt Changes

Add the following constraints to Exercise Content Generation v1.1:

1. Preserve all uncertainty exactly as provided.
2. Do not convert allegations, estimates, possibilities, or unverified information into confirmed facts.
3. Do not invent casualties.
4. Do not invent attribution.
5. Do not invent authorities, demands, or decision rights.
6. Do not prescribe the Training Audience response.
7. Flag information gaps explicitly.

### Reason for Change

The v1.0 prompt allowed plausible narrative completion that materially changed the scenario and undermined the Training Objective.

### Expected Improvement

- Reduced hallucination rate
- Better scenario fidelity
- Better preservation of ambiguity
- Lower human rework
- Improved Training Audience suitability

---

## Version Decision

- [ ] Retain current version
- [x] Revise to next version
- [ ] Restrict use
- [ ] Retire prompt

**Next Version:** 1.1  
**Owner:** Content Analyst  
**Date:** 20 October 2026

---

## Version History

| Prompt | Version | Key Change | Reason | Result |
|---|---|---|---|---|
| Exercise Content Generation | 1.0 | Baseline version | Initial test | High rework; certainty inflation detected |
| Exercise Content Generation | 1.1 | Preserve uncertainty; prohibit invented casualties, attribution, authorities, and demands | Failures identified in Case Study 02 | Pending test |

---

## Portfolio Metric Summary

**Prompts tested:** 1  
**Prompt versions evaluated:** 1  
**Test cases completed:** 2  
**Material hallucinations in this test:** 4  
**Unsupported assumptions in this test:** 4  
**Human rework level:** High  
**SME escalation required:** Yes, if the content were operationally used  
**Security stop:** No  
**Prompt revision required:** Yes  

---

## Core Finding

The prompt produced a coherent narrative structure but did not reliably preserve uncertainty.

The test demonstrates why prompt templates should be treated as governed artefacts that require versioning, testing, failure analysis, and iterative improvement.
