# Security Questionnaire Response Pack
## FinSight AI -- Sample Bank Diligence Responses

**Fictional sample. For educational and portfolio purposes only.**
FinSight AI is not a real company. These responses do not reflect any real company's controls or compliance status and would require validation by qualified security and legal teams before use in a real diligence process.

---

## Section 1: Company and Compliance Posture

---

### Q1. Does FinSight AI hold a current SOC 2 Type II report? If so, which trust service criteria are in scope?

**Sample response:**
FinSight AI holds a current SOC 2 Type II report covering the Security trust service criterion. The audit period covers 12 months ending Q4 2025 and was conducted by an independent third-party auditor. The Availability and Confidentiality criteria are in scope for the next audit cycle, currently underway. The full report is available to customers and qualified prospects under a signed NDA. A bridge letter attesting to no material changes in controls is available if the report is more than six months old at the time of request.

**Relevant trust theme:** Security governance and certification
**Evidence typically requested:** SOC 2 Type II report (under NDA), bridge letter if applicable

---

### Q2. Does FinSight AI have an information security policy? When was it last reviewed?

**Sample response:**
FinSight AI maintains a formal information security policy covering data classification, acceptable use, access control, incident response, and vendor risk. The policy is reviewed and formally approved by senior leadership on an annual basis, or following material changes to our environment or threat landscape. The most recent review was completed in Q4 2025. The policy is owned by the Head of Security. A summary version is available to customers under NDA.

**Relevant trust theme:** Security governance
**Evidence typically requested:** Policy summary or table of contents (under NDA), review date attestation

---

### Q3. Is FinSight AI pursuing or aligned with ISO 27001? If not certified, what elements of the standard do you follow?

**Sample response:**
FinSight AI is not currently ISO 27001 certified. Our information security program is designed to align with ISO 27001 principles, including risk-based control selection, access management, asset inventory, and supplier risk management. We rely on our SOC 2 Type II report as the primary third-party attestation of our security controls. We are evaluating ISO 27001 certification as our enterprise customer base and compliance requirements grow. A mapping of our SOC 2 control environment to ISO 27001 domains is available on request.

**Relevant trust theme:** Security governance and risk management
**Evidence typically requested:** SOC 2 Type II report, ISO 27001 control mapping (on request)

---

### Q4. Has FinSight AI undergone a third-party penetration test in the last 12 months?

**Sample response:**
FinSight AI conducts an annual third-party penetration test of its production environment. The most recent test was completed in Q1 2026 by an independent security firm with financial-services and AI product experience. The scope included external network, web application, and AI-specific attack vectors consistent with the OWASP LLM Top 10. Critical and high findings are remediated within defined SLAs -- critical within 15 days, high within 30 days -- and remediation is validated before the finding is closed. An executive summary of the most recent test is available to customers under NDA.

**Relevant trust theme:** Vulnerability management
**Evidence typically requested:** Pen test executive summary (under NDA), remediation attestation or log

---

### Q5. What is FinSight AI's vulnerability management program? How are critical vulnerabilities tracked and remediated?

**Sample response:**
FinSight AI operates a vulnerability management program covering all production systems and software dependencies. Vulnerabilities are identified through automated scanning on a weekly cadence, annual third-party penetration testing, and a responsible disclosure program for external researchers. Findings are tracked in a dedicated vulnerability register reviewed by the security team monthly. Remediation SLAs are tiered by severity: critical within 15 days, high within 30 days, medium within 90 days. Exceptions require documented approval and compensating controls. SLA adherence is reviewed quarterly.

**Relevant trust theme:** Vulnerability management
**Evidence typically requested:** Vulnerability management policy, SLA table, recent scan summary (redacted)

---

## Section 2: Data Protection and Privacy

---

### Q6. How is customer data encrypted at rest and in transit?

**Sample response:**
All customer data is encrypted at rest using AES-256. Data in transit is encrypted using TLS 1.2 or higher -- TLS 1.0 and 1.1 are disabled across all production endpoints. Encryption keys are managed through our cloud provider's key management service (KMS), with customer-specific key isolation. Keys are rotated on an annual basis or upon suspected compromise. These controls are validated in our SOC 2 Type II report under the Security trust service criterion.

