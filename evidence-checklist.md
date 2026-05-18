# Evidence Checklist
## AI Vendor Diligence -- Artifacts to Prepare

A practical checklist of artifacts an AI vendor should have ready before entering bank diligence. Organized by area, with the reason a bank asks for each item and the internal team most likely to own it.

**Fictional sample. For educational and portfolio purposes only.**

---

## Security Governance

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| SOC 2 Type II report (under NDA) | Third-party attestation that security controls worked over a period of time, not just at a point in time | Security / Compliance |
| Bridge letter (if report is more than 6 months old) | Attests that no material changes to the control environment have occurred since the audit period closed | Security / Compliance |
| Information security policy (summary) | Confirms controls are formally documented and maintained, not just practiced informally | Security |
| Annual policy review attestation | Shows the policy is current and actively maintained | Security |
| Penetration test executive summary (under NDA) | External adversarial validation of the production environment -- self-assessments are not accepted as a substitute | Security |
| Pen test remediation log or attestation | Confirms that critical and high findings from the most recent test were resolved, not left open | Security |
| Vulnerability management policy with SLA table | Shows that vulnerabilities are tracked and remediated within defined and enforceable timelines | Security |
| ISO 27001 certificate or gap assessment (if applicable) | Signals a structured, risk-based approach to information security management; increasingly expected by EU buyers | Security / Compliance |

---

## Data Protection

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Data Processing Agreement (DPA) | Establishes the legal framework for data handling, retention, deletion, and customer rights | Legal |
| Standard Contractual Clauses (SCCs) addendum | Required for GDPR-compliant transfer of personal data from the EU to other jurisdictions | Legal |
| Data flow diagram | Visual map showing where customer data travels -- including to third-party model providers -- within and beyond the vendor's infrastructure | Security / Engineering |
| Subprocessor list with roles and processing locations | Required for the bank to conduct fourth-party risk assessment and satisfy its own regulatory requirements | Legal / Privacy |
| Data retention policy | Documents how long data is kept, what triggers deletion, and how this is enforced technically | Legal / Privacy |
| Data deletion process documentation | Demonstrates operational capability to fulfill deletion requests, not just a contractual promise | Legal / Engineering |
| Sample deletion confirmation | Shows what the bank receives as proof that a deletion request was fulfilled | Legal / Operations |

---

## Access Control

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Access control policy | Documents how access to customer data and production systems is granted, reviewed, and revoked | Security |
| Privileged access review records | Evidence that access is audited regularly -- not just granted at onboarding and forgotten | Security |
| MFA policy | Confirms that multi-factor authentication is mandatory, not optional, for internal access | Security / IT |
| SSO and SAML integration documentation | Confirms the vendor supports the bank's identity provider and can delegate authentication | Engineering / IT |
| SCIM provisioning guide (if supported) | Shows that user lifecycle management can be automated through the bank's IdP | Engineering |
| RBAC model documentation | Describes what roles exist, what permissions each role carries, and how roles are assigned | Security / Engineering |

---

## Cloud Infrastructure

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Infrastructure architecture overview | Gives the bank a map of where processing occurs and how the environment is structured | Engineering / Security |
| Data residency attestation | Confirms that data does not leave approved jurisdictions without appropriate legal mechanisms | Legal / Engineering |
| Cloud provider shared responsibility model reference | Clarifies which controls belong to the vendor vs. the cloud provider -- important for understanding gaps | Security |
| Tenant isolation architecture documentation | Describes the mechanism used to prevent one customer's data from being accessible to another | Engineering / Security |

---

## AI Governance

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Model subprocessor agreement summary (under NDA) | Confirms the model provider cannot use customer data for training and is bound by appropriate contractual restrictions | Legal |
| Training prohibition attestation (written) | A named officer's written confirmation that customer data is not used for model training or improvement | Legal / Security |
| EU AI Act classification memo | Documents the vendor's analysis of where the product sits in the risk taxonomy and the reasoning behind the classification | Legal / Compliance |
| Technical system description (Article 11, if high-risk) | Required documentation for high-risk AI systems under the EU AI Act | Legal / Engineering |
| AI output logging architecture documentation | Demonstrates that AI interactions can be reconstructed for audit, regulatory examination, or legal purposes | Engineering / Security |
| Output log schema (redacted sample) | Shows what data is captured in each log record so the bank can assess whether it meets their audit requirements | Engineering |
| Prompt injection mitigation documentation | Describes the specific technical controls in place against AI-specific adversarial attacks | Security / Engineering |
| OWASP LLM Top 10 pen test scope confirmation | Confirms that AI-specific attack vectors were in scope for adversarial testing, not just standard web application attacks | Security |
| AI use case risk assessment | Documents which workflows have been assessed for high-impact risk and what human oversight is in place | Product / Compliance |
| Human-in-the-loop configuration guide | Shows how customers can configure or verify human review steps for high-impact workflows | Product / Engineering |

---

## Incident Response

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Incident response plan (summary or full, under NDA) | Documents the process for detecting, containing, and recovering from security incidents | Security |
| Contractual notification SLA | Confirms the timeline within which the bank will be notified of a breach affecting their data -- must meet GDPR (72 hours) and relevant banking regulatory requirements | Legal / Security |
| Tabletop exercise summary | Evidence that the incident response plan has been tested under realistic conditions, not just written and filed | Security |
| Post-incident report template | Shows the bank what to expect after an incident is resolved -- typically due within 30 days of closure | Security |

---

## Business Continuity

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Business continuity plan (BCP) summary | Documents how the vendor maintains operations during disruptions -- relevant for banking regulators who assess operational resilience | Operations / Security |
| Disaster recovery plan (DRP) with RTO and RPO | Specifies how quickly the vendor can restore service (RTO) and how much data loss is acceptable (RPO) -- banks need these numbers to assess their own resilience posture | Engineering / Operations |
| Historical uptime data or SLA documentation | Gives the bank a track record to evaluate reliability and understand remedies for downtime | Operations / Legal |

---

## Third-Party Risk

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Full subprocessor list with roles and locations | Required for the bank to conduct fourth-party risk assessment -- regulators expect banks to know where their data goes through the vendor supply chain | Legal / Procurement |
| Vendor risk management policy | Shows the vendor assesses and monitors its own suppliers, not just its internal controls | Security / Legal |
| Critical subprocessor SOC 2 report or attestation | Evidence that key suppliers -- particularly the AI model provider -- are also subject to independent control validation | Security / Compliance |

---

## Customer-Facing Documentation

| Artifact | Why a bank asks for it | Likely internal owner |
|---|---|---|
| Trust portal or security overview page | Centralized, self-serve reference for common diligence questions -- reduces back-and-forth during sales cycles | Security / Marketing |
| Executed DPA (customer-specific copy) | The agreed-upon legal framework for the specific customer relationship -- not a template, but a signed agreement | Legal |
| Pre-built DDQ response library | Pre-drafted answers to common diligence questions, available under NDA -- shortens the questionnaire review cycle | Customer Trust / Security |
| Audit log access guide | Instructions for how a bank can access, filter, and interpret their own audit and output logs | Engineering / Customer Success |
| Regulatory exam support policy | Documents what the vendor will produce, in what format, and within what timeline in response to examiner requests | Legal / Security |
| Product disclaimer language | Customer-visible language clarifying that AI outputs should be reviewed by a qualified professional before being acted upon | Legal / Product |

---

*This checklist is a fictional sample created for educational and portfolio purposes. It does not represent a complete compliance program or a legal requirement. Actual artifact requirements vary by customer, jurisdiction, and regulatory context.*
