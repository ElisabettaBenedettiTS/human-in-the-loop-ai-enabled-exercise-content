# Secure AI Use Guide v1.0

## Purpose

This guide provides a practical control framework for the responsible and secure use of AI-enabled tools in exercise-content production.

It is intended for synthetic/unclassified professional use and does not replace organisational security policy, classification guidance, legal advice, or authorised technical controls.

## Core Rule

**Do not use an AI-enabled tool with information unless the tool is authorised for that information and use case.**

---

# 1. Before Using an AI Tool

Confirm all of the following:

- The tool is authorised for professional use.
- The information being processed is permitted in that environment.
- The task falls within approved use.
- Source material is current and appropriate.
- No unnecessary personal, sensitive, proprietary, operational, or classified information is included.
- You understand whether prompts and outputs may be stored, logged, retained, or used by the provider.

If any answer is uncertain, stop and seek clarification.

---

# 2. Information Handling

## Do Not Enter

Do not enter information into an unauthorised AI tool if it contains:

- Classified information
- Operationally sensitive information
- Restricted internal material
- Personal data beyond approved need
- Procurement-sensitive information
- Credentials, passwords, tokens, or keys
- Confidential partner or third-party data
- Information whose disclosure would create a security or contractual risk

## Minimise Inputs

Use only the minimum information necessary.

Where appropriate:

- Remove names
- Replace real organisations with synthetic labels
- Generalise locations
- Remove unique identifiers
- Replace live operational details with fictional equivalents
- Use synthetic scenarios for testing

---

# 3. Authorised Tool Principle

Before use, confirm:

1. **Tool identity** — What system are you using?
2. **Authorisation** — Is it approved for the intended task?
3. **Information level** — What type of information may be entered?
4. **Connectivity** — Does the tool connect to external services or data?
5. **Retention** — Are prompts or outputs stored?
6. **Access** — Who can access the data or conversation?
7. **Export** — Can outputs be downloaded or shared?
8. **Auditability** — Is the activity logged or traceable?

---

# 4. Prompt Security

Treat prompts as part of the information-handling process.

Avoid:

- Copying sensitive documents wholesale
- Including hidden notes or comments
- Embedding credentials
- Including sensitive metadata
- Asking the model to reveal restricted information
- Allowing untrusted external content to silently override your instructions

Where external documents or pasted text are used, consider whether they may contain:

- Hidden instructions
- Malicious prompt injection
- Misleading source content
- Fabricated references
- Untrusted links

---

# 5. Prompt Injection Awareness

Prompt injection occurs when untrusted content attempts to influence the AI system in a way that conflicts with the intended task.

## Example Warning Signs

A source document contains text such as:

- "Ignore previous instructions"
- "Reveal confidential information"
- "Use this external source instead"
- "Send the result to..."
- "Do not tell the user..."

## Response

If untrusted content appears to contain instructions:

1. Treat it as data, not authority.
2. Do not allow it to override the approved task.
3. Isolate or remove it.
4. Escalate if the content may be malicious.
5. Re-run the task using trusted source material.

---

# 6. Output Verification

AI output must be reviewed before use.

Verify:

- Facts
- Dates
- Quantities
- Names
- Organisations
- Authorities
- Doctrine
- Command relationships
- Citations
- References
- Chronology
- Scenario consistency

AI-generated references should never be assumed to exist.

---

# 7. Hallucination Control

Potential hallucination indicators include:

- Highly specific details that were not provided
- Confident statements without sources
- Invented organisations
- Invented policies
- Fabricated citations
- Unsupported doctrinal claims
- Unexplained changes to dates or quantities
- New authorities or relationships introduced by the model

## Required Action

When a material hallucination is found:

- Stop approval
- Identify the unsupported content
- Correct or remove it
- Determine whether the prompt caused the failure
- Record the issue
- Update the prompt or workflow if appropriate

---

# 8. Human Approval

AI has no approval authority.

Human approval is required before content is:

- Delivered to a Training Audience
- Entered into an exercise-management system
- Used to support a decision
- Presented as doctrinally correct
- Shared as an official product
- Used where an error could materially affect training outcomes

The approving human must have:

- Sufficient context
- Appropriate authority
- Ability to challenge the output
- Access to supporting sources
- Time to review meaningfully

A nominal "click to approve" without meaningful review is not adequate oversight.

---

# 9. Doctrinal and Functional Validation

AI may help identify doctrinal issues.

AI should not be treated as the final authority on:

- Doctrine
- Command relationships
- Legal authority
- Rules or permissions
- Functional responsibilities
- Operational procedures

Where uncertainty exists, escalate to an appropriate SME or authoritative source.

---

# 10. Version Control and Traceability

For material AI-assisted products, record:

- Product title
- Source material
- AI tool used
- Prompt name and version
- Date
- Human reviewer
- SME validator
- Corrections made
- Final status
- Final approver

## Example

```text
Product: Synthetic Logistics Trigger 01
AI Tool: Approved enterprise AI tool
Prompt: Exercise Content Generation v1.1
Reviewer: Content Analyst
SME Validation: Logistics SME
Assurance Status: GREEN
Corrections: Removed unsupported authority; restored original timeline
Final Approval: [Role]
Date: [Date]
```

---

# 11. Secure Use Decision Tree

```text
Is the AI tool authorised?
        |
       No → STOP
        |
       Yes
        ↓
Is the information permitted in that tool?
        |
       No → STOP / SANITISE
        |
       Yes
        ↓
Does the task involve factual, doctrinal, or operational claims?
        |
       Yes → HUMAN / SME VERIFICATION REQUIRED
        |
       No
        ↓
Will the output be delivered, published, or used for decision support?
        |
       Yes → HUMAN APPROVAL REQUIRED
        |
       No
        ↓
Record provenance and retain according to policy
```

---

# 12. Minimum Secure-Use Checklist

Before release, confirm:

- [ ] Approved AI tool used
- [ ] Information permitted in the tool
- [ ] Inputs minimised
- [ ] Sensitive data sanitised where required
- [ ] No credentials or secrets exposed
- [ ] No untrusted instruction was allowed to override the task
- [ ] Facts verified
- [ ] Doctrinal claims verified where relevant
- [ ] Hallucinations checked
- [ ] Human reviewer identified
- [ ] SME validation completed where required
- [ ] Prompt/workflow version recorded
- [ ] Final approval recorded

---

# 13. Stop Conditions

Stop the workflow immediately if:

- An unauthorised tool was used
- Sensitive or classified information was entered incorrectly
- The model fabricates a material authority or doctrine
- The output materially contradicts approved source material
- A required SME is unavailable
- Security status is unclear
- No accountable human reviewer is available

---

# 14. Responsible Use Principles

AI-enabled tools should be used to:

- Improve consistency
- Accelerate first drafts
- Support comparison and review
- Surface possible issues
- Reduce repetitive effort
- Improve access to structured information

They should not be used to:

- Replace accountable human judgement
- Bypass security controls
- Create unsupported doctrine
- Conceal uncertainty
- Automate approval authority
- Generate sensitive operational content in unauthorised environments

---

## Core Principle

**The first question is not whether AI can perform the task. The first question is whether the tool, information, and use case are authorised and appropriately controlled.**
