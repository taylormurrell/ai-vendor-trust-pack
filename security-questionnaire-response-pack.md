# Sample Security Questionnaire Responses
## Five representative responses for a fictional AI-for-finance vendor undergoing bank diligence

**Fictional sample. For educational and portfolio purposes only.**
FinSight AI is not a real company. These responses do not reflect any real company's controls or compliance status and would require validation by qualified security and legal teams before use in a real diligence process.

These five responses were selected to show coverage across baseline assurance, AI data use, internal access, multi-tenant security, and AI governance.

---

### Q1. Does FinSight AI hold a current SOC 2 Type II report? If so, which trust service criteria are in scope?

**Sample response:**
FinSight AI holds a current SOC 2 Type II report covering the Security trust services category. The audit period covers 12 months ending Q4 2025 and was conducted by an independent third-party auditor. Availability and Confidentiality are planned for inclusion in a future audit cycle as customer requirements mature. The full report is available to customers and qualified prospects under a signed NDA. A bridge letter or management representation letter is available if the report is more than six months old at the time of request.

**Relevant trust theme:** Security governance and certification
**Evidence typically requested:** SOC 2 Type II report (under NDA), bridge letter or management representation letter if applicable

---

### Q7. Does FinSight AI use customer data to train, fine-tune, or improve AI models (including foundation models provided by third parties)?

**Sample response:**
FinSight AI does not use customer data to train, fine-tune, or otherwise improve AI models (including any foundation models provided by third-party subprocessors). This restriction applies by default and is not a configurable setting.

This commitment is reflected in our Data Processing Agreement (DPA), which explicitly prohibits use of customer data for model training purposes. Our primary model subprocessor operates under a separate data processing agreement containing equivalent restrictions. Where customer data is transferred from the EEA to a jurisdiction without an adequacy decision, the DPA incorporates Standard Contractual Clauses and supporting technical and organizational measures.

Customer data (including prompts, uploaded documents, and AI-generated outputs) is retained for the duration of the customer relationship and deleted within 30 days of contract termination or upon written request.

**Relevant trust theme:** AI governance and data protection
**Evidence typically requested:** DPA with explicit training prohibition language (under NDA), model subprocessor agreement summary, written attestation from a named officer on request, subprocessor list

---

### Q14. Which FinSight AI employees can access customer data or customer prompts, and under what conditions?

**Sample response:**
Access to customer data (including prompts, AI-generated outputs, and uploaded documents) is restricted to a defined set of roles with a documented business need. Access is granted through a formal request-and-approval process, requires MFA, and is logged to a write-protected or tamper-evident audit trail. Access reviews are conducted quarterly. Support staff may access session metadata for troubleshooting purposes but do not have access to prompt or output content without explicit customer authorization. Content access for security incident investigation is permitted only with documented approval from the Head of Security. FinSight AI does not grant persistent access to individual customers' data environments as a routine operational practice.

**Relevant trust theme:** Privileged access and data protection
**Evidence typically requested:** Access control policy, privileged access review records, SOC 2 logical access section, audit log format documentation

---

### Q16. How does FinSight AI achieve tenant isolation (ensuring one customer's data is not accessible to another customer's session or environment)?

**Sample response:**
FinSight AI enforces tenant isolation through tenant-scoped authorization checks at the application layer, database-level segmentation controls at the data layer, and session-level isolation of AI context and prompt history. A session authenticated for one customer has no access to data, query history, or AI context belonging to another. Tenant isolation controls are included in the scope of our annual penetration test, and findings related to logical separation are covered in our SOC 2 Type II report.

**Relevant trust theme:** Multi-tenancy and data isolation
**Evidence typically requested:** Architecture documentation, SOC 2 logical separation section, penetration test scope confirming isolation was tested

---

### Q22. What is FinSight AI's approach to human oversight for high-impact workflows such as credit analysis, compliance screening, or regulatory reporting?

**Sample response:**
FinSight AI is designed to support analyst workflows rather than replace human judgment in consequential decisions. For use cases identified as high-impact (including outputs used in credit analysis, regulatory reporting, or compliance screening), the platform requires user acknowledgment before an output is exported or used to trigger a downstream action. FinSight AI does not autonomously submit filings, execute transactions, or initiate downstream system actions without a human step in the workflow. Human review reduces risk in high-impact workflows but does not automatically remove a use case from high-risk treatment under frameworks such as the EU AI Act, where classification depends on whether the AI system materially influences a consequential decision. Customers deploying the platform in Annex III or Annex III-adjacent workflows are encouraged to conduct their own regulatory review. Customers can configure additional approval gates through the platform's workflow settings. Documentation on human-in-the-loop workflow design is included in our product guide and available during implementation.

**Relevant trust theme:** Human oversight and AI governance
**Evidence typically requested:** Product documentation on workflow controls, human-in-the-loop configuration guide, use case risk assessment

---

*This document is a fictional sample created for educational and portfolio purposes. FinSight AI is not a real company. Sample responses do not reflect any real company's controls or compliance posture and would require validation by qualified security, legal, and compliance professionals before use in a real diligence process.*