**Relevant trust theme:** Data protection
**Evidence typically requested:** SOC 2 Type II encryption section, technical architecture summary, key management policy

---

### Q7. Does FinSight AI use customer data to train, fine-tune, or improve AI models -- including foundation models provided by third parties?

**Sample response:**
FinSight AI does not use customer data to train, fine-tune, or otherwise improve AI models -- including any foundation models provided by third-party subprocessors. This restriction applies by default to all customers and is not a configurable setting.

This commitment is reflected in our Data Processing Agreement (DPA), which explicitly prohibits use of customer data for model training purposes. Our primary model subprocessor operates under a separate data processing agreement containing equivalent restrictions. EU-based customers and customers subject to GDPR are covered under Standard Contractual Clauses (SCCs) as the legal transfer mechanism, supplemented by technical and organizational measures documented in our DPA.

Customer data -- including prompts, uploaded documents, and AI-generated outputs -- is retained for the duration of the customer relationship and deleted within 30 days of contract termination or upon written request.

**Relevant trust theme:** AI governance and data protection
**Evidence typically requested:** DPA with explicit training prohibition language (under NDA), model subprocessor agreement summary, written attestation from a named officer on request

---

### Q8. What is FinSight AI's data retention policy? How long is customer data retained, and what triggers deletion?

**Sample response:**
FinSight AI retains customer data -- including prompts, AI-generated outputs, and uploaded documents -- for the duration of the active contract. Data is deleted within 30 days of contract termination unless a shorter period is agreed in writing. Operational and security logs may be retained for up to 12 months for audit and incident investigation purposes, after which they are purged. Customers may request accelerated deletion at any time. Retention terms are reflected in the DPA and are enforceable as a contractual obligation.

**Relevant trust theme:** Data protection and privacy
**Evidence typically requested:** Data retention policy, DPA retention clause, deletion process documentation

---

### Q9. Can a customer request deletion of their data? What is the process and timeline?

**Sample response:**
FinSight AI supports customer-initiated data deletion requests. Upon written request from an authorized customer contact, we will delete all customer data -- including prompts, outputs, and uploaded files -- within 30 days and provide written confirmation of deletion. For customers subject to GDPR, we also support individual data subject deletion requests through a documented process coordinated with the customer's privacy team. Deletion is performed at the application and storage layer; residual copies in backup systems are purged within the next scheduled backup cycle, not to exceed 60 days from the deletion request.

**Relevant trust theme:** Privacy and data subject rights
**Evidence typically requested:** DSR process documentation, sample deletion confirmation, DPA data subject rights clause

---

### Q10. Does FinSight AI transfer customer data outside the customer's jurisdiction? If so, under what legal mechanism?

**Sample response:**
FinSight AI processes customer data in the United States by default. For customers in the European Economic Area, we offer data processing within EU-based infrastructure (AWS EU regions) and rely on Standard Contractual Clauses (SCCs), incorporating the EU Commission's 2021 module, as the legal mechanism for any residual cross-border transfers. Our DPA includes the SCC addendum. A subprocessor list with processing locations is included in our DPA and is updated when material changes occur. Customers are notified of changes to processing locations with a minimum of 30 days' notice.

**Relevant trust theme:** Privacy and regulatory compliance
**Evidence typically requested:** DPA with SCC addendum, data flow diagram, subprocessor list with locations

---

## Section 3: Access Control and Identity

---

### Q11. Does FinSight AI support SSO/SAML integration for customer-facing authentication?

**Sample response:**
FinSight AI supports SSO via SAML 2.0 and OIDC, compatible with major enterprise identity providers including Okta, Azure AD, and Google Workspace. SSO integration is available to all enterprise-tier customers at no additional cost. When SSO is enabled, user authentication is delegated to the customer's identity provider, and FinSight AI does not store or manage user passwords. Provisioning and deprovisioning of user accounts can be managed through SCIM where supported by the customer's IdP.

**Relevant trust theme:** Access control and identity management
**Evidence typically requested:** SSO integration documentation, supported IdP list, SCIM configuration guide

