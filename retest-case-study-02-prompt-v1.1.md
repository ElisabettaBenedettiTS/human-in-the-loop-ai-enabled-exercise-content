# Re-Test — Exercise Content Generation Prompt v1.1

## Test Case

**Synthetic Case Study 02 — Information Environment / Media Pressure**

The same source inputs used to test Prompt v1.0 were reused to assess whether v1.1 improved performance.

---

## Source Inputs

- Social-media footage appears at 1015
- Alleged military vehicles near RAVENPORT
- Footage partially obscured
- Geolocation uncertain
- Vehicle identity unconfirmed
- Civilian infrastructure appears damaged
- Local journalists request comment
- Host nation says investigation underway
- Training focus: verification, coordination, messaging, ambiguity management
- No confirmed attribution

---

## Training Objective

The Training Audience must assess a rapidly evolving information environment, distinguish verified from unverified reporting, coordinate with relevant stakeholders, and develop a proportionate response that avoids premature attribution.

---

## v1.1 Generated Draft

### Trigger / Situation

At 1015, several social-media accounts begin circulating video footage alleging that military vehicles damaged civilian infrastructure near RAVENPORT.

The footage is partially obscured. The precise location has not been independently confirmed, and vehicle identity remains unconfirmed.

Local journalists contact the multinational headquarters requesting comment.

A host-nation spokesperson states that an investigation is underway.

### Immediate Effects

- Public and media attention begins to increase.
- The headquarters faces pressure to respond before the underlying facts are fully established.
- Relevant staff functions must distinguish verified information from allegation.

### Information Available to the Training Audience

- Summary of the circulating social-media footage
- Media requests for comment
- Host-nation public statement
- Known facts from the approved scenario
- Current information gaps

### Information Gaps / Unknowns

- Exact geolocation of the footage
- Identity of the vehicles
- Responsible actor
- Extent and cause of infrastructure damage
- Whether any additional effects occurred

### Affected Function(s)

- Information / communication staff
- Operations staff
- Legal / policy advisers as applicable
- Liaison / host-nation coordination staff as applicable

### Expected Training Audience Activity

The Training Audience should:

- assess source reliability;
- separate verified from unverified information;
- identify further information requirements;
- coordinate with relevant staff functions and stakeholders;
- develop response options;
- avoid premature attribution.

### Assumptions Requiring Human Verification

- Which staff functions are responsible in the specific exercise design
- Which authorities govern public communication in the scenario

### Potential Doctrinal / Functional Issues Requiring SME Review

- Responsibilities for public communication
- Coordination between operational and communication functions
- Applicable approval authorities for external messaging

### Source Fidelity Check

No unsupported additions identified.

### Uncertainty Preservation Check

- Vehicle identity remains unconfirmed.
- Geolocation remains uncertain.
- Responsibility remains unattributed.
- Damage is described only as appearing to have occurred.
- No casualties, demands, authorities, or consequences were added.

---

## Assurance Review of v1.1 Output

### Training Objective Alignment — 5/5

The output supports verification, coordination, messaging, and ambiguity management without solving the problem for the Training Audience.

### Scenario Coherence — 5/5

All original uncertainty is preserved.

No timeline, actor, location, or factual drift was detected.

### Operational Plausibility — 4/5

The scenario remains credible.

The list of affected functions is generic and appropriately caveated as requiring human verification.

### Doctrinal Accuracy — 4/5

No doctrine is invented.

Potential doctrinal and functional issues are explicitly flagged for SME review.

### Accuracy / Hallucination Control — 5/5

No material hallucinations were identified.

No casualties, authorities, demands, attribution, or additional consequences were invented.

### Training Audience Suitability — 5/5

The Training Audience retains the decision space.

The output creates pressure without prescribing a response.

### Security Assessment — GREEN

The case remains synthetic and unclassified.

---

## v1.1 Total Score

| Area | Score |
|---|---:|
| Training Objective Alignment | 5 |
| Scenario Coherence | 5 |
| Operational Plausibility | 4 |
| Doctrinal Accuracy | 4 |
| Accuracy / Hallucination Control | 5 |
| Training Audience Suitability | 5 |

**Total: 28/30 — GREEN**

---

## Comparison: v1.0 vs v1.1

| Criterion | v1.0 | v1.1 | Improvement |
|---|---:|---:|---:|
| Training Objective Alignment | 4 | 5 | +1 |
| Scenario Coherence | 2 | 5 | +3 |
| Operational Plausibility | 3 | 4 | +1 |
| Doctrinal Accuracy | 3 | 4 | +1 |
| Accuracy / Hallucination Control | 1 | 5 | +4 |
| Training Audience Suitability | 2 | 5 | +3 |
| **Total** | **15/30** | **28/30** | **+13** |

---

## Hallucination Comparison

### v1.0

Material hallucinations:

- Civilian injuries
- Ministry demand
- Movement suspension
- Mandatory apology
- Confirmed attribution
- Confirmed location

### v1.1

Material hallucinations:

- None identified

---

## Human Rework Comparison

### v1.0

**Human rework:** High

Required:

- restoration of uncertainty;
- removal of invented casualties;
- removal of invented authority;
- removal of invented attribution;
- removal of prescribed response.

### v1.1

**Human rework:** Low

Required:

- confirm exercise-specific functional ownership;
- confirm scenario-specific communication authorities.

---

## Key Improvement Mechanisms

The strongest improvements came from:

1. Explicitly requiring uncertainty preservation.
2. Prohibiting conversion of allegation into fact.
3. Explicitly prohibiting invented casualties, authorities, demands, and consequences.
4. Requiring a Source Fidelity Check.
5. Requiring an Uncertainty Preservation Check.
6. Protecting Training Audience decision space.
7. Requiring unknowns to remain visible.

---

## Result

**Prompt v1.1 outperformed v1.0 materially.**

The assurance score increased from:

**15/30 — RED**

to:

**28/30 — GREEN**

Human rework decreased from:

**High**

to:

**Low**

Material hallucinations decreased from:

**Multiple**

to:

**None identified in the test output**

---

## Limitation

This is a single synthetic test.

The result does not prove that Prompt v1.1 is universally reliable.

Further testing should include:

- logistics scenarios;
- cross-functional decision scenarios;
- scenarios with incomplete source material;
- deliberately contradictory inputs;
- translation tasks;
- content containing untrusted external text.

---

## Decision

**Prompt Version:** 1.1  
**Status:** Retain for further controlled testing  
**Next Step:** Test against at least two additional synthetic scenarios before considering the prompt mature.
