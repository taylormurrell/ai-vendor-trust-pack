# Control Theme Mapping
## FinSight AI -- Bank Questionnaire Control Theme Mapping

This table connects the six questionnaire areas to the frameworks and themes that typically inform bank diligence in each area. It is not a formal controls matrix or certification claim. It is a reference for understanding which frameworks are relevant to which buyer concerns.

This file is designed to help a questionnaire owner connect common customer questions to the most relevant control themes and evidence artifacts, not to serve as a formal framework-to-control crosswalk.

**Fictional sample. For educational and portfolio purposes only.**

---

| Questionnaire area | Example customer concern | Relevant framework / theme | Example evidence artifact |
|---|---|---|---|
| Company and compliance posture | Has the vendor's security program been independently validated over time? | SOC 2 Security (Trust Services Criteria CC1-CC9) | SOC 2 Type II report (under NDA), bridge letter |
| Company and compliance posture | Does the vendor have a structured, risk-based approach to managing information security? | ISO 27001 -- information security management system and risk treatment | ISO 27001 certificate or gap assessment, risk register summary |
| Company and compliance posture | Has the vendor been adversarially tested by a third party? | SOC 2 CC7 (vulnerability and threat management) | Penetration test executive summary (under NDA) |
| Data protection and privacy | Is customer data protected from unauthorized access or misuse? | SOC 2 Confidentiality / GDPR Article 5 (purpose limitation and data minimization) | DPA, SOC 2 confidentiality section, encryption policy |
| Data protection and privacy | Can the vendor honor individual deletion requests? | GDPR Article 17 (right to erasure) | Data subject request process documentation, sample deletion confirmation |
| Data protection and privacy | Does customer data leave the customer's jurisdiction, and under what legal basis? | GDPR Chapter V (cross-border transfers) / local banking data residency requirements | DPA with SCCs, data flow diagram, subprocessor list with locations |
| Data protection and privacy | Does customer data train the vendor's or provider's AI models? | ISO 42001 (AI management system) / GDPR purpose limitation / SOC 2 Confidentiality | DPA training prohibition clause, model subprocessor agreement, written attestation |
| Access control and identity | Can the bank enforce its own identity policies on the vendor platform? | ISO 27001 A.9 (access control) / SOC 2 CC6 (logical and physical access) | SSO and SAML integration documentation, SCIM provisioning guide |
| Access control and identity | Who inside the vendor organization can read customer data, and when? | ISO 27001 A.9.2 (user access management) / SOC 2 CC6 | Access control policy, privileged access review records, quarterly audit logs |
| Cloud and infrastructure security | Where is customer data physically and logically processed? | Data residency and cloud processing transparency / GDPR Chapter V where cross-border transfers apply / U.S. bank third-party risk expectations / CSA CCM or ISO 27017 for cloud-specific mapping | Infrastructure architecture overview, data residency attestation, subprocessor list with locations |
| Cloud and infrastructure security | Can one customer's data be accessed by another in a shared environment? | SOC 2 CC6 logical access / ISO 27001 access control / cloud tenant isolation / ISO 27017 as supporting cloud-specific guidance | Architecture documentation, penetration test scope confirming tenant isolation coverage, SOC 2 logical separation section |
| Cloud and infrastructure security | How does the vendor respond to and notify customers of security incidents? | SOC 2 CC7 incident response / contractual customer notification SLA / GDPR Articles 33 and 34 where personal data is affected / financial-sector notification expectations (timeline and scope depend on incident type, customer contract, and jurisdiction) | Incident response policy, contractual notification SLA, tabletop exercise summary |
| AI-specific governance and controls | Can the AI system be manipulated through adversarial input? | ISO 42001 AI risk management / OWASP LLM Top 10 | Penetration test scope (confirming AI-specific coverage), technical controls documentation |
| AI-specific governance and controls | Can the bank reconstruct what the AI produced for a given query? | EU AI Act Article 13 (transparency and provision of information) / financial-services audit requirements | Output logging architecture, log schema, audit interface documentation |
| AI-specific governance and controls | Is the product classified appropriately under AI governance regimes? | EU AI Act risk classification and transparency obligations / ISO 42001 AI management system | EU AI Act classification memo, technical system description, counsel engagement summary |
| AI-specific governance and controls | Is there human oversight built into high-impact workflows? | EU AI Act Article 14 (human oversight) / ISO 42001 operational controls | Human-in-the-loop configuration documentation, workflow design guide, use case risk assessment |
| Financial-services diligence | Can the vendor support the bank during a regulatory examination? | U.S. interagency third-party risk management guidance, FFIEC IT Examination Handbook themes, and applicable bank service-provider expectations (DORA Article 30 for EU entities) | Regulatory support policy, log production documentation, designated regulatory contact |

---

**Framework reference guide**

- **SOC 2** -- Service Organization Control 2. An independent audit framework developed by the AICPA. Type II reports cover a period of time (typically 6-12 months). The Security trust service criterion (formerly Common Criteria) is the most widely required by banks.
- **ISO 27001** -- International standard for information security management systems. Not the same as SOC 2; the two can complement each other. Certification requires third-party audit against the standard.
- **ISO 42001** -- International standard for AI management systems, published in 2023. Provides a framework for governing AI programs within an organization, analogous to how ISO 27001 governs information security. Not yet widely required by banks but increasingly referenced.
- **GDPR** -- EU General Data Protection Regulation. Applies to any organization processing personal data of EU residents. DPA and SCC requirements apply to vendor relationships.
- **EU AI Act** -- EU regulation assigning risk classifications to AI systems (unacceptable, high, limited, minimal) and imposing requirements based on classification. Applies to systems deployed in the EU, including by non-EU vendors.
- **OWASP LLM Top 10** -- A list of the top security risks specific to large language model applications, maintained by OWASP. Distinct from the standard OWASP Web Application Top 10.
- **U.S. interagency third-party risk management guidance / FFIEC** -- Joint guidance issued by the OCC, Federal Reserve, and FDIC governing how banks manage third-party relationships, including due diligence, ongoing monitoring, and contract requirements. The 2023 interagency guidance superseded earlier agency-specific bulletins. FFIEC IT Examination Handbook themes apply across US banking regulators.
- **DORA** -- EU Digital Operational Resilience Act. Applies to financial entities in the EU and their ICT third-party providers. Covers incident reporting, resilience testing, and third-party risk requirements.
- **ISO 27017** -- International standard providing cloud-specific security controls, supplementing ISO 27001. Referenced as optional supporting guidance for cloud infrastructure and tenant isolation rows.

---

*This document is a fictional sample created for educational and portfolio purposes. It does not constitute a compliance claim, controls attestation, or legal representation. Framework references are provided for educational context only.*