---

### Q12. Is MFA enforced for all internal FinSight AI employee access to production systems and customer data?

**Sample response:**
MFA is mandatory for all FinSight AI employees with access to production systems, internal tooling, and customer data. We enforce MFA through our identity provider using an authenticator app or hardware security key -- SMS-based MFA is not permitted for internal production access. MFA enrollment is required as part of the employee onboarding process and is audited quarterly. Access without MFA is blocked at the identity provider level and cannot be bypassed by individual users. This control is covered under the logical access section of our SOC 2 Type II report.

**Relevant trust theme:** Access control
**Evidence typically requested:** MFA policy, SOC 2 logical access section, quarterly access audit record

---

### Q13. How is role-based access control (RBAC) implemented within the FinSight AI platform?

**Sample response:**
FinSight AI implements role-based access control within the customer-facing platform. Customer administrators can assign users to predefined roles -- read-only analyst, standard user, and administrator -- each with distinct permissions governing data access, query history, and configuration rights. Role assignments are logged and can be reviewed by the customer's administrator at any time through the platform's audit interface. FinSight AI internal staff roles follow the same RBAC model, with additional restrictions on customer data access governed by a separate internal access control policy. Role changes require approval from a designated owner and are logged.

**Relevant trust theme:** Access control
**Evidence typically requested:** RBAC model documentation, platform admin guide, SOC 2 logical access section

---

### Q14. Which FinSight AI employees can access customer data or customer prompts, and under what conditions?

**Sample response:**
Access to customer data -- including prompts, AI-generated outputs, and uploaded documents -- is restricted to a defined set of roles with a documented business need. Access is granted through a formal request-and-approval process, requires MFA, and is logged to a write-protected audit trail. Access reviews are conducted quarterly. Support staff may access session metadata for troubleshooting purposes but do not have access to prompt or output content without explicit customer authorization. Content access for security incident investigation is permitted only with documented approval from the Head of Security. FinSight AI does not grant persistent access to individual customers' data environments as a routine operational practice.

**Relevant trust theme:** Privileged access and data protection
**Evidence typically requested:** Access control policy, privileged access review records, SOC 2 logical access section, audit log format documentation

---

## Section 4: Cloud and Infrastructure Security

---

### Q15. Which cloud provider(s) does FinSight AI use, and in which regions?

**Sample response:**
FinSight AI is hosted on Amazon Web Services (AWS). Production infrastructure operates in the US East (N. Virginia) and US West (Oregon) regions for availability and redundancy. EU customers can request data processing within AWS EU (Ireland) or EU (Frankfurt) regions, subject to configuration at contract time. FinSight AI does not operate on-premises infrastructure. A data residency attestation is available to customers with regulatory requirements around processing location, and is provided as part of the DPA package.

**Relevant trust theme:** Cloud infrastructure and vendor risk
**Evidence typically requested:** Infrastructure architecture overview, data residency attestation, AWS shared responsibility model reference

---

### Q16. How does FinSight AI achieve tenant isolation -- ensuring one customer's data cannot be accessed by another customer's session or environment?

**Sample response:**
FinSight AI enforces tenant isolation through tenant-scoped authorization checks at the application layer, database-level segmentation controls at the data layer, and session-level isolation of AI context and prompt history. A session authenticated for one customer cannot access data, query history, or AI context belonging to another. Tenant isolation controls are included in the scope of our annual penetration test, and findings related to logical separation are covered in our SOC 2 Type II report.

**Relevant trust theme:** Multi-tenancy and data isolation
**Evidence typically requested:** Architecture documentation, SOC 2 logical separation section, penetration test scope confirming isolation was tested

---

### Q17. What is FinSight AI's incident response plan? How quickly would a customer be notified of a breach affecting their data?

**Sample response:**
FinSight AI maintains a documented incident response plan covering detection, containment, eradication, recovery, and post-incident review. The plan is tested annually through a tabletop exercise. Customers are notified of confirmed security incidents affecting their data within 72 hours of FinSight AI's determination that a reportable incident has occurred. Customer notification timelines are contractually defined and designed to support applicable breach notification, privacy, and bank regulatory obligations. Notification is delivered to the customer's designated security contact and includes a description of the incident, the data potentially affected, and the remediation steps taken or underway. A post-incident report is provided within 30 days of incident closure.

**Relevant trust theme:** Incident response
**Evidence typically requested:** Incident response policy, contractual notification SLA, tabletop exercise summary (redacted)

---

### Q18. Does FinSight AI maintain audit logs of user activity and system events? How long are logs retained?

**Sample response:**
FinSight AI maintains audit logs covering user authentication events, data access, administrative actions, and AI query activity. Each log entry captures the user identity, action type, timestamp, and affected resource. Logs are retained for a minimum of 12 months and are stored in a write-protected environment separate from application infrastructure. Customers can access their own audit logs directly through the platform's administrator interface or via API export. Logs are available in a structured JSON format compatible with standard SIEM tools. Log retention beyond 12 months is available as a configurable option for customers with regulatory requirements.

**Relevant trust theme:** Audit logging and accountability
**Evidence typically requested:** Logging policy, log retention schedule, sample log schema (redacted), SIEM integration documentation

---

## Section 5: AI-Specific Governance and Controls

---

### Q19. How does FinSight AI mitigate prompt injection attacks?

**Sample response:**
FinSight AI applies layered controls to reduce the risk of prompt injection. At the input layer, user-submitted content is parsed and structured before being passed to the model, limiting the ability of malicious input to alter system-level instructions. System prompts are protected from user modification through application-layer controls and are not exposed in API responses or error messages. At the output layer, responses are filtered against a defined content policy before being returned to the user. FinSight AI includes AI-specific attack scenarios -- consistent with the OWASP LLM Top 10 -- in the scope of our annual penetration test. Runtime monitoring is in place to flag anomalous query patterns that may indicate injection attempts, with alerting routed to the security team.

**Relevant trust theme:** AI security and adversarial robustness
**Evidence typically requested:** Technical security architecture documentation, pen test scope confirming OWASP LLM Top 10 coverage, monitoring and alerting policy

---

### Q20. Are AI outputs logged and retained? Can a bank reconstruct what the model produced in response to a specific query?

**Sample response:**
FinSight AI logs all AI-generated outputs. Each log record captures the prompt submitted, the model response, the model version used, the user identity, and the timestamp. These logs are retained for 12 months by default and are accessible to the customer directly through the platform's administrator interface or via API export. Logs are stored in a write-protected environment and are not modified or deleted during the retention period. Customers can use these records to reconstruct any AI interaction for internal audit, regulatory examination support, or dispute resolution. Extended retention periods are available on request for customers with regulatory requirements. Logging configurations may vary by customer requirements, with access restrictions, redaction options, and retention limits available to support privacy and data minimization obligations.

**Relevant trust theme:** AI auditability and accountability
**Evidence typically requested:** Output logging architecture documentation, log retention policy, sample log schema (redacted), contractual log access provision

---

### Q21. How does FinSight AI handle hallucinations or outputs that may be unsupported by source data?

**Sample response:**
FinSight AI uses a retrieval-augmented generation (RAG) architecture for workflows that require factual grounding. In these workflows, model responses are generated from retrieved source documents rather than model weights alone, and each response includes citations to source material so users can verify the basis for the output. For workflows where grounding is not applicable, the platform displays a confidence indicator and a disclaimer that outputs should be reviewed by a qualified professional before being acted upon. FinSight AI does not represent AI-generated outputs as definitive, legally reliable, or a substitute for professional judgment. Internal adversarial testing is conducted to identify output failure modes specific to financial use cases.

**Relevant trust theme:** AI output integrity and risk management
**Evidence typically requested:** RAG architecture documentation, citation feature documentation, internal testing methodology, product disclaimer language

---

### Q22. What is FinSight AI's approach to human oversight for high-impact workflows such as credit analysis, compliance screening, or regulatory reporting?

**Sample response:**
FinSight AI is designed to support analyst workflows rather than replace human judgment in consequential decisions. For use cases identified as high-impact -- including outputs used in credit analysis, regulatory reporting, or compliance screening -- the platform requires user acknowledgment before an output is exported or used to trigger a downstream action. FinSight AI does not autonomously submit filings, execute transactions, or initiate downstream system actions without a human step in the workflow. Human review reduces risk in high-impact workflows but does not automatically remove a use case from high-risk treatment under frameworks such as the EU AI Act, where classification depends on whether the AI system materially influences a consequential decision. Customers deploying the platform in Annex III-adjacent workflows are encouraged to conduct their own regulatory review. Customers can configure additional approval gates through the platform's workflow settings. Documentation on human-in-the-loop workflow design is included in our product guide and available during implementation.

**Relevant trust theme:** Human oversight and AI governance
**Evidence typically requested:** Product documentation on workflow controls, human-in-the-loop configuration guide, use case risk assessment

---

### Q23. How does FinSight AI classify its product under the EU AI Act? Has a risk assessment been conducted?

**Sample response:**
For purposes of this sample, FinSight AI has prepared an internal EU AI Act classification memo. The product is designed as analyst-support software rather than autonomous decisioning software, which informs the current classification analysis. At the platform level, FinSight AI's core functionality does not make or directly output decisions in the Annex III categories. The current classification positions the core platform at the limited-risk tier under Article 50, where the primary transparency obligation is disclosure: users are informed when they are interacting with AI-generated output. This disclosure is implemented at the product level and documented in our user-facing terms of service.

However, customer deployments involving use cases such as creditworthiness assessment, credit scoring, employment screening, or other Annex III-adjacent workflows would require deployment-specific legal review and may be subject to high-risk obligations regardless of the vendor's product-level classification. A vendor-level classification does not substitute for customer-level analysis of how the tool is actually deployed.

We maintain technical documentation and a system description consistent with EU AI Act transparency requirements and have engaged external legal counsel to review our classification approach. We are prepared to share our classification rationale and supporting documentation with customers on request.

**Relevant trust theme:** Regulatory classification and AI governance
**Evidence typically requested:** EU AI Act classification memo (on request), technical system description, counsel engagement summary, product transparency disclosures

---

### Q24. Who are FinSight AI's AI model subprocessors? What data do they receive, and under what contractual terms?

**Sample response:**
FinSight AI uses a commercial foundation model API as its primary inference layer. Customer prompts and associated context are transmitted to the model provider's API for inference and are not used for model training. Any provider-side retention is limited to the terms documented in the subprocessor agreement. The model provider operates under a data processing agreement that prohibits use of API data for model training. FinSight AI maintains a current subprocessor list that is updated when material changes occur. Customers are notified of new or changed subprocessors with a minimum of 30 days' notice, as provided in our DPA. A full subprocessor list including processing locations and data categories is available as part of our DPA package.

**Relevant trust theme:** Third-party and subprocessor risk
**Evidence typically requested:** Subprocessor list with roles and locations, model provider DPA summary (under NDA), data flow diagram, subprocessor notification process documentation

---

## Section 6: Financial-Services Diligence

---

### Q25. Can FinSight AI support a bank's regulatory examination process -- for example, by producing audit logs, responding to examiner questions, or restricting access during an exam?

**Sample response:**
FinSight AI is prepared to support bank customers during regulatory examinations. Upon documented request coordinated through the customer, we can produce audit logs, user access records, and AI output logs in structured formats suitable for examiner review. We maintain a designated point of contact for regulatory inquiries and can respond to standard document requests within five business days. Customers subject to OCC, FDIC, Federal Reserve, PRA, or ECB SSM oversight may reference our SOC 2 Type II report and DPA in their vendor risk submissions. We are available to respond to written examiner questions and can participate in examiner interviews at the customer's request, subject to applicable confidentiality constraints.

**Relevant trust theme:** Regulatory exam readiness and financial-services vendor risk
**Evidence typically requested:** Regulatory support policy, log production capability documentation, SOC 2 report, designated regulatory contact information

---

*This document is a fictional sample created for educational and portfolio purposes. FinSight AI is not a real company. Sample responses do not reflect any real company's controls or compliance posture and would require validation by qualified security, legal, and compliance professionals before use in a real diligence process.*
